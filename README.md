# DiabetesEquiAI
Final Year Dissertation 2026

## Code description

**DiabetesEquiAI** is a final-year Computer Science project that investigates racial and socioeconomic bias in AI-driven diabetes risk prediction.

The project builds a fairness-aware machine learning pipeline using the NHANES population health dataset. The pipeline trains baseline diabetes prediction models, audits fairness across racial groups, applies bias mitigation techniques, and compares fairness–performance trade-offs.

## Project Aim

To design and evaluate a fairness-aware AI pipeline for diabetes risk prediction that investigates and mitigates demographic bias.

## Code Overview

The project code was developed in Python using Google Colab.

The notebook includes:

- Loading and merging NHANES dataset files
- Cleaning and preprocessing the dataset
- Creating a binary diabetes outcome variable
- Selecting demographic and socioeconomic features
- Training Logistic Regression and Random Forest models
- Evaluating model performance using accuracy, recall and AUC
- Auditing fairness across racial subgroups using recall/TPR and FPR
- Calculating Equal Opportunity and Equalised Odds gaps
- Applying bias mitigation techniques including:
  - class reweighting
  - demographic reweighting
  - group-specific threshold calibration
  - Fairlearn ExponentiatedGradient
- Comparing mitigation results and fairness–utility trade-offs

## Key Findings

- The cleaned NHANES dataset was highly imbalanced, with 92.3% non-diabetic and 7.7% diabetic cases.
- Logistic Regression achieved the strongest clinically useful baseline recall.
- The baseline fairness audit showed an Equal Opportunity Gap of 0.282.
- The lowest recall was observed in the Other/Multiracial group.
- Group-specific threshold calibration gave the best practical fairness–utility balance.
- Fairlearn achieved the strongest fairness improvement, but reduced predictive utility.

## Poster Materials

This repository supports the DiabetesEquiAI final-year project poster and contains the project code, references and supporting materials.

## Full References

Bird, S. et al. (2020) *Fairlearn: A toolkit for assessing and improving fairness in AI*.

Centers for Disease Control and Prevention (2023) *National Health and Nutrition Examination Survey*.

Hardt, M., Price, E. and Srebro, N. (2016) ‘Equality of opportunity in supervised learning’.

He, H. and Garcia, E.A. (2009) ‘Learning from imbalanced data’.

Obermeyer, Z. et al. (2019) ‘Dissecting racial bias in an algorithm used to manage the health of populations’, *Science*.

Pedregosa, F. et al. (2011) ‘Scikit-learn: Machine learning in Python’, *Journal of Machine Learning Research*.

Schaekermann, M. and Horn, I. (2024) *Health Equity Assessment of Machine Learning framework*.
