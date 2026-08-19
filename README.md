# Algorithmic Empathy: Aligning Explainable NLP with Psycholinguistic Theory
**Author:** Can Li

## Project Overview
This repository contains the data and reproducible code for the research project *"Algorithmic Empathy"*. The project addresses the "Black Box" problem in Artificial Intelligence for mental healthcare by evaluating the construct validity of NLP models. 

This project uses Explainable AI (SHAP) to extract the decision-making weights of machine learning models and quantitatively aligns them with established psycholinguistic markers (LIWC).

## Repository Structure
- `stress.csv`: The raw dataset containing Reddit posts (labeled 0 for Non-Stress, 1 for Stress)
- `Algorithmic_Empathy_Analysis.ipynb`: Colab notebook containing the complete workflow
- `README.md`: Project documentation and reproduction instructions


## Key Workflow Steps
1. *Data Preprocessing:* Noise reduction (URLs, punctuation removal) and psycholinguistic feature engineering
2. *Exploratory Data Analysis (EDA):** Visualizing class balance and text length distributions
3. *Modeling:** TF-IDF vectorization followed by Logistic Regression and Random Forest classification
4. *Explainability (SHAP):** Extracting global feature importance to verify if the model relies on meaningful psychological cues

## Preliminary Findings
The SHAP analysis successfully proved that the Logistic Regression model organically learned to identify stress using clinical psycholinguistic markers. The top features driving the model's predictions were first-person singular pronouns (e.g., *"me", "my", "I'm"*), empirically aligning machine logic with human psychological theory.


## Open Notebook in Google Colab
Click the badge below to automatically open, run, and view the visualizations in Google Colab:

<table align="left">
  <td>
    <a href="https://colab.research.google.com/github/ojos168/Algorithmic_Empathy/blob/main/Stress_Prediction_EDA_and_Baseline_Model.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
  </td>
</table>
<br><br>
