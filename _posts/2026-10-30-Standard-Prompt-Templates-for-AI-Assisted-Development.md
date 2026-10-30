---
layout: post
title: "Standard Prompt Templates for AI-Assisted Development"
date: 2026-10-30 14:00:00 +0700
categories:
  - Software Engineering
  - Prompting
  - Vibe Coding
tags:
  - AI
  - Software Engineering
  - Prompting
  - Vibe Coding
description: "Exploring how AI Standard Prompt Templates for AI-Assisted Development."
---
 # 1\. Tujuan

 Tujuan utama membuat prompt template adalah:

 - Tidak perlu mengarang prompt setiap mengerjakan Work Item.
- Menjaga workflow Claude tetap konsisten.
- Memisahkan tahap discovery, planning, implementation, review, dan testing.
- Mengurangi risiko Claude melakukan pekerjaan di luar scope.
- Menjadikan `CLAUDE.md` sebagai aturan utama project.
- Membuat prompt tetap pendek sehingga context/token tetap efisien.

 Prinsip utama:

 > **`CLAUDE.md` menentukan HOW Claude harus bekerja. Prompt menentukan WHAT Claude harus lakukan sekarang.**

---

 # 2\. Struktur File

 Recommended structure:

```
project/
│
├── CLAUDE.md
│
├── .claude/
│   └── prompts/
│       ├── 01-discovery.md
│       ├── 02-planning.md
│       ├── 03-implementation.md
│       ├── 04-review.md
│       ├── 05-testing.md
│       └── 06-commit.md
│
├── docs/
│   ├── architecture.md
│   ├── database.md
│   └── testing.md
│
├── src/
└── tests/
```

---

 # 3\. Hubungan `CLAUDE.md` dan Prompt

 `CLAUDE.md` berisi **aturan project yang stabil**.

 Contoh:

```
- Follow existing architecture.
- Reuse existing abstractions.
- Avoid unrelated changes.
- Do not add dependencies without justification.
- Follow project testing conventions.
```

 Prompt template berisi **instruksi tahap yang sedang dilakukan**.

 Contoh:

```
Use the discovery workflow.

Analyze the current Work Item.
Do not modify code.
Identify affected components.
```

 Jangan mengulang seluruh isi `CLAUDE.md` di setiap prompt.

 Struktur:

```
CLAUDE.md
    │
    │ Project rules
    ▼
┌─────────────────────────────────────┐
│                                     │
│  Discovery                          │
│  Planning                           │
│  Implementation                     │
│  Review                             │
│  Testing                            │
│  Commit                             │
│                                     │
└─────────────────────────────────────┘
```

---

 # 4\. Template 01 — Discovery

 ## Tujuan

 Memahami technical impact dari Work Item sebelum membuat implementation plan.

 Discovery menjawab:

 > **"Apa yang sudah ada dan apa yang kemungkinan terdampak?"**

 File:

```
.claude/prompts/01-discovery.md
```

 Template:

```
# Technical Discovery

Analyze the provided Work Item and inspect the existing codebase.

## Objective

Determine the technical impact of this Work Item before implementation.

## Instructions

1. Understand the Work Item requirements and acceptance criteria.
2. Inspect the existing implementation.
3. Identify existing functionality that can be reused.
4. Identify relevant modules, components, services, and files.
5. Determine dependencies and relationships between affected components.
6. Identify database/schema impact if applicable.
7. Identify API or external integration impact if applicable.
8. Identify relevant existing tests.
9. Identify potential risks and edge cases.
10. Use Graphify when it helps understand complex code relationships.

Do not modify any files.

Do not implement the feature.

## Output

Return:

### Summary

Brief description of the existing implementation.

### Relevant Components

List relevant components and their responsibilities.

### Affected Areas

Identify likely files/modules that may be affected.

### Existing Patterns

Identify existing implementations or abstractions that should be reused.

### Impact

Describe:

- Application impact
- Database impact
- API impact
- External integration impact
- Testing impact

### Risks

List important risks or unknowns.

### Recommendation

Provide a concise technical direction for the planning stage.
```

