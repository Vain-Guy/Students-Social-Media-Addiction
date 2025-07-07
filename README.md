# Scroll. Tap. Regret.

### A Data Science Project on Social Media Addiction and Its Impact on Academic Performance

## Overview

Universities today face an invisible epidemic- social media addiction. It’s not just about wasted time; it’s about eroded focus, disrupted sleep, poor mental health, and academic decline. This project explores those connections using real student data and delivers **insights + predictions** that stakeholders can act on.

If you’ve ever wondered how digital behavior shapes academic outcomes, this notebook has the answers — backed by numbers, logic, and a clear call to action.

## Problem Statement

> **Can we predict whether social media negatively impacts a student’s academic performance based on behavioral and demographic data?**

We go beyond basic stats and ask:

* Which behavioral signals are most predictive of academic struggles?
* Is addiction score alone enough to trigger concern?
* Can we model this problem well enough to identify students at risk?
  
## Objectives

* Clean and analyze survey-based student data related to social media habits
* Explore relationships between digital behavior and academic outcomes
* Engineer meaningful features to capture psychological signals
* Build and evaluate a **binary classification model** predicting academic impact
* Visualize insights in a compelling and actionable manner

## Stakeholders

* **Academic Decision-Makers**: Deans, department heads, and student success teams
* **Wellness & Counseling Units**: Prioritizing outreach to digitally overexposed students
* **Policymakers & Researchers**: Exploring tech’s effects on learning
* **EdTech Developers**: Building smarter intervention systems

## Dataset Summary

* **Source**: Student self-reported survey on social media usage, sleep, academic disruption, and stress
* **Features**:

  * **Demographics**: Gender, Age, Country, Relationship Status
  * **Behavioral**: Platforms used, daily usage time, sleep hours, late-night usage
  * **Psychological**: Addiction score (1–10), reported impact on academics

## Data Workflow

### 1. Data Cleaning

* Renamed cryptic column headers for readability
* Standardized categorical encodings (e.g 'Yes/No', 'Male/Female')
* Verified class distributions and checked for missing values

### 2. Exploratory Data Analysis (EDA)

* Addiction scores plotted against academic performance flags
* Gender and platform usage compared visually
* Country-level trends in perceived social media impact explored
* Patterns in sleep hours vs addiction and focus

### 3. Feature Engineering

* Created binary target: **Is student’s academic life affected by social media?**
* Encoded categorical values using label encoding
* Scaled numeric variables for modeling fairness

## 4. Predictive Modeling

Built a **Logistic Regression classifier** to predict whether a student’s academics are negatively affected by social media use.

### Model Performance

* **Accuracy**: 97.7%
* **Precision**: 98.2%
* **Recall**: 98.2%
* **AUC (ROC)**: 0.999
* Evaluated using:

  * Confusion Matrix
  * Classification Report
  * ROC & PR Curves

### Key Predictors

* Addiction score
* Sleep hours
* Daily screen time
* Use of phone during lectures
* Number of platforms used

> In short: If a student scrolls through 4 apps while half-asleep at 3AM, there’s a high chance their GPA is suffering.

## Visualizations

* **Hybrid plots**: Gender vs addiction vs academic impact
* **Heatmaps**: Country vs Platform usage
* **Curve plots**: ROC and Precision-Recall charts
* **Confusion matrix**: Strong balance between positive and negative prediction

## Tech Stack

* Python 3.x
* Jupyter Notebook
* 'pandas', 'numpy'
* 'matplotlib', 'seaborn', 'plotly'
* 'scikit-learn'

## How to Use

1. Clone this repository
2. Open the notebook 'std.ipynb'
3. Install dependencies (optional 'requirements.txt')
4. Run all cells
5. Observe model insights, visualizations, and classification performance

## Future Directions

* Expand dataset with time-series usage or app interaction data
* Deploy model in a dashboard for early intervention triggers
* Extend beyond academic impact to predict mental health decline
* Partner with universities for ethical, privacy-respecting rollout

## License

MIT License- build responsibly, use ethically.

## Final Word

This project isn’t a rant against social media. It’s a **data-driven invitation to intervene earlier, smarter, and with empathy**.
Because sometimes, the most impactful notification a student could receive… isn’t from an app, but from a caring system.

⚠️ **Note**: This analysis does not aim to ban or restrict social media usage but to promote healthy digital habits and support academic success through data-driven decisions.
