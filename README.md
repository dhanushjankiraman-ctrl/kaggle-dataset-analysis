# 📊 Kaggle Dataset Analysis

An Exploratory Data Analysis (EDA) project that analyzes Kaggle dataset views, downloads, votes, creation years, and user engagement metrics.

## 📌 Project Overview

This project performs exploratory data analysis on Kaggle dataset information to understand dataset popularity, usage, engagement, and activity over time.

The analysis focuses on:

- Dataset views
- Dataset downloads
- Dataset votes
- Dataset creation years
- Dataset usage categories
- Dataset contributors
- User engagement relationships

## 🎯 Objectives

The main objectives of this project are to:

- Analyze how Kaggle dataset views, downloads, and votes vary over time.
- Identify the years with higher dataset activity.
- Study the relationship between views and downloads.
- Analyze the relationship between downloads and votes.
- Identify highly active dataset contributors.
- Categorize datasets based on their download usage.
- Understand patterns in Kaggle dataset engagement.

## 🔄 Data Processing

The notebook performs the following preprocessing steps:

1. Load the Kaggle dataset using Pandas.
2. Select relevant columns:
   - `CreationDate`
   - `TotalViews`
   - `TotalDownloads`
   - `TotalVotes`
   - `OwnerUserId`
3. Sample 5,000 records for analysis.
4. Check for missing values.
5. Handle missing values using interpolation.
6. Convert `CreationDate` into datetime format.
7. Extract the dataset creation year.

## 📈 Analysis Performed

### Dataset Views

The distribution of dataset views is analyzed using a logarithmic scale to handle large differences in view counts.

### Dataset Downloads

Downloads are analyzed using box plots and logarithmic scaling to identify the distribution and potential outliers.

### Dataset Activity Over Years

The project analyzes:

- Average views per year
- Average downloads per year
- Average votes per year
- Number of datasets created per year

### Views vs Downloads

A log-scale scatter plot is used to study the relationship between dataset views and downloads.

**Key observation:** Datasets with higher views tend to receive more downloads.

### Correlation Analysis

A correlation heatmap is created for:

- `TotalViews`
- `TotalDownloads`
- `TotalVotes`

This helps examine relationships between different engagement metrics.

### Dataset Usage Categories

Datasets are categorized according to their download counts:

- Low Usage
- Medium Usage
- High Usage

The distribution of these categories is visualized using a donut chart.

### Top Dataset Contributors

The project identifies users with the highest number of datasets using `OwnerUserId`.

### Downloads vs Votes

A log-scale scatter plot is used to analyze the relationship between downloads and votes.

### Views Distribution Across Years

A box plot is used to compare the distribution of dataset views across different years.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📊 Visualizations

The project includes:

- Histograms
- Box plots
- Line charts
- Bar charts
- Scatter plots
- Correlation heatmap
- Donut chart

## 📁 Project Structure

```text
kaggle-dataset-analysis/
│
├── kaggle_dataset_analysis.ipynb
├── README.md
└── .gitignore
