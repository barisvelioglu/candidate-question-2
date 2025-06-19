# 🏭 OEE Anomaly Detection – Developer Challenge

Welcome! This challenge is designed to evaluate your ability to think critically, structure flexible applications, and use modern tools (including AI) effectively.

## 🎯 Objective

Build a modular and configurable application that:
1. Reads or generates OEE (Overall Equipment Effectiveness) data
2. Detects anomalies in the data
3. Outputs results to a destination based on configuration

---

## ⏱ Time Guidelines
- **1 hour** for implementation
- **30 minutes** for code review and discussion

---

## 📂 Provided
- `seed_oee_data.csv`: Small real-world sample for reference or expansion

---

## 🔧 Requirements

### 1. Synthetic Data Generation
- You must generate at least 100–500 rows of realistic OEE data.
- Include some anomalies (e.g., very low OEE caused by performance/availability/quality issues).

### 2. Configurable Input Source
Via config file or CLI flag:
- `file`: read from a CSV file
- `generated`: generate synthetic data

> Bonus: `db` (read from SQLite/PostgreSQL)

### 3. Anomaly Detection
- Use any approach: Z-score, IQR, logic rules, etc.
- Flag anomalies in the dataset

### 4. Configurable Output Target
Via config file or CLI flag:
- `file`: write results to a CSV or JSON
- `db`: write to SQLite or PostgreSQL

> Bonus: Add new output modules (e.g., Kafka, REST API)

---
