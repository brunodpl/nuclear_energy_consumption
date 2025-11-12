# ⚡ Project: Global Nuclear Energy Demand

<div align="center">

🌍 <b>Analysis of trends and prediction of global nuclear energy consumption</b>

</div>

---

## 👀 Quick Overview

- Analysis of consumption, electricity generation, and the role of the nuclear sector in the energy mix.
- Predictive modeling with ARIMA based on historical data and economic variables.
- Interactive visualizations and summary tables.

---

## 📂 Project Structure

- **owid-energy-data.csv**: Original data.
- **datos_nuclear.csv**: Cleaned data.
- **global_nuclear_energy.ipynb**: Main notebook with analysis and visualizations.
- **EDA_nuclear.ipynb**: Initial exploration and data cleaning.
- **Report.pdf**: Final report with conclusions and graphs.

---

## 🛠️ Tools Used

- **Python**: For data analysis and modeling.
- **Libraries**: Pandas, NumPy, Matplotlib, Statsmodels, Scikit-learn, XGBoost.
- **Jupyter Notebook**: For interactive development.

---

## 📊 Visualizations

- Graphs of nuclear consumption by country.
- Evolution of global nuclear consumption (total vs per capita).
- Correlations between economic variables and nuclear consumption.
- **Top 10 countries**: Identification of countries with the highest absolute and per capita nuclear consumption.
- **Temporal analysis**: Comparison of global and regional trends.

---

## 📈 Key Results

- **Global nuclear consumption**: Increasing trend with regional variations.
- **GDP-nuclear consumption correlation**: Countries with higher GDP tend to consume more nuclear energy.
- **ARIMA prediction**: Consumption projection for the next 5 years.
- **Stationarity**: Time series evaluation for ARIMA modeling.
- **Predictive models**: Comparison between ARIMA and XGBoost for consumption prediction.

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/brunodpl/Data-Analytics.git
   ```
2. Install dependencies:
   ```bash
   conda env create -f environment.yml
   conda activate nuclear_analysis
   ```
3. Open the notebooks in Jupyter:
   ```bash
   jupyter notebook
   ```

---

## 📝 Contributions

If you want to contribute, please open an issue or submit a pull request.

---

## 📧 Contact

- Author: Bruno DPL
- Email: bruno.dpl@example.com
- GitHub: [brunodpl](https://github.com/brunodpl)

---

<div align="center">

💡 <b>"Nuclear energy is key to a sustainable future."</b>

</div>

## 📁 Project File Structure

```
nuclear_energy_consumption/
├── README.md                      # This file
├── LICENSE                        # Project license
├── project-enviroment.yml         # Environment dependencies
│
├── /data                          # Data folder
│   ├── datos_nuclear.csv          # Processed and filtered data (nuclear energy only)
│   └── owid-energy-data.csv       # Original dataset from OWID (Our World in Data)
│
├── /notebooks                     # Analysis notebooks
│   ├── EDA_nuclear.ipynb          # Initial exploration, cleaning, and data preparation
│   └── global_nuclear_energy.ipynb # Main analysis: visualizations, correlations, and predictions
│
├── /docs                          # Documentation
│   └── Report.pdf                 # Final report with conclusions and graphs
│
└── /graphs                        # Generated visualizations
```

**Description of Main Files:**

- **datos_nuclear.csv**: Processed dataset containing only records with nuclear consumption (excluding empty values). Includes columns for `nuclear_consumption`, `nuclear_energy_per_capita`, `gdp`, and `population`.
- **EDA_nuclear.ipynb**: Initial exploration notebook where data cleaning, missing value identification, and descriptive analysis of the original dataset are performed.
- **global_nuclear_energy.ipynb**: Main notebook containing:
  - Analysis of nuclear consumption by country (top 10)
  - Correlation matrix between variables
  - Stationarity tests (ADF test)
  - ACF/PACF analysis for ARIMA parameter identification
  - ARIMA(2,2,1) modeling for time series
  - Nuclear consumption forecast for the next 5 years
  - Model diagnostics validation
