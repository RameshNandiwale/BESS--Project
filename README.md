# BESS-Data Analysis
Battery Energy Storage System (BESS) Fault Detection and Analysis
# 🔋 Battery Energy Storage System (BESS) Fault Detection and Operational Analysis

This repository presents a complete analysis of BESS (Battery Energy Storage System) data using Python. The goal is to detect operational anomalies, monitor system health, and support performance optimization using time-series data and statistical techniques.

---

## 📁 Project Structure

BESS-Project/
├── README.md
├── data/
│ ├── BESS_data_task1.csv
│ └── BESS_data_task2.csv
├── notebooks/
│ └── BESS_Analysis.ipynb

---

##  Project Overview

###  Task 1: Operational Fault Detection
- Data: `BESS_data_task1.csv`
- Insights:
  - Flat SOC (State of Charge) periods during active current flow
  - SBMU current limit violations (especially SBMU5, SBMU7, SBMU11, SBMU12)
  - Imbalance between BMU1 current and total SBMU current
- Techniques:
  - Line plots, difference calculations, and logical masking
  - Seaborn & Matplotlib visualizations for current/SOC trends

###  Task 2: Warning Analysis (SOC & Voltage Deviation)
- Data: `BESS_data_task2.csv`
- Insights:
  - Warning conditions triggered when SOC ≥ 10% and voltage deviation ≥ 50 mV
  - Warnings mostly occurred in 10–30% SOC range
  - Weak correlation between voltage deviation and temperature/current
- Tools:
  - Correlation heatmaps
  - Time-series warning analysis
  - SOC bin plots and per-day warning tracking

---

##  Visualizations

- SOC trend with red markers during flat periods
- SBMU current limit violations plotted against thresholds
- Heatmap of correlation during warning conditions
- Scatter plots of SOC vs voltage deviation
- Time-series of warning activity across days

---

##  Tools & Technologies Used

- Python 3.x
- Jupyter Notebook
- Pandas, NumPy
- Seaborn, Matplotlib

---

##  How to Run This Project

1. Clone the repository
```bash
git clone https://github.com/your-username/BESS-Project.git
cd BESS-Project
2. Install Python dependencies (if needed)
```bash
pip install pandas numpy matplotlib seaborn
3. Launch the notebook
```bash
jupyter notebook notebooks/BESS_Analysis.ipynb
---
## Skills demonstrated

Time-series data analysis

Energy systems diagnostics (SOC, current imbalance, voltage warnings)

Python scripting for data cleaning, feature extraction, and visualization

Statistical analysis and anomaly detection

Clear communication of findings using plots and summaries
