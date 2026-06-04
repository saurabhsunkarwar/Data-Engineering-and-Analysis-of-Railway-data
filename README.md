🚂 Multi-Batch Railway Data Engineering & Analytics Pipeline

An end-to-end data processing and business intelligence project that ingests raw, semi-structured nested JSON server logs, cleanses data anomalies using **Python (Pandas)**, and builds analytical reporting models in **Microsoft Power BI**.

---

📂 Repository Architecture & File Ledger
The project processes three distinct data batches through a structured pipeline:
* **Raw Ingestion Layer:** `backend-assignment-sample-01.json`, `-02.json`, `-03.json` (Raw nested railway transaction logs).
* **Data Processing Layer:** `solution.ipynb` (Jupyter notebook containing the Python/Pandas data-wrangling engine).
* **Cleaned Transformation Layer:** `FILE1_C.csv`, `FILE2_C.csv`, `FILE3_C.csv` (Production-ready tabular datasets exported via Pandas).
* **Business Intelligence Layer:** `FILE1_CLEAN.pbix`, `FILE2_CLEAN.pbix`, `FILE3_CLEAN.pbix` (Interactive Power BI data models and dashboard files).

---

🧹 Data Engineering Pipeline (Python & Pandas)
The raw data entered the pipeline as unstructured JSON records. The `solution.ipynb` notebook handles the following core data-wrangling steps:
1. **Schema Flattening:** Normalizing and flattening nested JSON keys into tabular rows and columns.
2. **Data Type Casting:** Converting timestamps and string objects into optimized date-time and numeric parameters.
3. **Anomaly Remediation:** Identifying missing railway station nodes, resolving route duration conflicts, and exporting verified production `.csv` files.

---

📊 Power BI Analytics & Data Modeling
The cleansed CSV datasets were loaded into Power BI to construct stable star-schema data models. The dashboards are designed to surface critical operational metrics:
* **On-Time Performance (OTP):** Tracking train delay variances across scheduled vs. actual arrival dimensions.
* **Volume Traffic Density:** Identifying high-congestion railway corridors and bottleneck stations.
* **Batch Comparison:** Comparing operational efficiency variations across all three system batches.

---

🚀 How to Review the Project
1. **Review Code Execution:** Click on `solution.ipynb` directly in GitHub to read the complete Python data-cleaning pipeline.
2. **Explore Dashboards:** Download any of the `.pbix` files to open them directly inside *Power BI Desktop* and interact with the data models.