---

 # 5\. Template 02 — Planning

 ## Tujuan

 Mengubah hasil discovery menjadi implementation plan yang jelas.

 Planning menjawab:

 > **"Bagaimana task ini akan dikerjakan?"**

 File:

```
.claude/prompts/02-planning.md
```

 Template:

```
# Implementation Planning

Create an implementation plan based on the Work Item and technical discovery.

## Objective

Create a clear, minimal, and actionable implementation plan.

## Instructions

1. Review the Work Item.
2. Review the technical discovery.
3. Inspect additional source code when necessary.
4. Reuse existing architecture and patterns.
5. Avoid unnecessary abstractions.
6. Keep the scope limited to the Work Item.
7. Identify required database, API, and integration changes.
8. Define the testing strategy.
9. Identify risks and unresolved questions.

Do not modify any files.

Do not implement the solution.

## Output

Return:

### Goal

What the implementation must achieve.

### Implementation Plan

Provide ordered implementation steps.

For each step include:

- Component/file
- Purpose
- Expected change

### Data Changes

Describe required schema/migration changes, if any.

### API Changes

Describe required API changes, if any.

### Testing Plan

Describe:

- Unit tests
- Integration tests
- Edge cases

### Risks

List relevant risks.

### Unresolved Questions

List anything that requires human clarification.

### Scope Check

Explicitly identify anything that should NOT be implemented because it is outside the Work Item scope.
```

 Setelah planning selesai:

```
Human Review
     ↓
Approve
     ↓
Implementation
```

---

 # 6\. Template 03 — Implementation

 ## Tujuan

 Mengimplementasikan plan yang sudah disetujui.

 File:

```
.claude/prompts/03-implementation.md
```

 Template:

```
# Implementation

Implement the approved plan for the current Work Item.

## Preconditions

The implementation plan has been reviewed and approved by a human.

## Instructions

1. Follow the approved implementation plan.
2. Follow CLAUDE.md and existing project conventions.
3. Inspect existing code before modifying it.
4. Reuse existing components and abstractions where appropriate.
5. Make the smallest reasonable change.
6. Do not implement unrelated improvements.
7. Do not introduce dependencies unless necessary.
8. Do not modify unrelated files.
9. Add or update relevant tests.
10. Preserve existing behavior outside the Work Item scope.

If the approved plan appears incorrect or incomplete:

- Stop implementation.
- Explain the issue.
- Do not silently change the architectural approach.

## After Implementation

Run the relevant tests.

Then report:

### Changes Made

List changed files and summarize each change.

### Tests

List tests executed and their results.

### Potential Issues

List remaining concerns.

### Scope Check

Confirm whether unrelated files or functionality were modified.
```

 Prinsip penting:

 > **Claude tidak boleh diam-diam mengubah approved plan.**

 Jika menemukan masalah:

```
Plan
 ↓
Problem discovered
 ↓
STOP
 ↓
Human review
 ↓
Update plan
 ↓
Continue implementation
```

---

 # 7\. Template 04 — Review

 ## Tujuan

 Melakukan review terhadap implementation tanpa langsung mengubah code.

 File:

```
.claude/prompts/04-review.md
```

 Template:

```
# Implementation Review

Review the current implementation against the approved plan and Work Item.

## Important

Do not modify any files during this review.

## Review Objectives

Check:

1. Requirement compliance.
2. Acceptance criteria.
3. Alignment with the approved plan.
4. Architecture consistency.
5. Existing code reuse.
6. Unnecessary complexity.
7. Duplicate functionality.
8. Error handling.
9. Security concerns.
10. Edge cases.
11. Test coverage.
12. Unrelated changes.
13. Potential regressions.

## Review Output

Return findings grouped by severity:

### Critical

Issues that must be fixed before proceeding.

### Important

Issues that should be addressed before merge.

### Minor

Non-blocking observations.

### Out of Scope

Improvements that should become separate Work Items rather than being implemented now.

For every finding include:

- Location
- Problem
- Why it matters
- Recommended action

Do not fix anything yet.
```

 Review harus bersifat **read-only terlebih dahulu**.

