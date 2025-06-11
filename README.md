# 🌍 Global Indicators Visualisation and Analysis
## Overview

### The [Global Development Indicators dataset](https://www.kaggle.com/datasets/michaelmatta0/global-development-indicators-2000-2020) is a popular dataset recently released on [Kaggle](https://www.kaggle.com). I created this project to  analyse and visualise key socio-economic and environmental indicators from 2000 to 2020. I use a combination of data cleaning (Power Query), visualisation (Power BI/Excel) and analysis (R in Google Colab Notebooks) to understand the data and see if it can be used to predict Life Expectancy.


## 📊 Key Features

### Data Source: [Global indicators from 2000 to 2020.](data/raw_data.csv)

### Visuals & Metrics:

Interactable Power BI dashboards relating to Health, Environment, Economy and General (pictured below) Indicators.

![General Interactable Dashboard of the Top 25 Countries by Population](images/General_Dashboard.png "General Dashboard of the Top 25 Countries by Population")

PivotTables and PivotCharts of various Indicators as well as spreadsheets for the original and cleaned versions of the dataset.

![PivotTable and PivotChart for Co2 Emissions vs. Renewable Energy by Year](images/Pivot.png "PivotTable and PivotChart for Co2 Emissions vs. Renewable Energy by Year")

Models trained for predicting Life Expectancy using R. 

Visualisations include model fits and their associated statistics. Best Subset Selection pictured below.

![Best Subset Selection for predicting Life Expectancy](images/Best_Subset_Selection.png "Best Subset Selection for predicting Life Expectancy")


### Technologies Used:

![Microsoft Excel](images/Excel_Logo.png "Microsoft Excel")&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Power Query](images/Power_Query_Logo.jpg "Power Query")![Power BI Desktop](images/power_bi_logo.png "Power BI Desktop")![R](images/r_logo.png "R Programming Language") &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Google Colab Notebooks](images/Colab_Logo.png "Google Colab Notebooks")

<pre> ## 📁 Project Structure ``` Global_Indicators/ ├── Analysis_of_Indicators.ipynb # Jupyter Notebook for data exploration and analysis ├── Dashboard.pbix # Power BI interactive dashboard file ├── Global_Development_Indicators_2000_2020.xlsx # Core dataset in Excel format ├── data/ │ └── raw_data.csv # CSV version of the dataset ├── docs/ │ └── methodology.md # Explanation of the methodology behind data processing ├── images/ # Icons for dashboard visuals and readme images ├── LICENSE.txt # Licensing terms ├── README.md # Project description (this file) └── .git/ # Git tracking files ``` </pre>

    

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