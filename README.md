# CNSSAP-High-Performance-Data-Auditor
📌 Project Overview
A custom-built data audit engine developed for the CNSSAP (Caisse Nationale de Sécurité Sociale des Agents Publics de l'État). This tool automates the validation, cleanup, and statistical analysis of social security contribution files for over 1.8 million civil servants. It transforms massive, stagnant Excel files into actionable insights in seconds.
🇨🇩 The Challenge: Legacy Data Bottlenecks
Managing social security for an entire nation involves massive datasets. Before this project, the audit team faced significant hurdles:

The "Excel Wall": Files exceeding 180MB crashed standard spreadsheet software.

Operational Latency: Manual data cleansing and audit procedures took days to complete.

Inconsistency: Human error in finding duplicates or missing entries led to financial reconciliation discrepancies.
🛠 Technical Solution
I replaced traditional spreadsheet-based workflows with a high-performance data pipeline built on Python and Polars.

Why Polars?
Unlike traditional Pandas which is memory-heavy, I selected Polars for its multithreaded execution and lazy evaluation, allowing it to process massive CSV/Excel files with minimal RAM usage.

Backend: Python 3.x

Core Logic: Polars (Data processing engine)

Performance: Optimized for CPU parallelism to handle 1.8M+ rows.

Output: Automated generation of audit reports (PDF/Excel) and interactive summary charts.
Key Features:
Instant Validation: Automated detection of missing data, formatting errors, and duplicate entries.

Statistical Profiling: Real-time generation of cross-tabulations and financial trends per trimester.

High-Speed Aggregation: Aggregates complex contribution data across 1.8M rows in under 2 minutes.

Audit Trail: Every audit session generates a timestamped report, ensuring transparency.
Impact & Results
Performance Benchmark: Reduced processing time from several hours to < 120 seconds.

Efficiency: Eliminated the need for expensive software licenses and hardware upgrades by optimizing the algorithm.

Data Integrity: Significant increase in the detection of invalid entries, ensuring accurate social security reporting for the Congolese State.

Decision Making: CNSSAP executives now have the ability to run on-demand audits between meetings, a feat previously impossible.
Technical Showcase
[!IMPORTANT]

Confidentiality Note: Data displayed in screenshots is anonymized. The core logic is private property of the CNSSAP.
<img width="1916" height="734" alt="Image" src="https://github.com/user-attachments/assets/34a56bbd-b006-4ec3-b80b-827cfc16ad7e" />
<img width="1897" height="868" alt="Image" src="https://github.com/user-attachments/assets/888d2e6c-0d50-49c7-890d-73bd10f9cd8c" />
<img width="1888" height="628" alt="Image" src="https://github.com/user-attachments/assets/566ff0b4-41be-49ea-a175-a05a4db31a4c" />
📂 Repository Structure
/src: The core audit engine and Polars logic.

/benchmarks: Comparison scripts showing the performance gap between traditional methods and the Polars engine.

/docs: Audit methodology and technical documentation.

📫 Contact
To discuss high-performance data engineering for large-scale public institutions:
Alpha Mubay - lucmubay@gmail.com
