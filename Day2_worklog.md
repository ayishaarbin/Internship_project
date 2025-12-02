# Internship Project – Sentinel: Day 2 Worklog

This file contains my Day 2 progress on the internship project for Python Development. The goal of this project is to build a basic system for log monitoring and anomaly detection.

---

## 📌 Day 1 Progress

- Project folder created  
- Virtual environment (venv) created and activated  
- Verified Python version  
- Created folders: src/, data/, logs/  
- Added documentation files  

*Folder Structure (Day 1)*

Internship_Project_sentinel/ │ ├── venv/ ├── src/ ├── data/ ├── logs/ └── README.md

---

## 📌 Day 2 Progress

*Tasks Completed:*

- Created model training script train_model.py in src/models/  
- Trained *Isolation Forest* model for anomaly detection  
- Saved trained model as log_anomaly_model.pkl in src/models/  
- Created anomaly detection script anomaly_detector.py in src/analytics/  
- Successfully ran anomaly detection on processed_logs.csv  

*Folder Structure (Day 2)*

Internship_Project_sentinel/ │ ├── venv/ ├── src/ │   ├── data/ │   │   └── processed_logs.csv │   ├── models/ │   │   ├── train_model.py │   │   └── log_anomaly_model.pkl │   └── analytics/ │       └── anomaly_detector.py ├── logs/ └── Day2_worklog.md

*Notes:*

- Converted all text columns in logs to numeric using LabelEncoder for Isolation Forest.  
- The anomaly detector reads logs from processed_logs.csv and prints detected anomalies in real-time.  
- PowerShell tip: Run scripts **without the (venv)** part in the command prompt. For example:  
  ```powershell
  python src/analytics/
