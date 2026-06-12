# 🎓 Student Placement Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20Matplotlib%20%7C%20Seaborn%20%7C%20Scikit--learn-green?style=flat)
![Dataset](https://img.shields.io/badge/Dataset-44%20Responses-orange?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)
![Academic](https://img.shields.io/badge/Academic-S.Y.%20B.Sc.%20Data%20Science-purple?style=flat)

> A data-driven mini project to identify key factors influencing student placement outcomes using statistical analysis, data visualization, and regression modeling.

---

## 📌 Table of Contents

- [About the Project](#about-the-project)
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Key Findings](#key-findings)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [How to Run](#how-to-run)
- [Team Members](#team-members)
- [References](#references)

---

## 📖 About the Project

Student placement analysis refers to the systematic examination of factors that influence whether a student secures employment after completing their academic program. This project explores a real-world dataset collected from **44 placed students** to identify patterns, correlations, and predictors of placement success.

**Academic Year:** 2025–2026  
**Course:** S.Y. B.Sc. (Data Science) — Semester II  

### 🎯 Objectives
- Understand the distribution and demographics of placed students
- Identify academic and non-academic factors that influence placement
- Visualize key trends and correlations in the data
- Build a regression model to study relationships between variables

---

## ❓ Problem Statement

Despite significant investments in education, many students graduate without securing employment. Institutions often lack clarity on *why* certain students get placed while others do not — leading to ineffective career support and misaligned curricula.

**Key questions this project answers:**
- Does academic performance (CGPA) significantly impact placement outcomes?
- How does prior work experience / internship affect placement probability?
- What stage of the placement process is most challenging for students?
- Do soft skills and personality traits play a role in placement success?
- What preparation method (self-study vs coaching) is more effective?

---

## 📊 Dataset

| Attribute | Details |
|-----------|---------|
| **Source** | Google Form Survey |
| **Total Responses** | 44 placed students |
| **Total Attributes** | 13 |
| **CGPA Range** | 7.0 – 9.6 |

**Data Collection Pipeline:**
```
Google Form → Google Sheets → CSV Export → Python Analysis
```

### 📋 Attributes Collected
| # | Attribute | Description |
|---|-----------|-------------|
| 1 | Full Name | Student respondent name |
| 2 | Academic Year of Placement | Year/semester of placement |
| 3 | CGPA / Percentage | Academic score (7.0–9.6) |
| 4 | Importance of Academic Performance | Student's opinion on academics |
| 5 | Higher Grades = Better Placement? | Yes / No / Maybe |
| 6 | Number of Companies Applied | Total companies applied to |
| 7 | Stage of Difficulty | Aptitude / Technical / HR |
| 8 | Reasons Students Fail | Top reasons for failure |
| 9 | Personality Traits Impact | Yes / No / Maybe |
| 10 | Reasons Students Succeed | Top success factors |
| 11 | Internship / Live Projects | Yes / No |
| 12 | Preparation Method | Self-study / Coaching |
| 13 | Soft Skills Matter | Yes / No |

---

## 🔄 Project Workflow

```
Data Collection (Google Form)
        ↓
Data Preprocessing
  ├── Removing irrelevant columns (Timestamp, Name)
  ├── Handling missing values (mode imputation)
  ├── Standardizing inconsistent formats (CGPA vs %)
  ├── Label Encoding (Yes/No/Maybe → 1/0/2)
  └── Cleaning open-ended text responses
        ↓
Exploratory Data Analysis & Visualization
  ├── Distribution of Student CGPA
  ├── Stages of Most Difficulty
  └── Preferred Preparation Method
        ↓
Correlation & Regression Analysis
  ├── Correlation Matrix (Heatmap)
  └── Linear Regression: CGPA vs Companies Applied
        ↓
Conclusion & Insights
```

---

## 💡 Key Findings

| # | Finding |
|---|---------|
| 📈 | Most placed students had CGPA between **8.5–9.0** |
| 📝 | **Aptitude Test** is the biggest challenge (~19 students struggled here) |
| 📚 | **69.8% of students prefer Self-Study** over coaching |
| 💼 | **82% of placed students** had completed internships or live projects |
| 🗣️ | **Soft skills** were rated as important by every single respondent |
| 🔗 | Higher CGPA students apply to **fewer companies** (more selective) |
| 💪 | **Confidence** was the most frequently mentioned success factor |

---

## 🛠️ Technologies Used

| Tool / Library | Purpose |
|----------------|---------|
| **Python 3.x** | Core programming language |
| **Pandas** | Data loading and manipulation |
| **NumPy** | Numerical computations |
| **Matplotlib** | Data visualization and charts |
| **Seaborn** | Statistical visualizations |
| **Scikit-learn** | Regression analysis and ML |
| **Google Forms** | Data collection |
| **Google Sheets** | Data export to CSV |
| **Python IDLE** | Development environment |

---

## 📁 Project Structure

```
student-placement-analysis/
│
├── 📄 README.md                        # Project documentation
├── 📊 dataset/
│   └── placement_data.csv              # Cleaned dataset (CSV)
│
├── 📓 notebooks/
│   └── placement_analysis.ipynb        # Jupyter Notebook (full analysis)
│
├── 📂 src/
│   ├── preprocessing.py                # Data cleaning & encoding
│   ├── visualization.py                # Charts and plots
│   └── regression.py                   # Correlation & regression model
│
├── 📂 outputs/
│   ├── cgpa_distribution.png           # CGPA histogram
│   ├── difficulty_stages.png           # Bar chart of difficulty stages
│   ├── preparation_method_pie.png      # Pie chart of prep methods
│   ├── correlation_heatmap.png         # Correlation matrix heatmap
│   └── regression_plot.png             # CGPA vs companies scatter plot
│
└── 📄 Mini_Project_Report.docx         # Full project report
```

---

## ▶️ How to Run

### 1. Clone this repository
```bash
git clone https://github.com/YOUR_USERNAME/student-placement-analysis.git
cd student-placement-analysis
```

### 2. Install required libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Run the analysis
```bash
# Option A: Run Jupyter Notebook
jupyter notebook notebooks/placement_analysis.ipynb

# Option B: Run Python script directly
python src/preprocessing.py
python src/visualization.py
python src/regression.py
```

---

## 👥 Team Members

| Name | Roll No |
|------|---------|
| Bijin Varghese | 14 |
| Shubham Fulzalke | 49 |
| Vishnu Chaphe | 65 |

**Course:** S.Y. B.Sc. (Data Science), Semester II  
**Academic Year:** 2025–2026

---

## 📚 References

- [GeeksforGeeks](https://www.geeksforgeeks.org) — Python & Data Science tutorials
- [Python Official Documentation](https://www.python.org) — Language reference
- [Seaborn Documentation](https://seaborn.pydata.org) — Visualization library
- [Scikit-learn Documentation](https://scikit-learn.org) — Machine learning library
- [Pandas Documentation](https://pandas.pydata.org) — Data manipulation library

---

<p align="center">
  Made with ❤️ by Bijin, Shubham & Vishnu &nbsp;|&nbsp; S.Y. B.Sc. Data Science 2025–26
</p>
