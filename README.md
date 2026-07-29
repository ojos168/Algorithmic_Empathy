# Algorithmic Empathy: Aligning Explainable NLP with Psycholinguistic Theory

**Author:** Can Li
**Advisor:** Dr. Christian E. Lopez Bencosme

## Project Overview
This repository contains the data and reproducible code for the research project *"Algorithmic Empathy"*. The project addresses the "Black Box" problem in Artificial Intelligence for mental healthcare by evaluating the construct validity of NLP models. 

Instead of relying solely on predictive accuracy, this project uses Explainable AI (SHAP) to extract the decision-making weights of machine learning models and quantitatively aligns them with established psycholinguistic markers (e.g., the LIWC framework).

## Repository Structure
- `stress.csv`: The raw dataset containing Reddit posts (labeled 0 for Non-Stress, 1 for Stress).
- `Algorithmic_Empathy_Analysis.ipynb`: The primary Jupyter/Colab notebook containing the complete reproducible workflow, from data loading to SHAP interpretation.
- `README.md`: Project documentation and reproduction instructions.

## How to Reproduce the Results
To run the code and reproduce the findings of this study, you do not need to download the data locally. The notebook is designed to be fully executable in the cloud.

1. Open `Algorithmic_Empathy_Analysis.ipynb` directly in **Google Colab**.
2. Run the notebook sequentially from top to bottom.
3. **Data Loading:** The script automatically fetches the `stress.csv` file directly from this GitHub repository. 
4. **Dependencies:** The only external library required that is not pre-installed in Colab is `shap`. The notebook contains the command `!pip install shap` in the relevant section to install it automatically.

## Key Workflow Steps
1. **Data Preprocessing:** Noise reduction (URLs, punctuation removal) and psycholinguistic feature engineering.
2. **Exploratory Data Analysis (EDA):** Visualizing class balance and text length distributions.
3. **Modeling:** TF-IDF vectorization followed by Logistic Regression and Random Forest classification.
4. **Explainability (SHAP):** Extracting global feature importance to verify if the model relies on meaningful psychological cues (e.g., elevated first-person pronoun usage).

## Preliminary Findings
The SHAP analysis successfully proved that the Logistic Regression model organically learned to identify stress using clinical psycholinguistic markers. The top features driving the model's predictions were overwhelmingly first-person singular pronouns (e.g., *"me", "my", "I'm"*), empirically aligning machine logic with human psychological theory.
