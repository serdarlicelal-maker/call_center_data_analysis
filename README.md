# call_center_data_analysis
# 📞 911 Emergency Calls — Exploratory Data Analysis

A data analysis portfolio project exploring patterns in 911 emergency call data using Python. The notebook investigates call frequency, reasons, temporal trends, and geographic distributions.

---

## 📋 Project Overview

This project performs an end-to-end exploratory data analysis (EDA) on a real-world 911 calls dataset. The goal is to uncover meaningful patterns — such as which emergencies are most common, when calls peak, and how call volume varies by day, hour, and month.

---

## 📁 Dataset

- **Source:** `911.csv` (loaded via Google Drive)
- **Key columns used:**
  - `zip` — ZIP code of the emergency
  - `twp` — Township
  - `title` — Emergency call title (used to extract the reason)
  - `timeStamp` — Date and time of the call

---

## 🔧 Technologies Used

| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Pandas | Data loading and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Plotting |
| Seaborn | Statistical visualizations |
| Google Colab | Development environment |

---

## 📊 Analysis Highlights

### 1. Geographic Breakdown
- Top 5 ZIP codes and townships by call volume

### 2. Call Reason Classification
Calls are grouped into three categories extracted from the `title` field:
- 🚑 **EMS** (Emergency Medical Services)
- 🔥 **Fire**
- 🚗 **Traffic**

### 3. Temporal Analysis
- Call distribution by **hour of day**
- Call distribution by **day of week**
- Call distribution by **month**
- Daily call trends overall and broken down by reason

### 4. Heatmaps
- **Day of Week × Hour** — identifies the busiest time slots
- **Day of Week × Month** — reveals seasonal and weekly patterns

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install numpy pandas matplotlib seaborn
```

### Running the Notebook

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. Place the `911.csv` dataset in your working directory (or update the file path in the notebook).

3. Open the notebook:
   ```bash
   jupyter notebook ders14_portfolio.ipynb
   ```

> **Note:** The notebook was originally developed in Google Colab. If running locally, remove the `google.colab` drive mount cell and update the CSV path accordingly.

---

## 📌 Key Findings

- **EMS** calls are the most frequent category, followed by **Traffic** and **Fire**.
- Call volume shows clear **hourly patterns**, with peaks during daytime hours.
- **Friday** tends to have higher traffic-related calls.
- Heatmaps reveal strong time-of-day and day-of-week interaction effects.

---

## 📂 Project Structure

```
📦 project-root
 ┣ 📓 ders14_portfolio.ipynb   # Main analysis notebook
 ┣ 📄 README.md                # Project documentation
 ┗ 📄 911.csv                  # Dataset (not included — add your own)
```

---

## 🙌 Acknowledgements

- Dataset inspired by the [Kaggle 911 Calls dataset](https://www.kaggle.com/datasets/mchirico/montcoalert)
- Project developed as part of a data science portfolio exercise
