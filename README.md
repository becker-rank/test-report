# Test Documentation Repository

This repository stores the test documentation and test execution records for the project.

The repository is organized to separate test definitions from completed test records.

## Repository Structure

```text
.
├── test_definitions/
│   └── adcs/
│       ├── test_index.md
│       └── ADCS-001_magnetometer_functional_test/
│           ├── README.md
│           ├── ADCS-001_magnetometer_functional_test_form.tex
│           ├── ADCS-001_magnetometer_functional_test_fillable.pdf
│           └── procedure.pdf
│
├── test_records/
│   ├── README.md
│   └── adcs/
│       └── ADCS-001_magnetometer_functional_test/
│           ├── README.md
│           └── YYYY-MM-DD_run-XX/
│               ├── completed_form.pdf
│               ├── raw_data/
│               ├── images/
│               ├── plots/
│               ├── logs/
│               └── notes.md
│
├── .gitignore
└── README.md
```

## Folder Description

### `test_definitions/`

This folder contains the definition of each test.

It includes templates, fillable forms, procedures, instructions, references, and any other files needed to describe how a test should be performed.

Files in this folder should not contain completed test results.

### `test_records/`

This folder contains the records of tests that have already been executed.

Each test execution should have its own folder and may include completed forms, raw data, images, plots, logs, notes, and other evidence collected during the test.

For each test, records should be organized under the corresponding subsystem and test ID folder.

Example structure for an executed ADCS-001 test:

```text
test_records/
└── adcs/
    └── ADCS-001_magnetometer_functional_test/
        ├── README.md
        └── 2026-07-11_run-01/
            ├── completed_form.pdf
            ├── raw_data/
            ├── images/
            ├── plots/
            ├── logs/
            └── notes.md
```

## Test Definition Naming Convention

Each test definition should follow this format:

```text
<SUBSYSTEM>-<NUMBER>_<short_test_name>
```

Example:

```text
ADCS-001_magnetometer_functional_test
```

## Test Record Naming Convention

Each executed test should be stored using the following format:

```text
YYYY-MM-DD_run-XX
```

Example:

```text
test_records/adcs/ADCS-001_magnetometer_functional_test/2026-07-11_run-01/
```

## General Rules

- Test templates and procedures belong in `test_definitions/`.
- Completed forms, measurements, images, plots, logs, and notes belong in `test_records/`.
- Each subsystem should maintain its own `test_index.md` file listing the available tests.