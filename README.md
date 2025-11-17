# 💤 Sleep Health & Stress Level Analysis

This repository contains a full data analysis project exploring how sleep-related factors affect stress levels using the **Sleep Health and Lifestyle Dataset** from Kaggle (created by Laksika Tharmalingam).  
The analysis was completed using **Python**, **Pandas**, **Matplotlib**, **Seaborn**, and **Jupyter Notebook**.

---

## 📂 Project Structure
|_ Introduction
|_ Analysis
  |_ Data Collection
  |_ Data Cleaning
  |_ Data Analysis
|_ Describing

---

## 📊 About the Dataset  
The dataset originally contains **374 individuals** and includes the following key features:

| Column | Description |
|--------|-------------|
| `gender` | Male or Female |
| `age` | Age in years |
| `sleep_duration` | Hours of sleep |
| `sleep_quality` | Self-rated sleep quality (1–10) |
| `stress_level` | Stress level (1–10) |
| `sleep_disorder` | Sleep disorder diagnosis or NaN |
| ... | Other lifestyle-related fields |

Notably:
- Only **155 entries** contain valid `sleep_disorder` values  
- **219 entries are missing**, which is expected since many individuals do not have a diagnosed disorder

---

## 🧹 Data Cleaning Steps

### ✔️ Step 1: Column Standardization  
- Converted all column names to **lowercase** and removed spaces  
- Ensured consistency for easier referencing in Python

### ✔️ Step 2: Removing Unnecessary Columns  
- Dropped unrelated or irrelevant fields  
- Focused analysis on:  
  - gender  
  - age  
  - sleep duration  
  - sleep quality  
  - sleep disorder  
  - stress level  

### ✔️ Step 3: Handling Missing Values  
- Inspected missing values in critical columns  
- Kept NaN values in `sleep_disorder` since they represent *no disorder*  
- Ensured the dataset remains accurate and representative

---

## 📈 Visualizations & Insights

The notebook includes multiple charts such as:

### 📌 Stress Level Distribution by Gender  
Stacked bar plots comparing how male and female participants’ stress levels differ across age groups.

### 📌 Relationship Between Sleep Quality & Stress  
Scatter plots and trend analysis to identify negative correlations.

### 📌 Impact of Sleep Disorders  
Comparison between individuals with:
- **Insomnia**,  
- **Sleep Apnea**, and  
- **No disorders (NaN)**  

### 📌 Multi-Category Comparisons  
Combined visuals examining:
- Age categories  
- Sleep duration  
- Stress-level groupings  

These visualizations help highlight trends such as:
- Lower sleep duration generally → higher stress  
- Poor sleep quality strongly correlates with higher stress  
- Sleep disorders significantly influence both sleep quality and stress  

---

## 🛠️ Technologies Used
- **Python 3.12**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## 🚀 How to Run This Project

### 1. Clone the repository:
```bash
git clone https://github.com/SMK-BTW/StressCauses.git
cd StressCauses
