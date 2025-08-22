# OEE Anomaly Detection – Live Coding Challenge

Welcome! This challenge evaluates your ability to think critically, design modular software, and deliver a working solution under time constraints. Please read carefully.

## Objective

Build a **config-driven application** that:

1. Generates or ingests OEE (Overall Equipment Effectiveness) data
2. Detects anomalies via a pluggable detection strategy
3. Exports results to one or more configurable destinations

## Timebox

* Approximately **1 hour** to implement a working prototype
* Favor clarity, modularity, and correctness over completeness

## Provided

* `seed_oee_data.csv` (realistic sample for reference or testing)

## Requirements

### 1) Input Sources

Support **two input types**, selectable via CLI flag or configuration:

* `file`: read from a CSV file
* `generated`: produce synthetic OEE data (at least 500 rows, including anomalies)

### 2) Anomaly Detection

Implement **two detection strategies**, selectable via CLI/config:

* `zscore`: a statistical approach
* `rules`: a simple threshold/logic–based approach (define your own sensible thresholds)

### 3) Output Targets

Support **two output targets**:

* `file`: write anomalies to CSV or JSON
* `db`: write anomalies to SQLite (PostgreSQL is a bonus)

### 4) Modularity

* Implement input, detection, and output as **separate modules/components**
* Design so new inputs/outputs/detectors can be added with minimal changes
* Avoid large conditional blocks; prefer a plugin-like structure

### 5) Bonus (optional)

* Externalized, configurable thresholds (e.g., JSON)
* Multiple outputs in a single run (e.g., file + db)
* Basic CLI help

## Evaluation Criteria

* **Architecture & Modularity**: Clear separation of concerns; ease of extensibility
* **Correctness**: Reasonable anomaly detection behavior for both strategies
* **Code Quality**: Readability, structure, and concise documentation/comments
* **Execution**: Usability via CLI or configuration without hardcoding
* **Bonus**: Any optional features implemented well

## Deliverable

* A runnable prototype, with brief instructions (README or inline) on how to execute with different inputs, detectors, and outputs
* Include any schema/assumptions you make

Good luck!

