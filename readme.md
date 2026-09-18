# Alessio Cristofano - Python Developer | Data Engineer

I build **Python-based software, data workflows, and engineering applications**, combining software development with numerical computing and data analysis.

My background combines engineering, scientific computing, Python development, databases, APIs, and data processing. I am specializing this experience into modern Data Engineering.

**Focus:** Python · Data Engineering · SQL · Data Processing · Scientific Computing · CI/CD

[GitHub](https://github.com/alessio-cristofano) · [LinkedIn](https://linkedin.com/in/alessiocristofano)


---

## Featured Project: Bearing Predictive Maintenance Pipeline

* **Repository:** [GitHub - bearing-predictive-maintenance](https://github.com/alessio-cristofano/bearing-predictive-maintenance)

### Project Overview
An end-to-end Medallion data engineering pipeline designed to ingest, validate, and extract features from high-frequency (20 kHz) IoT sensor telemetry. Built using the benchmark IMS Bearing dataset, this project transforms multi-gigabyte raw ASCII test-to-failure records into highly compressed, queryable analytical Parquet tables.
The IMS dataset contains three test-to-failure experiments. The source documentation specifies 20 kHz sampling and 20,480 points per one-second vibration snapshot, with different channel configurations across the three datasets.

### Why?

During my experience as an engineer in R&D environments, I repeatedly encountered the same challenge: engineering data is often produced by different teams, stored in different formats, and distributed across different systems. Mechanical/aerospace engineers may have a deep understanding of the physical phenomena behind the data, while software and IT teams provide the infrastructure to process it, but the connection between these worlds is not always straightforward.

As a result, companies can accumulate large amounts of valuable data without having an efficient way to integrate it, process it, and turn it into actionable information.

This observation, together with inspiration from a recent visit to the LMSD research department at KU Leuven, led me to explore this problem through a concrete engineering case: **predictive maintenance of mechanical bearings**.

Bearings are relatively simple and widespread mechanical components, but their failure can have significant consequences. They also generate rich vibration data that provides an interesting opportunity to combine engineering knowledge, Python, data processing, and Data Engineering.

This project is therefore an experiment in **merging engineering data and software engineering** to build a reliable pipeline that transforms raw sensor measurements into structured and useful information.


### Architecture & Tech Stack
* **Language & Layout:** Python 3.11+ using a strict modular `src/` layout.
* **Data Processing:** `Polars` for fast, multithreaded columnar dataframe transformations.
* **Analytical Engine:** `DuckDB` for serverless, zero-copy SQL analytics directly on Parquet files.
* **Orchestration & CLI:** Parameterized interface built with `Click`.
* **CI/CD & Code Quality:** Automated `GitHub Actions` workflow enforcing strict static analysis (`Ruff`) and unit testing (`Pytest`).

### Pipeline Layers
1. **Bronze Layer (Ingestion & Validation):** Parses raw filename timestamps and ingests thousands of unheaded ASCII snapshots. Actively enforces strict data contracts (e.g., asserting exactly 20480 rows per 1-second file) to prevent downstream data corruption.
2. **Silver Layer (Feature Extraction):** Aggregates high-frequency signals into statistical time-domain features (RMS, Kurtosis, Peak-to-Peak) to capture mechanical degradation signatures over time.

---

## About Me
### Engineering Background

My engineering background gives me experience working with computational and technical systems. I am building on that foundation with modern Python and Data Engineering practices.

Rather than treating Data Engineering as a separate career from engineering, I focus on applying software engineering discipline to real data problems: correctness, reproducibility, performance, maintainability, and reliability.


### Core Competencies & Skills

* **Data Engineering:** ETL/ELT Design, Medallion Architecture (Bronze/Silver/Gold), Columnar Storage Formats (Parquet).
* **Languages & Frameworks:** Python, SQL, PostgreSQL, Polars, DuckDB, Pytest, TypeScript, Vue, Fortran.
* **DevOps & Tooling:** Git/GitHub, GitHub Actions (CI/CD), Makefiles, Docker foundations.

---

## 📫 Connect with Me
I am interested in opportunities involving **Python development, Data Engineering, data platforms, backend systems, and engineering software**.
* **Github**: [@alessio-cristofano](https://github.com/alessio-cristofano)
* **LinkedIn**: [Alessio Cristofano](https://linkedin.com/in/alessiocristofano)