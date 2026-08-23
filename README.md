# OsdagBridge Testing Submission

This repository contains the functional testing artifacts, documentation, and test case files submitted for the **OsdagBridge Software Testing & Issue Reporting** screening task (FOSSEE Osdag project).

## Repository Contents

```
├── screenshots/              # Screenshots documenting each test case and observed behavior
├── test_notes.md             # Detailed log of all test cases (working and failed)
├── test_cases.osi/                # Saved .osi input files for each test scenario
├── osdagbridge_testing_report.pdf   # Compiled PDF testing report
└── README.md                 # This file
```

## Summary of Work

Testing covered the following areas of OsdagBridge:

- **Input validation** - boundary values, invalid inputs, decimal precision handling across Basic Inputs fields (Span, Carriageway Width, Skew Angle, etc.)
- **Custom property testing** - verifying custom girder/geometric properties (e.g. custom Number of Girders) are correctly registered and reflected in design output, rather than defaulting
- **Multi-run stability** - three consecutive design runs with modified parameters, checking for stale data, crashes, or inconsistent 3D/graphical output
- **UI/menu functionality** - Structure Type dropdown, Graphics/Database/Help menu bar, input panel lock behavior after running Design
- **3D CAD output verification** - confirming the 3D model and summary panel values match the entered UI inputs

Full details, methodology, and observations for each test case are documented in [`osdagbridge_testing_report.pdf`](./osdagbridge_testing_report.pdf) and [`test_notes.md`](./test_notes.md).

## Issues Filed

| Issue | Title | Severity | Link |
|---|---|---|---|
| #53 | Graphics, Database, and Help menu dropdowns open but options are unresponsive | Medium | [View Issue](https://github.com/Nidhikhare12/OsdagBridge/issues/53) |

## Video Demonstration

A screencast demonstrating the testing workflow — including a custom material input run, a consecutive multi-run sequence, and the resulting 3D CAD output — is available here:




## Test Case Files

The `test_cases/` folder contains saved `.osi` input files for each distinct scenario tested, so that any test case can be reproduced exactly by loading the file in OsdagBridge:
- `multirun_test1.osi`
- `multirun_test2.osi`
- `multirun_test3.osi`

## Author

Richa Devaraj
Submitted as part of the FOSSEE Osdag Fellowship screening process.
