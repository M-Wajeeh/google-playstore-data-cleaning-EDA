# Google Playstore EDA & Feature Engineering

A comprehensive data analysis and feature engineering project on the **Google Playstore dataset**, aimed at uncovering patterns, cleaning inconsistencies, and preparing high-quality features for potential machine learning tasks.

---

## Objectives

- Understand the structure and characteristics of apps published on the Google Play Store
- Handle missing values, outliers, and inconsistencies in the dataset
- Perform meaningful **exploratory data analysis (EDA)** to derive insights
- Engineer useful features that can be leveraged in machine learning models
- Visualize key relationships between variables like app category, ratings, installs, and more

---

## Dataset

The dataset used was sourced from publicly available Google Play Store data. It contains the following key attributes:

- `App`: Name of the application
- `Category`: Category the app belongs to (e.g., Games, Productivity)
- `Rating`: User rating of the app (0 to 5)
- `Reviews`: Total number of user reviews
- `Size`: Size of the app
- `Installs`: Number of times the app has been downloaded
- `Type`: Free or Paid
- `Price`: Price of the app (if paid)
- `Content Rating`: Age group the app is suitable for
- `Genres`: Broad genre classification
- `Last Updated`: Date of last update
- `Current Ver`: Current version of the app
- `Android Ver`: Minimum Android version required

---

## Feature Engineering & Cleaning

Key transformations applied:

- Converted `Installs`, `Price`, and `Reviews` to numerical values
- Handled and imputed missing values across multiple columns
- Removed duplicate entries and outliers (e.g., apps with over-inflated ratings or installs)
- Parsed and normalized `Size` column (e.g., converting MB/KB values to float)
- Extracted new features such as:
  - App update recency
  - Price buckets
  - Install bands

---

## Exploratory Data Analysis

The notebook contains a variety of visualizations and insights, including:

- Distribution of app ratings and installs
- Top categories by app count and popularity
- Relationship between app size and rating
- Pricing trends among paid apps
- Review count vs installs (engagement proxy)

---

## Key Insights

- Most apps are free, but paid apps tend to have slightly higher ratings
- Games dominate the Play Store in volume but not necessarily in ratings
- Very few apps have high install counts; most apps remain under 100k installs
- Recent updates are loosely correlated with better ratings, suggesting active maintenance matters

---

## Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---
