Berikut catatan `.md` yang merangkum workflow berbasis **Sprint Planning + GitLab \+ Claude + VS Code**, termasuk pembagian tanggung jawab dan mekanisme commit/push.

 Sprint-Based AI-Assisted Development Workflow

# Sprint-Based AI-Assisted Development Workflow

 ## 1\. Prinsip Utama

 Dalam workflow berbasis Sprint:

 > **Human menentukan WHAT dan WHY. Claude membantu menentukan HOW dan WHERE. GitLab menjadi source of truth untuk pekerjaan.**

 Pembagian utama:

```
Human
  │
  ├── Requirement
  ├── Sprint Planning
  ├── Approval
  ├── Code Review
  └── Merge Decision
  │
  ▼
Claude
  │
  ├── Technical Discovery
  ├── Codebase Analysis
  ├── Planning
  ├── Implementation
  ├── Testing Assistance
  └── Review Assistance
  │
  ▼
GitLab
  │
  ├── Work Items
  ├── Branches
  ├── Commits
  ├── Merge Requests
  └── Merge
```

---

 # 2\. Sprint Planning

 Work Item dibuat berdasarkan hasil diskusi Sprint Planning oleh human/team.

 Human **tidak harus mengetahui detail teknis** seperti:

 - File mana yang berubah.
- Service mana yang terdampak.
- Database apa yang berubah.
- Berapa banyak file yang terdampak.
- Dependency apa yang perlu digunakan.
- Test apa yang harus ditambahkan.

 Hal tersebut dapat dianalisis oleh Claude setelah Work Item dibuat.

---

 # 3\. GitLab Work Item

 GitLab Work Item menjadi **source of truth untuk requirement**.

 Work Item sebaiknya berisi:

 - Objective.
- Business requirement.
- Acceptance criteria.
- Scope.
- Priority/Sprint.
- Informasi bisnis yang relevan.

 Contoh:

```
# TASK-123: Password Reset

## Objective

Allow users to reset their password when they forget it.

## Acceptance Criteria

- User can request a password reset.
- User receives a reset link.
- Reset token expires.
- User can set a new password.
- Invalid or expired tokens are rejected.

## Sprint

Sprint 24

## Notes

Technical implementation to be investigated.
```

 Work Item menjawab:

 > **WHAT dan WHY?**

 Tidak perlu memaksakan informasi seperti:

```
src/auth/AuthService.ts
src/auth/TokenService.ts
src/users/UserRepository.ts
```

 jika belum diketahui.

---

 # 4\. Technical Discovery dengan Claude

 Setelah Work Item dibuat, Claude digunakan untuk melakukan **technical discovery / impact analysis**.

 Contoh prompt:

```
Analyze GitLab Work Item TASK-123.

Do not modify any files.

I want to understand the technical impact before implementation.

Please inspect the existing codebase and determine:

1. Where the current functionality is implemented.
2. Which components are likely affected.
3. Whether similar functionality already exists.
4. Existing patterns that should be reused.
5. Database/schema impact.
6. API impact.
7. External service impact.
8. Unit/integration tests that may need changes.
9. Dependencies that may be affected.
10. Potential risks.

Use Graphify if it helps understand relationships between components.

Return a concise technical analysis and implementation plan.

Do not make any code changes.
```

 Tujuannya adalah mengetahui:

```
Work Item
    │
    ▼
Claude Discovery
    │
    ├── Existing components
    ├── Affected files
    ├── Dependencies
    ├── Database impact
    ├── API impact
    ├── Test impact
    └── Risks
```

---

 # 5\. Graphify dalam Discovery

 Graphify digunakan **secara situasional**, bukan wajib untuk setiap task.

```
Technical Discovery
        │
        ▼
Apakah relationship codebase kompleks?
        │
     ┌──┴──┐
     │     │
    No    Yes
     │     │
     ▼     ▼
Source   Graphify
Code       │
     │     │
     └──┬──┘
        ▼
Technical Understanding
```

 Graphify membantu menjawab:

 > **"Komponen apa berhubungan dengan komponen lain?"**

 Graphify bukan pengganti Work Item atau `architecture.md`.

---

 # 6\. Technical Plan

 Setelah discovery, Claude membuat technical plan.

 Contoh struktur:

```
## Technical Analysis

### Existing Flow

Controller
    ↓
Service
    ↓
Repository
    ↓
Database

### Existing Components

- AuthController
- AuthService
- TokenService
- UserRepository

### Expected Changes

1. Modify AuthController.
2. Extend AuthService.
3. Reuse TokenService.
4. Modify UserRepository.
5. Add tests.

### Database Impact

Potential schema/migration changes.

### Risks

- Token expiration.
- Token reuse.
- Security considerations.
```

 Claude **belum mengubah code**.

