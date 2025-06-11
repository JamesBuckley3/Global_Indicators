# 🌍 Global Indicators Visualisation and Analysis
## Overview

### The [Global Development Indicators dataset](https://www.kaggle.com/datasets/michaelmatta0/global-development-indicators-2000-2020) is a popular dataset recently released on [Kaggle](https://www.kaggle.com). I created this project to analyse and visualise key socio-economic and environmental indicators from 2000 to 2020. I use a combination of data cleaning (Power Query), visualisation (Power BI/Excel) and analysis (R in Google Colab Notebooks) to understand the data and see if it can be used to predict Life Expectancy.


## 📊 Key Features

### Data Source: [Global indicators from 2000 to 2020.](data/raw_data.csv)

### Visuals & Metrics:

Interactable Power BI dashboards relating to Health, Environment, Economy and General (pictured below) Indicators.

![General Interactable Dashboard of the Top 25 Countries by Population](images/general_dashboard.png "General Dashboard of the Top 25 Countries by Population")

PivotTables and PivotCharts of various Indicators as well as spreadsheets for the original and cleaned versions of the dataset.

![PivotTable and PivotChart for Co2 Emissions vs. Renewable Energy by Year](images/pivot.png "PivotTable and PivotChart for Co2 Emissions vs. Renewable Energy by Year")

Models trained for predicting Life Expectancy using R. 

Visualisations include model fits and their associated statistics. Best Subset Selection pictured below.

![Best Subset Selection for predicting Life Expectancy](images/best_subset_selection.png "Best Subset Selection for predicting Life Expectancy")


### Technologies Used:

![Microsoft Excel](images/excel_logo.png "Microsoft Excel")&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Power Query](images/power_query_logo.jpg "Power Query")![Power BI Desktop](images/power_bi_logo.png "Power BI Desktop")![R](images/r_logo.png "R Programming Language") &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Google Colab Notebooks](images/colab_logo.png "Google Colab Notebooks")

## 📁 Project Structure

<pre>
Global_Indicators/
├── Analysis_of_Indicators.ipynb                    # Jupyter Notebook
├── Dashboard.pbix                                  # Power BI dashboard
├── Global_Development_Indicators_2000_2020.xlsx    # Core dataset
├── data/
│ └── raw_data.csv                                  # Raw CSV dataset
├── docs/
│ └── methodology.md                                # Methodology documentation
├── images/                                         # Dashboard visuals
├── LICENSE.txt                                     # License
├── README.md                                       # This file
└── .git/                                           # Git metadata
</pre>
    

## 🔍 How to Use

### Notebook Analysis

    Open and run Analysis_of_Indicators.ipynb in Jupyter Notebooks.

    Observe the data wrangling, exploratory analysis and model fits for predicting Life Expectancy.

### Power BI Dashboard

    Open Dashboard.pbix in Microsoft Power BI Desktop.

    Interact with filters, visuals, and insights.

### Data Files

    Use Global_Development_Indicators_2000_2020.xlsx or raw_data.csv as the source for custom analysis.

## 📘 Documentation

### Please refer to docs/methodology.md for:

    Indicator definitions

    Data processing pipeline

    Visualization logic

## 📄 License

This project is licensed under the terms described in LICENSE.txt.