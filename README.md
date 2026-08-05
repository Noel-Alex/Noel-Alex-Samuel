# House Price Exploratory Data Analysis — Phase 1

This repository contains the Phase 1 exploratory data analysis project for the House Price dataset.

The analysis is implemented in Python using Jupyter Notebook and covers data loading, statistical analysis, missing-value handling, data cleaning, feature transformation, and univariate, bivariate, and multivariate analysis.

## Dataset

The dataset is loaded directly from the following public GitHub URL:

```text
https://raw.githubusercontent.com/salemprakash/EDA/main/Data/house%20price.csv
```

## Phase 1 Requirements Completed

The notebook completes the following tasks:

- Loading the dataset
- Inspecting the dataset structure and data types
- Applying basic statistical analysis
- Identifying and handling missing data
- Removing duplicate and invalid records
- Cleaning numerical, categorical, and date columns
- Performing data transformation and feature engineering
- Univariate analysis with a minimum of three visualizations
- Bivariate analysis with a minimum of three visualizations
- Multivariate analysis with a minimum of three visualizations
- Exporting the cleaned dataset, summary reports, and figures

## Visualizations Included

### Univariate Analysis

1. Distribution of house sale prices
2. Frequency of properties by number of bedrooms
3. Box plot of living area
4. Top cities by number of property sales

### Bivariate Analysis

1. Living area versus sale price
2. Bedroom group versus sale price
3. Median sale price by city
4. Waterfront status versus sale price

### Multivariate Analysis

1. Correlation heatmap of numerical variables
2. Sale price versus living area, condition, and bathrooms
3. Median sale price by bedroom count and property condition

## Data Cleaning

The notebook performs the following cleaning operations:

- Standardizes column names
- Removes unnecessary whitespace
- Converts placeholder values such as `?`, `NA`, and `null` into missing values
- Converts the sale date into a proper datetime format
- Converts numerical columns into appropriate numerical data types
- Removes exact duplicate rows
- Removes rows with missing, zero, or negative sale prices
- Removes records with impossible non-positive property-area values
- Fills missing discrete values using the mode
- Fills missing numerical predictor values using the median
- Fills missing categorical values using the mode or an `Unknown` placeholder

Extreme but potentially valid property values are retained. Selected visualizations use percentile limits only to improve readability.

## Data Transformation

The following derived features are created:

- Sale year
- Sale month
- Sale month name
- Sale quarter
- House age at the time of sale
- Renovation indicator
- Years since renovation
- Price per square foot
- Living-area-to-lot-area ratio
- Basement indicator
- Log-transformed sale price
- Log-transformed lot area
- Bedroom groups
- Price quartile categories

## Repository Structure

```text
.
├── House_Price_EDA_Phase_1.ipynb
├── README.md
└── phase1_outputs/
    ├── house_price_cleaned_transformed.csv
    ├── cleaning_log.csv
    ├── correlation_matrix.csv
    ├── validation_summary.csv
    ├── missing_values_before_cleaning.csv
    ├── missing_values_after_cleaning.csv
    ├── numeric_summary_before_cleaning.csv
    ├── numeric_summary_after_cleaning.csv
    ├── categorical_summary_before_cleaning.csv
    ├── categorical_summary_after_cleaning.csv
    ├── additional_statistics_before_cleaning.csv
    └── figures/
        ├── univariate_01_price_distribution.png
        ├── univariate_02_bedroom_counts.png
        ├── univariate_03_living_area_boxplot.png
        ├── univariate_04_top_cities.png
        ├── bivariate_01_living_area_vs_price.png
        ├── bivariate_02_bedroom_group_vs_price.png
        ├── bivariate_03_city_vs_median_price.png
        ├── bivariate_04_waterfront_vs_price.png
        ├── multivariate_01_correlation_heatmap.png
        ├── multivariate_02_price_area_condition_bathrooms.png
        └── multivariate_03_bedrooms_condition_price.png
```

The `phase1_outputs` directory is created automatically when the notebook is executed.

## Requirements

Install the required Python libraries using:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

Recommended Python version:

```text
Python 3.10 or newer
```

## Running the Notebook Locally

1. Clone or download this repository.
2. Open the repository folder in Jupyter Notebook, JupyterLab, or Visual Studio Code.
3. Open `House_Price_EDA_Phase_1.ipynb`.
4. Select a Python kernel.
5. Run all cells from top to bottom.

Using Jupyter Notebook:

```bash
jupyter notebook
```

Using JupyterLab:

```bash
jupyter lab
```

The dataset is downloaded automatically from the public GitHub URL. If internet access is unavailable, download the CSV and place it beside the notebook using either of these names:

```text
house price.csv
house_price.csv
```

## Running in Google Colab

1. Open Google Colab.
2. Select **File → Open notebook**.
3. Open the **GitHub** tab.
4. Enter the repository URL.
5. Select `House_Price_EDA_Phase_1.ipynb`.
6. Select **Runtime → Run all**.
7. Save the completed notebook back to the same GitHub repository.

## Generated Outputs

After execution, the notebook automatically creates:

- A cleaned and transformed CSV file
- Missing-value reports
- Statistical summary tables
- A cleaning-operation log
- A correlation matrix
- A final validation report
- Eleven visualization files

## Final Validation

The final notebook cell checks that:

- No missing values remain
- No exact duplicate rows remain
- No non-positive sale prices remain
- At least three univariate visualizations are included
- At least three bivariate visualizations are included
- At least three multivariate visualizations are included

## Author

**Name:** Noel Alex Samuel
**Registration Number:** 23BDS0291
**Course:** Exploratory Data Analysis 