---

 # 8\. Template 05 — Testing

 ## Tujuan

 Melakukan verification terhadap implementation dan acceptance criteria.

 File:

```
.claude/prompts/05-testing.md
```

 Template:

```
# Testing and Verification

Verify the implementation against the Work Item and acceptance criteria.

## Instructions

1. Inspect the changed files.
2. Inspect existing tests.
3. Review the acceptance criteria.
4. Identify missing test coverage.
5. Run the most relevant tests.
6. Run broader tests when appropriate.
7. Do not weaken existing tests to make them pass.
8. Do not modify production code during verification unless explicitly requested.

## Verify

### Acceptance Criteria

For each acceptance criterion:

- PASS
- FAIL
- NOT VERIFIED

Provide evidence for each result.

### Unit Tests

Report:

- Tests executed
- Tests passed
- Tests failed

### Integration Tests

Run when relevant.

### Regression

Identify whether existing functionality may be affected.

### Final Result

Return:

- PASS
- PASS WITH WARNINGS
- FAIL

Explain the result.
```

 Testing harus memiliki hubungan dengan acceptance criteria:

```
Acceptance Criteria
        ↓
Test Plan
        ↓
Implementation
        ↓
Tests
        ↓
Verification
```

---

 # 9\. Template 06 — Commit Preparation

 ## Tujuan

 Memastikan perubahan siap di-commit tanpa langsung melakukan push atau merge.

 File:

```
.claude/prompts/06-commit.md
```

 Template:

```
# Commit Preparation

Prepare the current implementation for commit.

## Preconditions

- Implementation is complete.
- Relevant tests have been executed.
- Review has been completed.
- No unresolved blocking issues remain.

## Instructions

1. Inspect git status.
2. Inspect the complete diff.
3. Ensure there are no unrelated changes.
4. Confirm tests are passing.
5. Suggest an appropriate commit message.
6. Do not push.
7. Do not merge.

## Output

Return:

### Changed Files

List changed files.

### Test Status

Summarize relevant test results.

### Commit Message

Provide one recommended commit message.

### Scope Check

Confirm whether unrelated changes are present.

### Commit Readiness

READY / NOT READY
```

 Setelah Claude menyatakan:

```
READY
```

 human dapat memberikan approval untuk commit.

---

 # 10\. Workflow Penggunaan Template

 Workflow standar menjadi:

```
GitLab Work Item
       │
       ▼
01 Discovery
       │
       ▼
02 Planning
       │
       ▼
Human Approval
       │
       ▼
03 Implementation
       │
       ▼
05 Testing
       │
       ▼
04 Review
       │
       ├── Bug
       │    ↓
       │  Fix
       │    ↓
       │  Test Again
       │
       └── Improvement
            ↓
        New Work Item
       │
       ▼
06 Commit
       │
       ▼
Push
       │
       ▼
GitLab Merge Request
       │
       ▼
Human Review
       │
       ▼
Merge
```

---

 # 11\. Mengapa Discovery dan Planning Dipisahkan?

 Discovery:

 > **"Apa yang ada sekarang?"**

 Planning:

 > **"Apa yang harus kita ubah?"**

 Contoh:

```
Discovery

AuthController
    ↓
AuthService
    ↓
TokenService
    ↓
UserRepository
```

 Kemudian Planning:

```
1. Extend AuthService.
2. Reuse TokenService.
3. Modify UserRepository.
4. Add reset endpoint.
5. Add unit tests.
```

 Pemisahan ini mencegah Claude terlalu cepat coding sebelum memahami codebase.

---

 # 12\. Jangan Duplikasi `CLAUDE.md`

 Hindari template seperti:

```
Follow CLAUDE.md.

- Do not modify unrelated files.
- Reuse existing abstractions.
- Do not add dependencies.
- Follow architecture.
- Follow testing conventions.
...
```

 Jika aturan tersebut sudah berada di `CLAUDE.md`, tidak perlu diulang.

 Lebih baik:

