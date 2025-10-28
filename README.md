### Customer Shopping Trends Analysis: 
Statistical Hypothesis Testing and Exploratory Data Analysis using Python
   ## Overview
his project explores customer purchase behavior through a real-world dataset to identify whether there is a statistically significant difference between male and female customers’ average purchase amounts.
Using Python, we conduct end-to-end data analysis — from data cleaning and visualization to hypothesis testing using two-sample t-tests and ANOVA (f_oneway).
The analysis provides data-driven insights into customer segmentation, purchase patterns, and behavioral trends, which can help businesses make informed marketing and pricing decisions.
   ## Dataset
- Source: The dataset used in this analysis is available on Kaggle.
- Columns: The dataset includes various columns such as Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount (USD), and more.
   ## Objective
The main objective of this project is to test a real hypothesis derived from customer transaction data:

H₀ (Null Hypothesis): The average purchase amount of males = average purchase amount of females.
H₁ (Alternative Hypothesis): The average purchase amount of males ≠ average purchase amount of females.

By applying inferential statistics, this project helps understand whether gender has a meaningful impact on purchase behavior.

##  Project Workflow
1️) Data Understanding

The dataset includes customer purchase-related attributes such as gender, purchase amount, product category, and more.
The first step involves exploring column data types, checking for null values, and understanding the dataset’s distribution.

2️) Data Cleaning

- Removed or filled missing values

- Standardized categorical data

- Handled duplicates and inconsistent values

- Converted datatypes for analysis compatibility

3️) Exploratory Data Analysis (EDA)

EDA was performed to understand relationships and patterns:

- Visualized purchase distributions by gender

- Identified average and total spending behavior

- Detected outliers and spread using boxplots

- Analyzed variance within gender-based purchase groups

4️) Hypothesis Testing

We used two-sample t-test to compare means between male and female purchase amounts.
To verify consistency across multiple groups, we also performed ANOVA (Analysis of Variance).

Key functions used:

from scipy.stats import ttest_ind, f_oneway

5️) Visualization

Data visualizations were created using Matplotlib and Seaborn to highlight differences between groups and visualize distribution patterns.

## Statistical Analysis
1) Two-Sample t-Test

Used to determine if the mean purchase amounts of two independent groups (male vs female) are significantly different.

2) ANOVA (f_oneway)

Used to test if there are significant differences among the means of multiple groups.

## Statistical Interpretation
Metric	Description
t-statistic	Indicates how far apart the two group means are relative to their variation.
p-value	Represents the probability that the observed difference occurred by random chance.

## Decision Rule:

If p < 0.05, reject H₀ → significant difference exists.

If p ≥ 0.05, fail to reject H₀ → no significant difference detected.

This ensures a data-driven, evidence-based approach to understanding consumer behavior.

## Visual Insights

The following visualizations were created:

- Distribution plots to visualize purchase amounts by gender.

- Boxplots to show variance, spread, and outliers in purchasing patterns.

- Histograms for frequency distribution.

- Mean comparison plots to illustrate group differences.

These visuals help non-technical stakeholders easily interpret patterns and results.

## Libraries & Tools
- import pandas as pd
- import numpy as np
- import matplotlib.pyplot as plt
- import seaborn as sns
- from scipy.stats import ttest_ind, f_oneway
- import scipy.stats as stats

## Results Summary

1) The t-test and ANOVA results provide statistical evidence about gender-based purchasing behavior.

2) Visuals support the statistical conclusions with clear separation or overlap between distributions.

3) The project demonstrates end-to-end analytical capability, from raw data to insight presentation.
