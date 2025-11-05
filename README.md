# Temperature Data Processing & Analysis (Microsoft Fabric)

---

## 📌 Project Overview

This project ingests global temperature-change data from a **CSV** into **Microsoft Fabric (Lakehouse)**, cleans and standardizes it with **PySpark**, persists it back as a managed **Spark table**, and runs **SparkSQL** for analysis.

**Goals**

* Ingest raw CSV -> Lakehouse table
* Clean/standardize units, months, and text encodings
* Handle nulls/duplicates
* Save a clean, query‑ready table (`temperature_table`)
* Run exploratory SparkSQL queries (e.g., India’s Oct/Nov 2019 temps, global max 2019)

---

##  Tech Stack

* **Microsoft Fabric** (Lakehouse + Notebooks)
* **Apache Spark / PySpark**
* **SparkSQL**

---

## Data & Table

* **Source**: CSV (imported to Fabric Lakehouse Files)
* **Target table**: `temperature_table`
* **Key columns** (post‑cleaning)

  * `Area_Code` (int), `Area` (string)
  * `Months_Code` (int), `Months` (string)
  * `Element_Code` (int), `Element` (string)
  * `Unit` (string) — standardized to `degree celsius`
  * `Y1961` … `Y2019` (double)

---

## License

[License](LICENSE)

---