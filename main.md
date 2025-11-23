from google.colab import files
uploaded = files.upload()import pandas as pd

df = pd.read_csv("Student Stress Factors (2).csv")
df.head()
df.info()df = df.rename(columns={
    "kindly rate your sleep quality": "sleep_quality",
    "how many times a week do you suffer headache": "headache_freq",
    "how would you rate your academic performance ": "academic_performance",
    "How would you rate your study load ": "study_load",
    "how many times a week you practice extracurricular activities": "extracurricular_freq",
    "how would you rate your stress levels?": "stress_level"
})
df.isnull().sum()
df.describe()
import seaborn as sns
import matplotlib.pyplot as plt

plt.figure(figsize=(8,6))
sns.heatmap(df.corr(), annot=True, cmap="coolwarm")
plt.title("Correlation between Factors and Stress Level")
plt.show()
import seaborn as sns
import matplotlib.pyplot as plt

plt.figure(figsize=(6,4))
sns.scatterplot(x=df['sleep_quality'], y=df['stress_level'])
plt.title("Sleep Quality vs Stress Level")
plt.show()
df.columns      
df = df.rename(columns={
    "kindly rate your sleep quality": "sleep_quality",
    "how would you rate your stress levels?": "stress_level"
})
sns.scatterplot(x=df['Kindly Rate your Sleep Quality 😴'], y=df['How would you rate your stress levels?'])                                                                                                                                              
