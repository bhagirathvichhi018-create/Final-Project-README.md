# COVID-19 Data Analysis and Visualization

## 📌 Project Overview

This project analyzes COVID-19 data to understand the spread and impact of the pandemic across different countries and regions.

The analysis focuses on:

* Confirmed COVID-19 cases
* Deaths
* Recovered cases
* Active cases
* Case Fatality Ratio
* Incident Rate
* Country-wise confirmed cases
* Overall COVID-19 statistics
* Data cleaning and missing-value handling
* Data visualization

The project is developed using **Python, Pandas, NumPy, Matplotlib, Seaborn, and Plotly**.

---

## 📊 Dataset

The dataset contains **4,011 records and 14 columns**.

### Main Columns

| Column              | Description                    |
| ------------------- | ------------------------------ |
| FIPS                | Geographic/FIPS identifier     |
| Admin2              | Administrative area            |
| Province_State      | Province or state              |
| Country_Region      | Country/region name            |
| Last_Update         | Last update timestamp          |
| Lat                 | Latitude                       |
| Long_               | Longitude                      |
| Confirmed           | Confirmed COVID-19 cases       |
| Deaths              | Reported deaths                |
| Recovered           | Recovered cases                |
| Active              | Active cases                   |
| Combined_Key        | Combined geographic identifier |
| Incident_Rate       | COVID-19 incident rate         |
| Case_Fatality_Ratio | Case fatality ratio            |

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** – Data cleaning and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Static data visualization
* **Seaborn** – Statistical visualization
* **Plotly** – Interactive visualization

---

## 🔍 Data Cleaning

The following data-cleaning steps were performed:

1. Loaded the COVID-19 CSV dataset using Pandas.
2. Checked dataset shape and column names.
3. Inspected data types using `df.info()`.
4. Checked missing values using `df.isnull().sum()`.
5. Checked duplicate records.
6. Converted `Last_Update` into datetime format.
7. Filled missing numerical values using the median.
8. Filled missing text/categorical values with `"Unknown"`.
9. Verified that no missing values remained.

Initially, missing values were present in columns such as `FIPS`, `Admin2`, `Province_State`, `Lat`, `Long_`, `Incident_Rate`, and `Case_Fatality_Ratio`.

After cleaning, all analyzed columns contained non-null values.

---

## 📈 Analysis Performed

### 1. Overall COVID-19 Statistics

The project calculated total:

* Confirmed Cases
* Deaths
* Recovered Cases
* Active Cases

Based on the notebook results:

* **Confirmed Cases:** 84,335,814
* **Deaths:** 1,911,317
* **Recovered:** 47,359,111
* **Active Cases:** 37,140,221

---

### 2. Average Case Fatality Ratio

The average Case Fatality Ratio calculated in the analysis was approximately:

**2.22%**

---

### 3. Country-wise Confirmed Cases

Confirmed cases were grouped by country and sorted in descending order.

The top countries in the analyzed dataset include:

| Rank | Country        | Confirmed Cases |
| ---: | -------------- | --------------: |
|    1 | US             |      20,397,401 |
|    2 | India          |      10,305,788 |
|    3 | Brazil         |       7,703,971 |
|    4 | Russia         |       3,153,960 |
|    5 | France         |       2,697,014 |
|    6 | United Kingdom |       2,549,671 |
|    7 | Turkey         |       2,220,855 |
|    8 | Italy          |       2,129,376 |
|    9 | Spain          |       1,928,265 |
|   10 | Germany        |       1,721,839 |

These values come from the country-wise aggregation performed in the notebook.

---

## 📊 Visualizations

The project includes data visualizations for understanding COVID-19 statistics.

### Overall COVID-19 Statistics

A Matplotlib bar chart was created to compare:

* Confirmed
* Deaths
* Recovered
* Active cases

The chart is titled **"Overall COVID-19 Statistics"**.

---

## 💡 Key Insights

* The dataset contains COVID-19 information across multiple countries and regions.
* Confirmed cases are substantially higher than reported deaths.
* A large number of cases were recorded as recovered or active.
* The US had the highest confirmed-case total among the countries shown in the country-wise analysis.
* India ranked second in confirmed cases in this dataset.
* The calculated average Case Fatality Ratio was approximately 2.22%.
* Data preprocessing was important because several geographic and rate-related fields contained missing values.

---

## 📁 Project Structure

```text
COVID19-Data-Analysis/
│
├── COVID19_Analysis.ipynb
├── covid19.csv
├── README.md
└── images/
    └── charts/
```

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Open the project

Open `COVID19_Analysis.ipynb` in:

* Jupyter Notebook
* JupyterLab
* VS Code

### 3. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn plotly
```

### 4. Update the CSV file path

Make sure `covid19.csv` is available and update the path in the notebook if required.

```python
df = pd.read_csv("covid19.csv")
```

### 5. Run the notebook

Run the cells from top to bottom to reproduce the analysis and visualizations.

---

## 🎯 Project Objective

The main objective of this project is to demonstrate practical **Data Analysis and Data Visualization** skills using Python.

This project demonstrates:

* Data loading
* Data cleaning
* Missing-value treatment
* Duplicate checking
* Datetime conversion
* Aggregation using Pandas
* Statistical analysis
* Country-wise analysis
* Data visualization

---

## 👨‍💻 Author

**Bhagirath**

Data Analysis Project using Python

---

## ⭐ Conclusion

This COVID-19 Data Analysis project provides a structured analysis of COVID-19 statistics using Python. It demonstrates the complete basic data-analysis workflow, starting from data loading and cleaning and continuing through statistical analysis and visualization.
# Final-Project-README.md
