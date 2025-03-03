# **Session Analysis**

## **Overview**
This project analyzes user session behavior using data from Open University Learning Analytics (OULAD). The analysis focuses on detecting patterns of engagement, hesitation, rage clicks, task abandonment, dwell time, and user clustering. Additionally, a logistic regression model is applied to predict user dropout.

## **Author**
Bahareh Jozranjbar

## **Key Features**
- **Hesitation Detection**: Identifies pauses between interactions to measure engagement levels.
- **Rage Click Detection**: Captures rapid clicks within short time intervals to detect frustration.
- **Task Abandonment Analysis**: Uses engagement drop-off to determine users who disengage early.
- **Dwell Time Distribution**: Measures the average time spent per session to assess user engagement.
- **User Clustering**: Groups users based on session behavior using k-means clustering.
- **Dropout Prediction**: Implements a logistic regression model to predict user dropout likelihood.

## **Installation**
Ensure that the following R packages are installed before running the analysis:

```r
install.packages(c("ouladFormat", "dplyr", "ggplot2", "ggthemes", 
                   "cluster", "pROC", "factoextra", "tidyr", "forcats"))
```

## Usage
1. Load and Prepare Data
Downloads and loads the OULAD dataset.
Preprocesses session data for analysis.
2. Analyze Session Patterns
Detects user hesitations and rage clicks.
Identifies task abandonment using the lower quartile of last session dates.
Computes dwell time and visualizes engagement levels.
3. User Behavior Clustering
Uses k-means clustering to categorize users based on dwell time patterns.
4. Dropout Prediction
Builds a logistic regression model to predict dropout likelihood.
Uses session metrics as predictors.

## Results
The analysis produces various visualizations including histograms, bar plots, and ROC curves.
Logistic regression and clustering models provide insights into user disengagement patterns.
