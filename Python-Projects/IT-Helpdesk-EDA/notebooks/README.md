# 📉 IT Helpdesk Operations Analysis (Lean Six Sigma Approach)

### Project Overview
This project applies **Data Analytics** and **Lean Six Sigma** methodologies to analyze 2,400+ IT helpdesk tickets from the Leena AI system (2025). 

The primary goal is to identify operational bottlenecks, quantify "waste" (Muda) in support processes, and provide data-driven recommendations to reduce Ticket Volume and Resolution Time (MTTR).

### 🎯 Key Business Questions
1. **Pareto Analysis:** What are the top 20% of issues causing 80% of the support volume?
2. **Operational Efficiency:** Are there specific regions or times of day where performance lags?
3. **Root Cause Identification:** Differentiating between "automatable" IT tasks vs. complex software defects.

### 🛠️ Tech Stack & Methodology
* **Python:** Pandas (Data Cleaning), NumPy (Vectorization).
* **Visualization:** Matplotlib & Seaborn (Heatmaps, Pareto Charts).
* **Methodology:** Lean Six Sigma (DMAIC Framework).
* **Environment:** Jupyter Notebook.

### 📊 Executive Summary & Insights
Analysis of the dataset revealed that the **Top 5 Sub-Issues** account for a significant portion of total volume. These were categorized for strategic action:

#### 1. Identity & Access Management (IAM) High Volume
* **Issues:** *Login Failure, Password/Unlock, Account Provisioning.*
* **Insight:** These represent repetitive, administrative tasks.
* **Recommendation:** Implement Self-Service Password Reset (SSPR) and automated provisioning scripts to reduce Level 1 support load.

#### 2. Operational Software Gaps
* **Issues:** *Roster/Manifest, Geofence/Map Data.*
* **Insight:** These are domain-specific errors affecting field operations (Transportation/Logistics). High frequency suggests a disconnect between the software planning and field execution.
* **Recommendation:** Prioritize "Map Data" integrity fixes in the Engineering backlog to prevent downstream support tickets.

### 📈 Visualizations Included
* **Pareto Chart:** Visualizing the "Vital Few" sub-issues vs. the "Trivial Many."
* **Correlation Heatmap:** analyzing the relationship between `Region` and `Issue Type` to spot localized anomalies.
* **Resolution Time Distribution:** Histogram analysis to detect outliers in SLA compliance.

### 🚀 How to Run
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install pandas seaborn matplotlib openpyxl