```
Follow CLAUDE.md and the approved plan.
```

 Dengan demikian:

```
CLAUDE.md
    ↓
Global project rules

Prompt
    ↓
Current task instructions
```

---

 # 13\. Penggunaan Documentation

 `docs/architecture.md`, `docs/database.md`, dan `docs/testing.md` dibaca **ketika relevan**.

 Contoh:

```
Task sederhana
     ↓
CLAUDE.md
     ↓
Prompt
     ↓
Done
```

 Task kompleks:

```
CLAUDE.md
     ↓
Discovery
     ↓
architecture.md
     ↓
Graphify
     ↓
Planning
```

 Task database:

```
CLAUDE.md
     ↓
Discovery
     ↓
database.md
     ↓
Database schema
     ↓
Planning
```

 Task testing:

```
CLAUDE.md
     ↓
testing.md
     ↓
Test implementation
```

 Jangan memaksa semua dokumentasi dibaca pada setiap task.

---

 # 14\. Prinsip Hemat Token

 Gunakan prinsip:

 > **Load context only when needed.**

 Hindari:

```
Every prompt
    ↓
CLAUDE.md
    +
architecture.md
    +
database.md
    +
testing.md
    +
Graphify
    ↓
Huge context
```

 Lebih baik:

```
Simple task
    ↓
CLAUDE.md
    +
relevant source
```

 atau:

```
Complex architecture task
    ↓
CLAUDE.md
    +
architecture.md
    +
Graphify
    +
relevant source
```

---

 # 15\. Human Approval Gates

 Workflow memiliki beberapa approval gate:

```
Work Item
   ↓
Discovery
   ↓
Planning
   ↓
🔵 HUMAN APPROVAL
   ↓
Implementation
   ↓
Testing
   ↓
Review
   ↓
🔵 HUMAN APPROVAL
   ↓
Commit
   ↓
🔵 HUMAN APPROVAL
   ↓
Push
   ↓
Merge Request
   ↓
🔵 HUMAN CODE REVIEW
   ↓
Merge
```

 Tujuan approval gate:

 - Mencegah AI mengubah scope.
- Mencegah AI mengubah architecture tanpa persetujuan.
- Mencegah perubahan yang belum diverifikasi masuk repository.
- Menjaga human tetap menjadi decision maker.

---

 # 16\. Tahap Berikutnya: Automation

 Jangan langsung membuat automation.

 Tahap awal:

```
Use .claude/prompts/01-discovery.md
Use .claude/prompts/02-planning.md
Use .claude/prompts/03-implementation.md
...
```

 Setelah workflow stabil, template dapat diubah menjadi command/skill:

```
/discover TASK-123
/plan TASK-123
/implement TASK-123
/review TASK-123
/test TASK-123
/commit TASK-123
```

 Sehingga workflow akhirnya menjadi:

```
/discover
    ↓
/plan
    ↓
Human Approval
    ↓
/implement
    ↓
/test
    ↓
/review
    ↓
/commit
    ↓
GitLab MR
```

 Automation dilakukan **setelah workflow manual terbukti stabil**, bukan sebelum memahami prosesnya.

---

 # 17\. Prinsip Akhir

```
CLAUDE.md
    =
Project Rules

Prompt Template
    =
Stage Instructions

Work Item
    =
Business Requirement

Discovery
    =
Understand Existing System

Planning
    =
Decide Implementation Approach

Implementation
    =
Modify Code

Testing
    =
Verify Behavior

Review
    =
Find Problems

Commit
    =
Record Approved Changes

GitLab MR
    =
Human Final Review
```

 Prinsip utama:

 > **Jangan membuat Claude melakukan semuanya dalam satu prompt. Pecah pekerjaan berdasarkan tahap sehingga setiap tahap memiliki tujuan, output, dan approval yang jelas.**

 Dengan struktur ini, prompt menjadi **repeatable, konsisten, mudah diperbaiki, dan lebih hemat context** dibandingkan membuat prompt baru secara manual untuk setiap Work Item.
