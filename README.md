# OrangeHRM Manual QA Testing Project

A self-initiated, end-to-end manual testing project built on the [OrangeHRM Open Source demo application](https://opensource-demo.orangehrmlive.com), created to demonstrate the full manual QA lifecycle for a resume/portfolio.

## What's in this project

| File | Description |
|---|---|
| `Test_Plan_OrangeHRM.docx` | Scope, strategy, test environment, entry/exit criteria, risks, and schedule |
| `Test_Cases_OrangeHRM.xlsx` | 33 detailed test cases across 6 modules, with a Summary tab (pass/fail metrics by module) |
| `Bug_Report_Log_OrangeHRM.xlsx` | 4 sample defects logged from failed test cases, with severity/priority and repro steps |
| `Test_Summary_Report_OrangeHRM.docx` | Final execution report: metrics, module-wise results, key defects, recommendations |
| `Traceability_Matrix_OrangeHRM.xlsx` | 29 requirements mapped to all 33 test cases, with a Coverage Summary tab (100% requirement coverage) |

## Modules covered

- **Login / Authentication** — valid/invalid credentials, field validation, forgot password, logout
- **Admin — User Management** — add/edit/delete/search system users
- **PIM** — add employee, search/filter employee list, file upload validation
- **Leave** — apply leave, date validation, cancel leave, My Leave list
- **Recruitment** — add candidate, email validation, resume upload
- **Dashboard** — widget load, navigation

## Approach

- **Test design techniques:** Equivalence Partitioning, Boundary Value Analysis, Error Guessing, Decision Table Testing
- **Test types:** Positive, negative, boundary, and UI validation scenarios
- **Defect lifecycle:** Logged with severity/priority, mapped back to the originating test case ID
- **Tools used:** Excel for test case management and defect tracking, Word for planning/reporting — mirroring lightweight QA tooling used at small-to-mid-size companies

## Results snapshot

- 33 test cases executed → **29 passed / 4 failed** (87.9% pass rate)
- 4 defects logged (1 High, 2 Medium, 1 Low severity)
- 1 High-severity defect (invalid leave date range accepted) recommended as a blocker for release sign-off
