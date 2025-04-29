# Customer Personality Analysis

This project performs a detailed analysis of customer personality data to help businesses better understand their customers. By analyzing customer behaviors, demographics, and purchasing patterns, businesses can tailor their products and marketing strategies to meet the specific needs of different customer segments.

---

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Key Findings](#key-findings)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [References](#references)

---

## Introduction

Customer Personality Analysis is a detailed analysis of a company’s ideal customers. It helps businesses:
- Understand customer behaviors and preferences.
- Segment customers into meaningful groups.
- Optimize marketing strategies and product offerings.

---

## Dataset

The dataset used in this project is the **Customer Personality Analysis** dataset from Kaggle. It contains customer demographic and purchasing data.

### Key Features:
- **Demographics**: Age, marital status, education, income, etc.
- **Purchasing Behavior**: Amount spent on different product categories.
- **Engagement**: Number of purchases through different channels (web, store, catalog).
- **Campaign Response**: Acceptance of marketing campaigns.

---

## Project Workflow

1. **Exploratory Data Analysis (EDA)**:
   - Understand the dataset structure.
   - Identify missing values and outliers.
   - Visualize data distributions and correlations.

2. **Data Cleaning**:
   - Handle missing values and outliers.
   - Drop irrelevant columns.
   - Map categorical variables to numerical values.

3. **Feature Engineering**:
   - Create new features like `TotalAcceptedCmp` and `Children`.
   - Standardize numerical features for modeling.

4. **Unsupervised Modeling**:
   - Apply **Principal Component Analysis (PCA)** for dimensionality reduction.
   - Perform clustering using:
     - **KMeans**
     - **Gaussian Mixture Model (GMM)**
     - **Agglomerative Clustering**
   - Evaluate clustering performance using silhouette scores.

5. **Customer Segmentation**:
   - Analyze clusters to identify distinct customer groups.
   - Generate actionable insights for marketing strategies.

---

## Key Findings

### Clustering Results:
- **KMeans** achieved the highest silhouette score (0.2489), indicating the best cluster separation.
- Identified 4 customer segments:
  1. **Moderate Earners with Higher Education Presence**
  2. **Lower Income, Without Higher Education**
  3. **High Income, Without Higher Education, Low Children**
  4. **Smallest Group, Low Income**

### Marketing Recommendations:
- **Group 2**: Focus on premium product promotions and loyalty programs.
- **Group 1 & 3**: Offer value deals, discounts, and education-focused campaigns.
- **Group 0**: Use a mixed approach, highlighting variety and convenience.

---

## Technologies Used

- **Python**:
  - Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- **Jupyter Notebook** for interactive data analysis and visualization.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>

2. Install required libraries:
   `pip install -r requirements.txt `
4. Run the Jupyter Notebook:
   `jupyter notebook CustomerPersonalityAnalysis.ipynb`

References
- Customer Personality Analysis Dataset on Kaggle
- Silhouette Score Explanation
