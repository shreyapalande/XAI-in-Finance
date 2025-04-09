# Bridging Gaps in Explainable AI for Finance: Multi-Stakeholder Analysis

## Overview

This project aims to improve **transparency, trust, and interpretability** in AI-driven credit scoring by applying **explainable AI (XAI)** techniques tailored for diverse stakeholders—**customers, loan officers, and technical teams**. Using the **HELOC dataset**, we explore the effectiveness of multiple XAI methods in making machine learning models more understandable and actionable.

## Objectives

- Apply XAI methods to credit risk prediction models.
- Generate tailored explanations for different stakeholder needs.
- Evaluate the effectiveness of explanations using practical metrics.

## Dataset

**HELOC (Home Equity Line of Credit)** dataset: An anonymized dataset used to assess applicants as "Good" or "Bad" based on credit behavior. Features include credit utilization, trade counts, and repayment history.

## Models Used

- `XGBoost` (XGBClassifier)
- `LightGBM` (LGBMClassifier)

Models were trained on preprocessed data (imputation, normalization, 80-20 split) and evaluated using accuracy and F1-score.

## Explainability Techniques

| Technique    | Purpose                                                                 |
|--------------|-------------------------------------------------------------------------|
| **C-CHVAE**  | Generates actionable counterfactuals to help customers improve creditworthiness |
| **LIME**     | Provides local, model-agnostic explanations for individual predictions  |
| **SHAP**     | Offers global and local feature contributions to predictions           |
| **ProtoDash**| Uses prototype comparisons to support loan officer decision-making     |

## Stakeholder-Focused Explanations

- **Customers**: Get personalized advice via C-CHVAE (e.g., "Increase income by $500").
- **Loan Officers**: Use ProtoDash to compare customer profiles to "Good"/"Bad" prototypes.
- **Technical Teams**: Visualize feature impacts and model behavior using SHAP and LIME.

## Evaluation Metrics

- **Fidelity**: How well explanations reflect the model’s logic.
- **Actionability**: Usefulness of explanations for making changes.
- **Realism**: Plausibility of counterfactual suggestions.
- **Transparency**: Clarity and interpretability of insights.