---

 # 7\. Human Approval

 Technical plan harus direview oleh human sebelum implementation.

```
GitLab Work Item
       ↓
Claude Discovery
       ↓
Technical Plan
       ↓
Human Review
       │
   ┌───┴────┐
   │        │
Reject    Approve
   │        │
   ▼        ▼
Revise   Implement
```

 Human memastikan:

 - Scope masih sesuai Sprint.
- Solusi teknis masuk akal.
- Tidak ada perubahan yang tidak diperlukan.
- Risiko dapat diterima.
- Acceptance criteria tetap terpenuhi.

---

 # 8\. Implementation

 Setelah plan disetujui:

```
Plan approved.

Implement the approved plan.

Requirements:

- Follow CLAUDE.md.
- Do not implement unrelated changes.
- Reuse existing abstractions.
- Follow existing project patterns.
- Do not add dependencies unless necessary.
- Add/update relevant tests.
```

 Prinsip:

 > **Implementasi mengikuti plan yang sudah disetujui.**

 Hindari:

 - Refactoring yang tidak berkaitan.
- Abstraction berlebihan.
- Dependency baru tanpa alasan.
- Perubahan file yang tidak berhubungan.

---

 # 9\. Unit Testing

 Test plan sebaiknya sudah dibuat pada tahap planning.

 Contoh:

```
Feature: Password Reset

Expected behavior:

✓ Valid token → password berubah.
✓ Expired token → rejected.
✓ Invalid token → rejected.
✓ Used token → rejected.
✓ Unknown email → appropriate response.
```

 Setelah implementasi:

```
Add or update the relevant tests.

Please:

1. Cover expected behavior.
2. Cover relevant failure cases.
3. Reuse existing testing patterns.
4. Run the relevant test suite.
5. Fix failures caused by our implementation.
```

 Testing bukan hanya aktivitas terakhir.

```
Planning
   ↓
Test Plan
   ↓
Implementation
   ↓
Unit Test
   ↓
Review
   ↓
Final Test
```

---

 # 10\. AI Review

 Setelah implementation dan testing, Claude melakukan review.

 Hal yang diperiksa:

 - Apakah implementation sesuai plan?
- Apakah acceptance criteria terpenuhi?
- Apakah ada unnecessary complexity?
- Apakah ada duplicate functionality?
- Apakah ada security issue?
- Apakah edge case penting sudah ditangani?
- Apakah error handling memadai?
- Apakah ada file yang tidak seharusnya berubah?
- Apakah implementation mengikuti architecture?
- Apakah test sudah memadai?

 Claude sebaiknya **melaporkan masalah terlebih dahulu**, sebelum melakukan perubahan tambahan.

---

 # 11\. Bug vs Improvement

 Hasil review harus dibedakan menjadi dua kategori.

 ## Bug / Defect

 Jika implementation salah atau test gagal:

```
Review
   ↓
Bug found
   ↓
Fix now
   ↓
Test again
```

 Contoh:

```
Password reset menggunakan token
yang sudah expired tetapi tetap berhasil.
```

 Ini harus diperbaiki dalam task tersebut.

 ## Improvement / Out-of-Scope

 Jika ditemukan sesuatu yang tidak diperlukan untuk task:

```
Review
   ↓
Improvement found
   ↓
Create new Work Item
   ↓
Backlog
```

 Contoh:

```
AuthService memiliki refactoring
yang akan membuat code lebih clean,
tetapi tidak diperlukan untuk Password Reset.
```

 Jangan langsung dikerjakan jika tidak termasuk scope.

---

 # 12\. Commit

 Commit dilakukan **setelah implementation, testing, dan review**.

 Recommended flow:

```
Implementation
      ↓
Testing
      ↓
Review
      ↓
Human Approval
      ↓
Commit
```

 Claude dapat membantu melakukan commit.

 Contoh:

```
Review the current changes.

If the implementation and tests are correct,
prepare a commit with an appropriate commit message.

Do not push or merge.
```

 Claude dapat menjalankan Git command seperti:

```
git status
git diff
git add
git commit
```

 Namun human tetap dapat melakukan commit secara manual melalui VS Code.

---

 # 13\. Commit vs Push

 Commit dan push adalah dua hal berbeda.

 ### Commit

```
Local working tree
       ↓
     commit
       ↓
Local Git repository
```

 Artinya perubahan direkam secara lokal.

 ### Push

```
Local Git repository
       ↓
      push
       ↓
GitLab repository
```

 Artinya perubahan dikirim ke repository perusahaan.

 Recommended workflow:

```
Implementation
    ↓
Test
    ↓
Review
    ↓
Human approval
    ↓
Commit
    ↓
Human approval
    ↓
Push
```

 Untuk tahap awal, commit dan push dapat dilakukan manual dari VS Code.

 Setelah workflow sudah stabil, proses mekanis dapat diotomatisasi.

