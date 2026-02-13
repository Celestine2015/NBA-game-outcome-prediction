# NBA-game-outcome-prediction

This work is being prepared for submission as an arXiv preprint

Overview

This repository contains the code, experiments, and analysis for an empirical study investigating feature representation, model robustness, and generalization in supervised machine learning for sports outcome prediction. The project uses multi-season NBA data as a real-world testbed to examine methodological trade-offs across different model classes.

The work was conducted as part of an MSc dissertation in Data Science and is intended to support reproducible research and further methodological exploration.

Research Motivation

Predictive modeling in real-world domains often involves noisy data, temporal drift, and complex feature interactions. While prior work in sports analytics frequently emphasizes predictive accuracy, fewer studies systematically examine how modeling choices affect robustness, interpretability, and generalization across time.

This project aims to address this gap by providing a controlled comparative evaluation of commonly used supervised learning models under consistent experimental settings.

Research Questions

This study focuses on the following research questions:

How does feature representation influence predictive performance and generalization across multiple seasons?

What trade-offs exist between interpretability and performance when comparing linear, ensemble-based, and neural models?

Which performance indicators remain stable predictors across seasons, and which exhibit temporal variability?

How sensitive are predictive models to feature selection and preprocessing choices?

Methods
Feature Engineering

Domain-specific features capturing shooting efficiency, rebounding, turnovers, fouls, and efficiency ratings

Aggregation of player-level metrics to team-level representations

Standardization and normalization applied where appropriate

Models Evaluated

The following supervised learning models were evaluated under consistent experimental protocols:

Logistic Regression (linear baseline)

Random Forest (ensemble-based)

Multilayer Perceptron (neural network)

Model Selection and Evaluation

Recursive Feature Elimination (RFE) for feature selection

Cross-validation for performance estimation

Hyperparameter tuning using GridSearchCV and RandomizedSearchCV

Evaluation metrics: accuracy, precision, recall, F1-score, ROC–AUC

Experimental Design

Experiments were conducted using a reproducible pipeline to ensure fair comparison across models. Training and evaluation were performed on held-out datasets, with additional analysis of model behavior through feature importance and error inspection.

Where applicable, temporal considerations were incorporated to assess generalization across seasons.

Key Findings

Key observations from the study include:

Certain performance indicators (e.g., shooting efficiency and turnovers) consistently contributed to predictive accuracy across seasons

Feature importance varied across models, highlighting trade-offs between complexity and robustness

Model performance was sensitive to feature selection, emphasizing the importance of controlled experimental design

Reproducibility

All experiments are fully reproducible.

Requirements

Python 3.x

NumPy

Pandas

scikit-learn

Matplotlib / Seaborn

Running Experiments

# Cloning this repository
git clone https://github.com/Celestine2015/NBA-game-outcome-prediction.git
cd your-repo-name

# Installing dependencies
pip install -r requirements.txt

# Running the main experiments
python main.py

Ethical Considerations and Limitations

This study uses publicly available data and does not involve personal or sensitive information. Limitations include reliance on historical performance metrics and potential temporal drift across seasons. These limitations are discussed in detail in the accompanying dissertation.

Future Work

Potential extensions of this work include:

Temporal cross-validation and concept drift analysis

Expansion to additional sports or decision-making domains

Investigation of explainability techniques for complex models

Development of more robust feature representations

Contact

For questions or collaboration inquiries, please contact:
Celestine Ifeanyi Ojiaku
celestineojiaku@yahoo.com
