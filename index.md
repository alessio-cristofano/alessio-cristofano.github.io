# Alessio Cristofano | Junior Data Engineer

Welcome to my portfolio! I am an aspiring Data Engineer transitioning from a technical background into designing robust, production-grade data pipelines. My core focus is building scalable, cost-aware data architectures using modern tools like Python, Polars, DuckDB, Terraform, and cloud-native storage.

---

## 🚀 Featured Project: IMS Bearing Predictive Maintenance Pipeline

* **Repository:** [GitHub - bearing-predictive-maintenance](https://github.com/alessio-cristofano/bearing-predictive-maintenance)
* **Status:** Phase 1 Complete (Local Lakehouse Foundation & CI/CD Automation)

### Project Overview
An end-to-end Medallion data engineering pipeline designed to ingest, validate, and extract features from high-frequency (20 kHz) IoT sensor telemetry. Built using the benchmark IMS Bearing dataset, this project transforms multi-gigabyte raw ASCII test-to-failure records into highly compressed, queryable analytical Parquet tables.

### Architecture & Tech Stack
* **Language & Layout:** Python 3.11+ using a strict modular `src/` layout.
* **Data Processing:** `Polars` for fast, multithreaded columnar dataframe transformations.
* **Analytical Engine:** `DuckDB` for serverless, zero-copy SQL analytics directly on Parquet files.
* **Orchestration & CLI:** Parameterized interface built with `Click`.
* **CI/CD & Code Quality:** Automated `GitHub Actions` workflow enforcing strict static analysis (`Ruff`) and unit testing (`Pytest`).

### Pipeline Layers
1. **Bronze Layer (Ingestion & Validation):** Parses raw filename timestamps (`YYYY.MM.DD.HH.MM.SS`) and ingests thousands of unheaded ASCII snapshots. Actively enforces strict data contracts (e.g., asserting exactly 20,480 rows per 1-second file) to prevent downstream data corruption.
2. **Silver Layer (Feature Extraction):** Aggregates high-frequency signals into statistical time-domain features (RMS, Kurtosis, Skewness, Peak-to-Peak) to capture mechanical degradation signatures over time.

---

## 🛠️ Core Competencies & Skills

* **Data Engineering:** ETL/ELT Design, Medallion Architecture (Bronze/Silver/Gold), Columnar Storage Formats (Parquet).
* **Languages & Frameworks:** Python, SQL, Polars, DuckDB, Pytest, Ruff.
* **DevOps & Tooling:** Git/GitHub, GitHub Actions (CI/CD), Makefiles, Docker foundations.
* **Cloud & Infrastructure (In Progress):** AWS S3, Infrastructure as Code (Terraform), Dagster Orchestration.

---

## 📫 Connect with Me
* **GitHub:** [@alessio-cristofano](https://github.com/alessio-cristofano)