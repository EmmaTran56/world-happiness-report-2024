# World Happiness Report 2024 – Power BI Dashboard

## 1. Project Overview

This project presents an interactive **Power BI dashboard** built from the **World Happiness Report 2024** dataset.

The main goals are to:

- Compare happiness levels across countries and regions.
- Explore key factors ("drivers") that contribute to the overall happiness score (Ladder score).
- Provide an intuitive, visual tool for students, policymakers, and the general public to understand global well-being patterns.

---

## 2. Dataset

- **Source:** World Happiness Report 2024 (https://www.kaggle.com/datasets/jainaru/world-happiness-report-2024-yearly-updated)
- **Scope:** Country-level data on subjective well-being and explanatory variables.

Typical fields used in this project include:

- `Country name`
- `Regional indicator`
- `Ladder score` (overall happiness score)
- `Logged GDP per capita`
- `Social support`
- `Healthy life expectancy`
- `Freedom to make life choices`
- `Generosity` (if provided)
- `Perceptions of corruption`
- `Whisker range`

---
  
## 3. Repository Structure

```text
world-happiness-2024/
│
├─ data/
│   └─ raw/                 # Original data files (CSV/Excel) from Kaggle 
│
├─ powerbi/
│   └─ WorldHappiness2024.pbix    # Main Power BI report file
│
├─ docs/
│   └─ dashboard_screenshots/     # Screenshots of the Power BI report pages
│
├─ README.md
└─ .gitignore
```
---

## 4. Dashboard Pages & Main KPIs

The Power BI report is organised into several pages. Below is an example structure (adapt it to match your implementation):

4.1 Global Overview

- Purpose: Provide a high-level view of global happiness.

- Key KPIs:
Average global Ladder score
Number of countries in the dataset
The happiest country
The least happy country
Average Whisker range

- Main visuals:
Avg Ladder score by region
World map coloured by Ladder score
Top 10 happiest countries (bar chart)
Bottom 10 countries (bar chart)
Global ranking table with search and filters

- Filters / Slicers:
Region

---

## 5. Data Model (Power BI)

-Fact table
  -FactHappiness
    Country name
    Regional indicator
    Ladder score
    Log GDP pẻ capita
    Social support
    Healthy life expectancy
    Freedom to make life choices
    Generosity
    Perceptions of corruption
    Dystopia + residual
    Whisker range
    upperwhisker
    lowerwhisker
    Driver Sum
    Global Rank

---

## 6. How to Run the Project

- Clone this repository:

git clone https://github.com/EmmaTran56/world-happiness-report-2024.git
cd world-happiness-report-2024

- Download the dataset:

Download the World Happiness Report 2024 dataset from Kaggle.
Save the files in the data/raw/ folder.

- Open the Power BI report:

Install Microsoft Power BI Desktop.
Open powerbi/WorldHappiness2024.pbix.
Update data source paths (if needed):
In Power BI, go to Transform data > Data source settings.
Update the file paths to point to your local data/ folder.
Click Refresh to load data.

---

## 7. Tools & Technologies

- Power BI Desktop – Data modelling and interactive visualisation
- Data cleaning and exploratory analysis
- Git & GitHub – Version control and project sharing

---

## 8. Future Improvements

Potential next steps for this project:

- Add more years of World Happiness data to enable time-series analysis.
- Include additional socio-economic indicators (e.g., inequality, education).
- Deploy the report via Power BI Service and share as an interactive web dashboard.
- Build a small API or web app to allow users to query country profiles.

---

## 9. Author

Name: Emma Tran
Institution: Charles Darwin University
Contact: xuanthanh561194@gmail.com
GitHub: @EmmaTran56
