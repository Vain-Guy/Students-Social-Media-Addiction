# Scroll. Tap. Regret.

### A Data Science Deep Dive into Social Media Addiction and Academic Fallout

## Overview

Universities today face a quiet crisis: students glued to screens, distracted in lectures, and trading sleep for scrolling.  
But this project goes beyond anecdote—it’s a data-driven diagnosis of **how digital behavior affects academic performance**.

Using real student survey data, we built a complete pipeline- from raw behavior to predictive modeling to behavioral tribe clustering.  
> If you’ve ever asked, “Is Instagram tanking my GPA?”- this notebook gives answers.

## Problem Statement

**Can we predict whether social media negatively impacts a student’s academic performance using behavioral and demographic data?**

We explore:

- What behavioral signals predict academic struggles?
- Is addiction score alone a red flag?
- Can we cluster students by behavior and personalize interventions?

## Objectives

- Clean and prepare raw survey data
- Engineer smart features to capture digital and psychological patterns
- Run **exploratory data analysis** to uncover risk trends
- Build a high-performing **Logistic Regression model**
- Use **clustering (KMeans + PCA + t-SNE)** to uncover behavioral tribes
- Visualize insights and recommend targeted, humane interventions

## Stakeholders

| Group | Why It Matters |
|-------|----------------|
| **University Leaders** | Data to back better digital wellness policies |
| **Counselors & Wellness Units** | Proactively identify and support at-risk students |
| **Researchers & Policymakers** | Fresh insights into tech’s effect on learning |
| **EdTech Builders** | Use behavior signals to trigger meaningful nudges |

## Dataset Summary

- **Source**: Student self-reported survey
- **Key Features**:
  - Demographics: Age, Gender, Country, Relationship Status
  - Behavior: Time spent online, sleep hours, most used platforms
  - Psychological: Addiction score (1–10), conflict due to social media
  - Label: Self-reported academic impact ('Yes/No')

## Data Workflow

### 1. Cleaning & Preparation
- Renamed cryptic columns
- Standardized labels (e.g. ‘Male/Female’, ‘Yes/No’)
- Checked for missing values, class imbalances

### 2. Feature Engineering
- Binary academic impact label
- Social intensity (usage × addiction)
- Mental strain (mental health ÷ sleep hours)
- Binned usage and sleep behavior
- One-hot encoded categorical features

## Exploratory Analysis (EDA)

- Heatmaps of platform use by country
- Addiction scores vs academic impact
- Gender patterns in usage and platform loyalty
- Sleep vs addiction scatter insights
- Multivariable relationship mapping

## Predictive Modeling

Built a **Logistic Regression classifier** to predict if a student’s academic life is affected by social media.

### Model Performance:

- ✅ Accuracy: 97.7%
- 🎯 Precision: 98.2%
- 🔁 Recall: 98.2%
- 📈 AUC Score: 0.999

> Translation: This model knows when someone’s GPA is under digital attack.

## Top Predictors

- Addiction score
- Average daily usage
- Sleep hours
- Conflict due to social media
- Phone use during lectures
- Number of platforms

## Clustering (Unsupervised Learning)

We used **PCA + KMeans + t-SNE** to segment students into **4 behavioral tribes**:

| Tribe | Behavior Snapshot |
|-------|-------------------|
| **Cluster 0** | Balanced scrollers—moderate use, decent sleep |
| **Cluster 1** | Burnouts in progress—high addiction, low sleep, mental strain |
| **Cluster 2** | Mindful minimalists—low usage, high mental health |
| **Cluster 3** | Strained socialites—high usage, low rest, socially overwhelmed |

Each tribe was profiled via radar plots, heatmaps, and platform preferences- fueling **targeted intervention strategies**.

## Visualizations

- ROC & Precision-Recall curves
- Confusion Matrix
- Heatmaps of usage and platform breakdowns
- Behavioral trait radar plots per tribe
- t-SNE cluster scatter visualization (2D)

## Tech Stack

- Python 3.x
- Jupyter Notebook
- 'pandas', 'numpy', 'matplotlib', 'seaborn', 'plotly'
- 'scikit-learn` for modeling and clustering

## How to Use

1. Clone this repo
2. Open the notebook 'std.ipynb'
3. (Optional) Install requirements with 'pip install -r requirements.txt'
4. Run all cells top to bottom
5. Explore the insights and customize for your context

## Future Directions

- Expand data collection (e.g. time-series, screen-on events)
- Build a live dashboard for university wellness teams
- Integrate real-time behavioral flagging systems
- Extend to mental health, productivity, and sleep prediction
- Partner with universities for pilot implementation

## License

MIT License. Use it ethically. Build systems that care.

## Final Word

This project isn’t anti-social media. It’s **pro-awareness**.  
It’s about seeing the warning signs early- when a student’s only crime is checking TikTok at 3 AM on a Tuesday.

> Because the most powerful notifications don’t come from apps…  
> They come from systems that understand, predict, and care.

Let’s build those systems.

