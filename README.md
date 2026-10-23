# Jet Airline Safety Data Analysis

> **Project Goal:** To analyze aviation accident data and provide actionable recommendations to an aviation insurer regarding the safest commercial and passenger jet aircraft makes and models.

## Table of Contents
* [Business Understanding](#business-understanding)
* [Data Overview](#data-overview)
* [Methodology](#methodology)
* [Key Findings & Visualizations](#key-findings--visualizations)
* [Conclusions & Recommendations](#conclusions--recommendations)
* [Repository Structure](#repository-structure)

## Business Understanding
We have been tasked by a prominent airline/airplane insurer to conduct a comprehensive analysis of commercial and passenger jet airline safety. The client's primary objective is to identify which types of aircraft exhibit the lowest rates of total destruction and the lowest likelihood of fatal or serious passenger injuries in the event of an accident.

Additionally, the client is interested in understanding general variables and conditions that contribute to aviation accidents.

### Key Project Parameters

| Parameter | Constraint | 
| :--- | :--- | 
| **Timeframe** | Data analysis is restricted to aircraft from **1983 onwards** (assuming a 40-year maximum lifetime for aircraft retirement). | 
| **Aircraft Type** | Analysis is limited to active, **professionally built** aircraft only. | 
| **Scope** | Provide separate recommendations for **small aircraft** versus **larger passenger models**. | 
| **Statistical Rigor** | Claims and comparisons between groups must be statistically robust and backed by adequate sample sizes. | 

## Data Overview
The analysis utilizes aviation accident data initially spanning from 1948 to 2023. 

* **Data Cleaning:** Raw data was cleaned and filtered to include only professional builds from 1983-2023. Missing values were handled systematically, and relevant columns were transformed to create accurate safety measures.
* **Prepared Dataset:** The cleaned dataset is exported and used as the foundation for the exploratory data analysis phase.

## Methodology
The project is divided into two main phases, documented across two Jupyter Notebooks:

### 1. Data Cleaning (`Aviation_Accident_Cleaning.ipynb`)
* Loaded and inspected the raw dataset using Pandas.
* Cleaned the data by filtering for the post-1983 timeframe and removing amateur builds.
* Exported the cleaned, analysis-ready dataset to a `.csv` file.

### 2. Exploratory Data Analysis (`Aviation_Accident_Data_Analysis.ipynb`)
* Conducted Exploratory Data Analysis (EDA) using statistical summary methods and the split-apply-combine paradigm (`groupby`).
* Utilized Seaborn and Matplotlib for statistical visualizations to identify trends in passenger injuries and aircraft damage.
* Evaluated external factors and conditions contributing to airplane safety outcomes.

## Key Findings & Visualizations

> **Note to Reviewer/Student:** *Replace the placeholder text and image links below with your actual analysis summaries and exported charts.*

### 1. Safest Small Aircraft
**Summary:**
[Insert a 2-3 sentence summary of your findings regarding the safety records of specific small aircraft makes/models.]

**Visual Evidence:**
*(Insert visualization here)*

### 2. Safest Large Passenger Models
**Summary:**
[Insert a 2-3 sentence summary of your findings regarding the safety records of specific large passenger aircraft makes/models.]

**Visual Evidence:**
*(Insert visualization here)*

### 3. Factors Influencing Airplane Safety
* **Factor 1 ([Insert Factor Name]):** [Briefly discuss how this factor relates to serious injuries or airplane damage based on your EDA.]
* **Factor 2 ([Insert Factor Name]):** [Briefly discuss how this factor relates to serious injuries or airplane damage based on your EDA.]

**Visual Evidence:**
*(Insert visualization here)*

## Conclusions & Recommendations
Based on the data analysis, we recommend the insurer consider the following for favorable risk profiles:

* **Small Aircraft Recommendations:**
  * [Make/Model 1]
  * [Make/Model 2]

* **Large Aircraft Recommendations:**
  * [Make/Model 1]
  * [Make/Model 2]

* **Risk Factors to Monitor:**
  * [Condition/Variable 1]
  * [Condition/Variable 2]

## Repository Structure

```text
├── data/
│   ├── raw_aviation_data.csv             # Original dataset 
│   └── cleaned_aviation_data.csv         # Cleaned dataset exported from Part 1
├── images/
│   └── [your_visualizations.png]         # Exported charts used in this README
├── Aviation_Accident_Cleaning.ipynb      # Phase 1: Data cleaning process
├── Aviation_Accident_Data_Analysis.ipynb # Phase 2: EDA and statistical modeling
└── README.md                             # Project presentation and summary
```