# 📊 Methodology: Global Indicators Visualisation and Analysis

## 1. 📥 Data Collection

### The dataset was sourced from [Kaggle](https://www.kaggle.com/), specifically a [public dataset](https://www.kaggle.com/datasets/michaelmatta0/global-development-indicators-2000-2020) on global development indicators from 2000 to 2020. This dataset includes a wide range of socio-economic, environmental, and governance indicators across countries and regions. 

### I plan to explore the data to understand how these different indicators are interconnected, and later analyse the effect they have on Life Expectancy.

## 2. 🧹 Data Cleaning and Preprocessing

### Initial data preparation was conducted using Power Query in Excel. The following steps were applied:

    Removed Invalid Rows: Filtered out non-country entities (e.g. regions or aggregates) to focus only on actual countries.

    Corrected Country Names: Cleaned country names that included illegal characters or formatting inconsistencies.

    Dropped Columns:

        country_code (no relational table used).

        years_since_century, years_since_2000 and is_pandemic_period (can be calculated if needed).

        governance_quality_index (no variance in values—constant at 0.5).

    Rescaled Percentage Columns: Converted all percentage values (e.g. literacy rate, renewable energy usage) from whole numbers (e.g. 45) to true percentages (e.g. 0.45) for compatibility with Excel's percentage data type.

## 3. 🔍 Exploratory Data Analysis (EDA)

### Preliminary exploration was performed to understand the structure and trends in the data. This included:

    Reviewing summary statistics (mean, median, null counts, etc.) in Power Query.

    Assessing data completeness across years and indicators.

## 4. 📊 Visualisations and Reporting

### Several basic visualisations were created to explore development patterns:
    In Excel I made:
    
        Treemaps for:
            Population by Region (2020)
            Population by Income Group (2020)

        Pivot Tables + Sparklines for:
            Life Expectancy over time (2000–2019) for countries averaging over 50M in population.
            Inflation Rates for the same subset.

        Combo Chart (Column + Line) for:
            UK’s CO₂ emissions per capita (tons) vs Renewable Energy % over time.
    
    I then created a general Power BI dashboard that highlights certain important indicators across the 25 countries that averaged the highest populations in the dataset.

    After that I created three additional Power BI dashboards relating to Health, Environment and Economy indicators. I created a third data table for a 100% stacked area chart that shows CO2 emissions over time for the top 5 emitting countries (2000-2020).

All icons used in the card visuals were downloaded from the copyright free image website [pixabay](https://pixabay.com).

## 5. 📈 Statistical Analysis

### Data sorting and Visualisation

    Data was loaded in and examined using some visualisations that are not easily achievable with other tools.

    Data was separated into training and test sets.

    Non-numerical data was discarded and rows with missing values omitted due to some models not being compatible with NAs.

### Training the models

    Both multiple linear regression and linear regression were performed on each predictor. Polynomial regression was tried on the best performing predictors and lag variables were created for Child Mortality.

    Also based on the simple linear and multiple linear regression a small subset was trained and best subset selection was used to compare and identify the best model for each number of predictors up to 10 at a time.

    GLM (Generalised Linear Model) techniques were tried on the child mortality predictor with cross-validation used to determine the best number of cuts.

    Decision tree, bagged trees and random forest trees were also used.

### Testing our models

    First I performed a t test to determine if the training and test set were similar enough. Then I tested a selection of three models on the data:

    - Linear Regression using Child Mortality
    - Natural Spline also using Child Mortality
    - Bagged Trees


## 6. 🛠 Tools Used

    Microsoft Excel: Core tool for transformation, analysis, and visualization.
    
    Power Query: For data loading, cleaning, and transformation.

    Power BI: Snazzier visualisations that allow you to isolate the more populous countries and understand their key development indicators.

    R / Google Colab: Statistical analysis using the Jupyter Notebook based Google Colab Notebooks site.
    
    Kaggle: Data source.

## 7. ⚠️ Limitations

    The dataset contains missing or interpolated values in some indicators.

    No external validation was performed on the accuracy of reported values.

    Strong likelihood of multicollinearity between Life Expectancy and its strongest predictors.

## 8. 📌 Potential Next Steps

    Contact the data publisher to learn specifics about the data.
    
    Perform PCA (Principal Component Analysis), Ridge Regression or the Lasso on a subset of the data that may include predictors that are suspected of multicollinearity.