---

 # 14\. Jangan Langsung Memberikan Claude Full Git Control

 Hindari workflow seperti:

```
Implement feature and push everything to GitLab.
```

 Karena terlalu banyak proses terjadi sekaligus:

```
Analyze
   ↓
Code
   ↓
Test
   ↓
Commit
   ↓
Push
```

 Lebih baik menggunakan checkpoint:

```
Planning
   ↓
Human approval
   ↓
Implementation
   ↓
Testing
   ↓
Review
   ↓
Human approval
   ↓
Commit
   ↓
Human approval
   ↓
Push
   ↓
Merge Request
```

 Hal ini memberikan **human-in-the-loop** pada titik penting.

---

 # 15\. Merge Request

 Setelah push:

```
Branch
   ↓
Push
   ↓
GitLab Merge Request
   ↓
Human Code Review
   ↓
Approval
   ↓
Merge
```

 Merge Request menjadi tempat final review terhadap perubahan code.

 Review dapat memeriksa:

 - Requirement.
- Acceptance criteria.
- Technical implementation.
- Test.
- Code quality.
- Scope.
- Security.
- Regression risk.

---

 # 16\. Peran Tools

 ## Human

 Bertanggung jawab atas:

 - Sprint Planning.
- Requirement.
- Business decision.
- Scope.
- Planning approval.
- Code review.
- Merge decision.

 ## Claude

 Membantu:

 - Technical discovery.
- Codebase exploration.
- Impact analysis.
- Planning.
- Implementation.
- Unit testing.
- Review assistance.
- Git operations jika diizinkan.

 ## GitLab

 Menjadi **system of record**:

 - Work Items.
- Sprint.
- Branch.
- Commit.
- Merge Request.
- Review.
- Merge.

 ## VS Code

 Menjadi **human control surface**:

 - Inspect source code.
- Review changes.
- Review Git diff.
- Debugging.
- Run application.
- Run tests.
- Manual modification.

 ## Graphify

 Digunakan saat perlu memahami relationship codebase yang kompleks.

 ## RTK

 Membantu mengurangi output CLI yang masuk ke context Claude.

 ## Ponytail

 Mendukung workflow implementasi yang menghindari perubahan dan abstraction yang tidak perlu.

---

 # 17\. Full Workflow

```
                    SPRINT PLANNING
                           │
                           ▼
                      HUMAN TEAM
                           │
                           ▼
                  GITLAB WORK ITEM
                 WHAT + WHY + AC
                           │
                           ▼
                 CLAUDE DISCOVERY
                           │
                    ┌──────┴──────┐
                    │             │
                 Simple        Complex
                    │             │
                    ▼             ▼
               Source Code     Graphify
                    │             │
                    └──────┬──────┘
                           ▼
                  TECHNICAL PLAN
                           │
                           ▼
                    HUMAN APPROVAL
                           │
                           ▼
                    IMPLEMENTATION
                           │
                           ▼
                      UNIT TEST
                           │
                           ▼
                      AI REVIEW
                           │
                  ┌────────┴────────┐
                  │                 │
                Defect          Improvement
                  │                 │
                  ▼                 ▼
                Fix Now        New Work Item
                  │
                  ▼
               Test Again
                  │
                  ▼
              Review Diff
                  │
                  ▼
             HUMAN APPROVAL
                  │
                  ▼
                COMMIT
                  │
                  ▼
                 PUSH
                  │
                  ▼
          GITLAB MERGE REQUEST
                  │
                  ▼
           HUMAN CODE REVIEW
                  │
                  ▼
                MERGE
                  │
                  ▼
                 DONE
```

---

 # 18\. Prinsip Akhir

 Workflow ini mengikuti prinsip:

 > **Human menentukan tujuan dan keputusan. Claude membantu pekerjaan teknis. GitLab menjaga traceability. VS Code menjadi tempat human mengontrol dan memverifikasi perubahan.**

 Tidak semua proses harus otomatis.

 Untuk tahap awal:

```
Human
   ↓
Claude
   ↓
Human
   ↓
Claude
   ↓
Human
```

 adalah workflow yang baik.

 Setelah pola kerja sudah stabil, baru identifikasi proses yang bersifat mekanis untuk diotomatisasi.

 ## Rule of Thumb

```
WHAT / WHY
    → Human

HOW / WHERE
    → Claude

SOURCE OF TRUTH
    → GitLab

CODE CONTROL & VISUAL REVIEW
    → VS Code

CODE RELATIONSHIP ANALYSIS
    → Graphify

CLI OUTPUT OPTIMIZATION
    → RTK

SIMPLIFICATION / IMPLEMENTATION DISCIPLINE
    → Ponytail
```
