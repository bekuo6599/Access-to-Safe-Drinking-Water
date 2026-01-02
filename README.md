# Access-to-Safe-Drinking-Water
Data preparation and exploratory analysis of global access to drinking water (2020)
# 🌍 Access to Safe Drinking Water

## Data Preparation and Exploratory Analysis (2020)

---

## 📌 Project Overview

Access to safe and affordable drinking water is a key global development indicator. This project explores **global access to drinking water** using country-level data, focusing on how **population size, urbanization, and income group** relate to access across different water service levels.

This repository documents **Part 1** of a two-part integrated data analysis project, with emphasis on:

* Data cleaning and validation
* Feature engineering
* Exploratory data analysis (EDA)
* Aggregation and visualization

The analysis was conducted using **Google Sheets** on a CSV dataset.

---

## 🎯 Project Objectives

* Understand the structure and quality of a real-world global dataset
* Compare dataset population estimates with global benchmarks
* Analyze urban vs rural population distributions
* Explore access to drinking water across service levels
* Investigate differences by income group
* Apply appropriate summary statistics and visualizations

---

## 🛠 Tools & Technologies

* **Google Sheets** – data cleaning, calculations, pivot tables, charts
* **CSV dataset** – global population and water access indicators
* **GitHub** – project documentation and version control

---

## 📊 Dataset Description

The dataset contains **16 features**, including:

### Demographics

* `income_group` – World Bank income classification
* `pop_n` – National population (in thousands)
* `pop_u` – Urban population share (%)

### Water Access Indicators (%)

**National:**

* `_wat_bas_n_`, `_wat_lim_n_`, `_wat_unimp_n_`, `_wat_sur_n_`

**Rural:**

* `_wat_bas_r_`, `_wat_lim_r_`, `_wat_unimp_r_`, `_wat_sur_r_`

**Urban:**

* `_wat_bas_u_`, `_wat_lim_u_`, `_wat_unimp_u_`, `_wat_sur_u_`

---

## 🧹 Data Preparation & Cleaning

* Fixed incorrect CSV imports caused by mixed delimiters (commas and semicolons)
* Validated row integrity using a `value_cnt` feature with `COUNTA()`
* Identified and corrected malformed rows
* Handled missing values represented as `NAN`
* Corrected percentage values exceeding 100% via conditional rounding

---

## 🔧 Feature Engineering

New features created include:

* `pop_u_val` – absolute urban population per country
* `pop_r` – rural population share (100 − pop_u)
* `pop_n (m)` – population size rounded to the nearest million
* Rounded and cleaned water access percentage columns
* Numeric encoding of income groups for ordered analysis

---

## 📈 Exploratory Analysis

### Population Analysis

* Compared dataset population totals with 2020 world population estimates (7.821 billion)
* Calculated urban population totals and shares
* Computed percentage differences between dataset and global benchmarks

### Visualization Techniques

* Line charts and 100% stacked column charts
* Box-and-whisker (candlestick) plots for five-number summaries
* Pivot-table-driven charts grouped by income group

### Statistical Measures

* Mean, median, and mode
* Minimum, maximum
* Quartiles (Q1, Q3)
* Interquartile range (IQR)
* Standard deviation

---

## 🔍 Key Insights (Part 1)

* Dataset population closely aligns with global estimates
* Urbanization increases consistently with income group
* Access to basic water services is generally high, but other service levels show wide variation
* Water access distributions are skewed, not normal
* Income group strongly correlates with water access quality

---

## 🔗 Project Link

(https://docs.google.com/spreadsheets/d/1gMZdPneKTafdLTSTeTsTEyecWG3vwcT4GxuHJ34zlP0/edit?usp=sharing)


---

## 🚀 Next Steps

Part 2 of this project will focus on:

* Deeper comparative analysis
* Population-size-based access trends
* Advanced storytelling and insights

---

## 👤 Author

Dike Philip-Neri Bekuochi
Data Analyst | Environmental & Public Health & Development Enthusiast

📜 License

This project is for educational and portfolio purposes.
