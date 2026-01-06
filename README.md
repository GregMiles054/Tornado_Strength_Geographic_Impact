# Analysis of Tornado Patterns (2004–2024)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Library-Pandas-orange.svg)
![NOAA](https://img.shields.io/badge/Data-NOAA-informational.svg)

## 🌪️ Overview
Welcome to my project! As a weather fanatic, I have always been interested in severe weather. After some thought and consideration, I have decided to answer the main question: **"Is tornado alley shifting eastward?"**

This project explores tornadoes across the United States from 2004 up until 2024. To identify long-term trends while filtering out yearly "noise," the data is polled once per decade: **2004, 2014, and 2024.** We will investigate:
* Which states have the highest tornado frequency.
* Which regions experience the most severe storms.
* Physical characteristics like EF status, path length/width, and time of day/year.



---

## 🎯 Project Goals
The primary objective of this project is to demonstrate a full data science workflow:
1.  **Data Cleaning:** Handling raw meteorological records.
2.  **Transformation:** Standardizing formats across three different decades.
3.  **Aggregation:** Summarizing data by state and intensity.
4.  **Visualization:** Creating maps and charts using Python and `pandas`.

---

## 📂 Data Structure
The data utilized in this project is organized as follows:

* **`data/raw/`**: Original, unmodified CSV files obtained from **NOAA** (The National Oceanic and Atmospheric Administration).
* **`data/cleaned/`**: A processed CSV file used for analysis, containing all three decadal data points combined and standardized.

| Variable | Description |
| :--- | :--- |
| **EF Status** | The Enhanced Fujita scale rating (intensity). |
| **Length/Width** | The physical dimensions of the tornado's path. |
| **Time-Based** | The specific month and time of day of touchdown. |

---

## 🛠️ Project Directory
```text
project_root/
│
├── data/
│   ├── Raw_Tornado_Data             # 2004, 2014, 2024 raw files
│   └── Cleaned_Tornado_Data       # Combined master dataset
│
├── notebooks/
│   ├── Tornado_data_exploration.ipynb
│
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run the Analysis

Follow these steps to set up the environment and replicate the analysis on your local machine.

### 1. Clone the Repository
Open your terminal or command prompt and run:
```bash
git clone https://github.com/GregMiles054/Tornado_alley_evaluation.git
```

### 2. Install dependencies and requirements
Open your terminal and run:
```bash
pip install -r requirements.txt
```

### 3. Run the Data cleaning notebook
Run the Tornado_data_exploration.ipynb file to generate the analysis and the tornado_all_years_cleaned_csv