# 📊 Mutual Fund Overview & Insights

An end-to-end mutual fund analysis project using **Python, Excel, PostgreSQL concepts, and Power BI** to explore fund performance, evaluate key financial metrics, and identify the top 30 mutual funds using a custom weighted scoring model.

## 🎯 Project Overview

This project analyzes mutual fund data to understand fund performance, compare investment-related metrics, and rank funds based on a structured scoring approach.

The analysis includes data exploration, cleaning, normalization, weighted scoring, ranking, and interactive visualization.

## 🎯 Project Objectives

- Explore and understand mutual fund data.
- Analyze historical returns and fund characteristics.
- Examine expense ratios, risk metrics, and fund age.
- Normalize selected metrics for fair comparison.
- Develop a custom weighted scoring model.
- Identify and rank the top 30 mutual funds.
- Present insights through Excel outputs and a Power BI dashboard.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data analysis and processing |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Scikit-learn | Feature normalization |
| Jupyter Notebook | Exploratory analysis |
| Microsoft Excel | Results and reporting |
| Power BI | Dashboard and visualization |

## 📁 Repository Structure

```text
mutual-fund-overview-insights/
│
├── README.md
├── mutual_fund_analysis.ipynb
│
├── data/
│   └── comprehensive_mutual_funds_data.csv
│
├── output/
│   ├── Top_30_Mutual_Funds.csv
│   └── Top_30_Mutual_Funds.xlsx
│
├── dashboard/
│   └── power_bi.pbix
│
└── requirements.txt
```

*The structure above is the planned organization. Add each file to its corresponding folder when setting up the repository.*

## 🔍 Analysis Workflow

1. **Data Loading:** Import the mutual fund dataset into Python using Pandas.
2. **Exploratory Data Analysis:** Examine dataset structure, data types, missing values, duplicates, and descriptive statistics.
3. **Data Cleaning:** Handle missing values and prepare relevant features for analysis.
4. **Data Visualization:** Explore return distributions and fund characteristics.
5. **Feature Normalization:** Apply Min-Max scaling to selected metrics.
6. **Weighted Scoring:** Calculate a combined score using performance, expense, fund age, and risk-related metrics.
7. **Fund Ranking:** Rank funds and identify the top 30.
8. **Reporting:** Export results and explore insights through Power BI.

## 🧮 Custom Scoring Model

A weighted scoring model was developed to evaluate mutual funds using five components:

| Component | Weight |
|---|---:|
| 3-Year Returns | 40% |
| 1-Year Returns | 25% |
| Lower Expense Ratio | 20% |
| Moderate Fund Age | 10% |
| Lower Risk | 5% |
| **Total** | **100%** |

The model combines normalized metrics to calculate a final score for each eligible fund.

**Scoring formula:**

```python
final_score = (
    0.40 * returns_3yr_norm +
    0.25 * returns_1yr_norm +
    0.20 * low_expense_score +
    0.10 * moderate_age_score +
    0.05 * low_risk_score
)
```

Funds are ranked according to their final weighted scores.

## 📈 Project Outputs

- Top 30 ranked mutual funds in CSV format.
- Top 30 ranked mutual funds in Excel format.
- Scored mutual fund analysis.
- Power BI dashboard (`.pbix`).
- Jupyter Notebook containing the analysis workflow.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/prachimahajan192008/mutual-fund-overview-insights.git
```

### 2. Navigate to the project directory

```bash
cd mutual-fund-overview-insights
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

```bash
jupyter notebook mutual_fund_analysis.ipynb
```

Make sure the original dataset is placed in the `data/` folder and update the notebook's CSV file path accordingly.

## 📌 Key Learnings

- Practical experience in data cleaning and exploratory data analysis.
- Understanding feature normalization and weighted scoring.
- Applying Python to financial dataset analysis.
- Developing data-driven ranking methodologies.
- Creating structured analytical outputs and dashboards.

## ⚠️ Disclaimer

This project is for educational and analytical purposes only. The scoring model is a project-specific methodology and does not represent a recommendation to buy, sell, or invest in any mutual fund. Historical performance does not guarantee future returns.

The original dataset is subject to its source's licensing and redistribution terms. It should only be published if permission allows.

## 👩‍💻 Author

**Prachi Mahajan**

B.Tech Computer Science & Engineering (AI) Student  
Aspiring AI Engineer | Data Analyst

- GitHub: [@prachimahajan192008](https://github.com/prachimahajan192008)
- LinkedIn: [Connect with me](https://www.linkedin.com/in/prachimahajan)

---

⭐ If you find this project interesting, feel free to explore the repository!
