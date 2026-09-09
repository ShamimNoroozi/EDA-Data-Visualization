# EDA-Data-Visualization
Exploratory data analysis, data preprocessing, and data visualization projects using Python
# Water Potability EDA

This project explores a water-quality dataset with 3,276 samples and 10 variables, including pH, hardness, solids, chloramines, sulfate, conductivity, organic carbon, trihalomethanes, turbidity, and potability.

My goal was to better understand the structure of the data, identify data-quality issues, handle missing values, and explore how the different water-quality features relate to each other and to potability.

## What I worked on

In this notebook, I:

- explored the dataset and checked data types, descriptive statistics, and duplicates
- investigated missing values and their patterns using an UpSet plot
- handled the missing values using KNN imputation after feature standardization
- compared feature distributions between potable and non-potable samples
- examined potential outliers using boxplots
- explored relationships between variables using Spearman correlation and scatter plots

## Main findings

Missing values were mainly present in pH, sulfate, and trihalomethanes, with sulfate having the highest amount of missing data. Only 9 samples were missing all three variables.

The potable and non-potable groups showed considerable overlap across most individual features, so no single variable clearly separated the two groups.

The Spearman correlations were also generally weak, with most values close to zero, suggesting that there are no strong relationships between the water-quality features.

The scatter plots also showed several outliers and observations outside the highlighted reference ranges. Some samples labelled as potable had values outside these ranges, suggesting that potability cannot be determined from a simple threshold on one feature alone.

## Tools

Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, and UpSetPlot.

## Notebook

You can view the full analysis here:

[Water Potability EDA Notebook](./Water_Potability_EDA.ipynb)