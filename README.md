# Climate Change Trends Analysis - Week 2 Data Analytics Project

A Python-based data analytics project that analyzes climate change indicators such as temperature, CO2 emissions, sea level rise, precipitation, humidity, and wind speed. The project performs data cleaning, exploratory data analysis, correlation analysis, visualizations, forecasting, pivot table analysis, and exports final reports.

## Project Overview

This project studies climate change trends using a dataset containing 10,000 records across different locations and countries. The analysis focuses on understanding how major climate variables behave over time and how they relate to each other.

The project was prepared as part of **Week 2 - Data Analytics**.

## Repository Contents

```text
Week - 2 .tex        # LaTeX-exported notebook/report containing full analysis code and outputs
output_0_1.png       # Generated visualization output
output_0_2.png       # Generated visualization output
output_0_3.png       # Generated visualization output
output_0_4.png       # Generated visualization output
README.md            # Project documentation
```

## Dataset Description

The analysis uses a climate change dataset with the following columns:

| Column | Description |
|---|---|
| Date | Date/time of the observation |
| Location | Location name |
| Country | Country name |
| Temperature | Temperature value in °C |
| CO2 Emissions | CO2 emissions value |
| Sea Level Rise | Sea level rise measurement in mm |
| Precipitation | Precipitation value in mm |
| Humidity | Humidity percentage |
| Wind Speed | Wind speed in km/h |

Dataset size used in the analysis:

```text
10,000 rows x 9 columns
```

## Objectives

- Import and inspect the climate change dataset.
- Clean the dataset by checking missing values, duplicates, and data types.
- Perform descriptive statistical analysis.
- Analyze yearly climate trends.
- Study relationships between climate variables using correlation analysis.
- Create visualizations for trends, distributions, and relationships.
- Forecast future values for selected climate indicators.
- Generate pivot table summaries.
- Export cleaned data, statistics, plots, and a final report.

## Tools and Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn
- LaTeX

## Main Analysis Steps

### 1. Data Import

The dataset is loaded using Pandas. The project checks the shape, column names, and first few rows of the dataset.

### 2. Data Cleaning

The cleaning process includes:

- Checking missing values
- Checking duplicate rows
- Validating data types
- Converting the `Date` column into datetime format
- Extracting `Year` and `Month`
- Removing duplicates
- Dropping missing records, if any

### 3. Exploratory Data Analysis

The EDA section calculates:

- Mean
- Median
- Standard deviation
- Minimum and maximum values
- Yearly averages
- Top countries by average CO2 emissions

### 4. Correlation Analysis

A correlation matrix is generated for the major numerical climate variables:

- Temperature
- CO2 Emissions
- Sea Level Rise
- Precipitation
- Humidity
- Wind Speed

The analysis identifies whether relationships are weak, moderate, or strong.

### 5. Data Visualization

The project creates multiple visualizations, including:

- Temperature and CO2 trend over time
- Sea level rise trend
- Precipitation vs humidity scatter plot
- Wind speed distribution histogram
- Correlation heatmap
- Box plots for climate variables
- Forecast visualization

### 6. Forecasting

Linear Regression is used to forecast selected climate indicators:

- Temperature
- CO2 Emissions
- Sea Level Rise

Forecast years used:

```text
2015, 2020, 2025
```

### 7. Pivot Table Analysis

The project creates pivot tables for:

- Average climate values by period
- CO2 emissions by country and period
- Growth rates by period

### 8. Exported Results

The original analysis code exports the following files:

```text
climate_change_data_cleaned.csv
summary_statistics.csv
correlation_matrix.csv
yearly_averages.csv
pivot_table_averages.csv
climate_analysis_main.png
correlation_heatmap.png
box_plots.png
climate_forecast.png
climate_analysis_report.txt
```

## Key Findings from the Analysis

- The dataset contains no missing values and no duplicate rows.
- The average temperature is approximately `14.94°C`.
- The average CO2 emissions value is approximately `400.22`.
- The average precipitation is approximately `49.88 mm`.
- The average humidity is approximately `49.77%`.
- The average wind speed is approximately `25.08 km/h`.
- Most correlations between climate variables are weak in the analyzed dataset.
- The Temperature and CO2 Emissions correlation is approximately `-0.003`, indicating a very weak negative relationship in this dataset.

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/climate-change-trends-analysis.git
cd climate-change-trends-analysis
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

For Windows:

```bash
venv\Scripts\activate
```

For macOS/Linux:

```bash
source venv/bin/activate
```

### 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn
```

### 4. Add the Dataset

Place the dataset file in the project folder. The code expects a CSV file similar to:

```text
climate_change_data.csv
```

Update the dataset path in the code if required:

```python
df = pd.read_csv("climate_change_data.csv")
```

### 5. Run the Analysis

If you convert the LaTeX-exported notebook back into a Python script or notebook, run it using:

```bash
python climate_analysis.py
```

Or open the notebook version in Jupyter Notebook:

```bash
jupyter notebook
```

## Recommended Repository Structure

For better GitHub presentation, the project can be organized like this:

```text
climate-change-trends-analysis/
│
├── data/
│   └── climate_change_data.csv
│
├── outputs/
│   ├── output_0_1.png
│   ├── output_0_2.png
│   ├── output_0_3.png
│   └── output_0_4.png
│
├── reports/
│   └── Week - 2 .tex
│
├── climate_analysis.py
├── requirements.txt
└── README.md
```

## Sample Requirements File

Create a `requirements.txt` file with:

```text
pandas
numpy
matplotlib
seaborn
scipy
scikit-learn
jupyter
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

## Project Output Screenshots

The repository includes generated output images:

```text
output_0_1.png
output_0_2.png
output_0_3.png
output_0_4.png
```

These images represent the visual results generated during the analysis.

## Important Note

The uploaded project currently contains a `.tex` file exported from a notebook/report. For a more complete GitHub repository, it is recommended to also include:

- The original `.ipynb` notebook, or
- A clean `.py` Python script, and
- The dataset file or dataset download link.

## Future Improvements

- Add an interactive dashboard using Streamlit or Power BI.
- Add better forecasting models such as ARIMA, Prophet, or Random Forest Regression.
- Include country-wise climate trend comparison.
- Add automated report generation.
- Improve model evaluation for forecasting.
- Add a data source link and dataset documentation.

## Author

**Yatham Tejeswar Reddy**  
Domain: Data Analytics

## License

This project is for educational and academic purposes.
