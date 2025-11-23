# Student-stress-tracker
It is a python based student stress tracker which tracks a students stress level by asking various questions related to a students daily life


📚 Student Stress Factors Analysis
Project Overview
This repository contains the code and analysis for exploring the various factors that contribute to stress levels among students. Using a dataset of self-reported student metrics, I performed Exploratory Data Analysis (EDA) to identify key correlations between lifestyle, academic pressure, and mental health indicators with overall stress.

The goal was to gain insights into which variables are the strongest predictors of high stress, providing a data-driven foundation for potential interventions or further modeling.

📊 Key Findings
The correlation analysis revealed several important relationships:

Strong Stress Indicators (Positive Correlation)
The most significant factors correlated with higher stress levels are:

Anxiety and Depression: Unsurprisingly, higher anxiety_level and depression scores showed the strongest positive relationship with stress.

Physical Symptoms: The frequency of headache_freq (suffering headaches) is highly correlated with stress, suggesting stress manifests physically.

Study Load: Higher study_load contributes directly to elevated stress.

Stress Mitigation Factors (Negative Correlation)
Factors that tend to be associated with lower stress levels are:

Sleep Quality: As seen in the scatter plot, a better sleep_quality score has a clear inverse relationship with stress.

Self-Esteem: Higher self_esteem is negatively correlated with stress, indicating it may act as a protective factor.

Extracurriculars: Regular practice of extracurricular_freq shows a modest negative correlation, suggesting these activities help manage stress.

🛠️ Data and Tools
Dataset
Source: Student Stress Factors (2).csv

Observations: The dataset includes various student-reported metrics. Crucially, the data was clean (no missing values were found using df.isnull().sum()), which simplified the initial analysis.

Technologies
Python: The core language for the analysis.

Pandas: Used for data loading, cleaning, manipulation, and renaming messy columns into clear variables like sleep_quality and stress_level.

Matplotlib & Seaborn: Used for data visualization, specifically the Correlation Heatmap and the Sleep Quality vs. Stress Level Scatter Plot.

🚀 How to Run the Analysis
The core analysis was performed in a Google Colab notebook (since the initial code uses from google.colab import files).

Clone the Repository:

Bash

git clone [Your Repository URL]
cd [Your Repository Name]
Open the Notebook: The notebook file (e.g., student_stress_analysis.ipynb) contains all the code.

Upload the Data: Ensure you have the Student Stress Factors (2).csv file. You'll need to run the files.upload() command in Colab to load the data into the environment.

Execute Cells: Run the cells sequentially to perform the data loading, cleaning, descriptive statistics, and visualization steps.

🖼️ Visualizations
The two main visualizations that drove the insights:

1. Correlation Heatmap
This plot shows the linear relationship between all numerical factors. The colors clearly indicate positive (red/warm) and negative (blue/cool) correlations with stress.

2. Sleep Quality vs. Stress Level
This scatter plot visually confirms the inverse relationship: students reporting higher sleep quality tend to report lower stress levels.

