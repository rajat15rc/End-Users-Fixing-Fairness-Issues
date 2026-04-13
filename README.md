# End-Users-Fixing-Fairness-Issues
End-Users-Fixing-Fairness-Issues — Developed a loan-risk prediction and explanation workflow combining XGBoost, causal graph analysis, fairness metrics, and user-interaction analysis to make automated decisions more interpretable for end users

## What this project is about
This project explores a practical question:

**If a machine-learning model is used to support a loan decision, how can that decision be explained in a way that ordinary users can understand and question?**

To study this, I built a loan-risk prediction workflow and then examined how individual decisions could be made more transparent through fairness analysis, confidence scores, causal relationships between variables, and user-facing summaries.

## Why this matters
Automated decision systems can be useful, but they can also feel opaque and difficult to challenge. In high-impact settings such as lending, it is important not only to make predictions, but also to help people understand:

- what the model is predicting,
- which factors appear to matter,
- how similar cases are treated,
- and whether some groups may be treated differently from others.

This repository focuses on that wider problem of **responsible and understandable AI**, not just raw prediction accuracy.

## What the project does
The project uses loan application data to:

1. predict whether an application is likely to be low-risk or high-risk,
2. estimate how confident the model is in each decision,
3. inspect which features influence predictions,
4. explore possible relationships between variables using causal discovery,
5. compare outcomes across groups and feature combinations,
6. analyse user feedback on how people interacted with the explanations.

## Main components
### 1. Predictive modelling
A machine-learning model is trained to classify loan applications into risk categories.

### 2. Decision transparency
For each application, the project looks beyond the final prediction and provides supporting information such as confidence levels and feature-level analysis.

### 3. Fairness analysis
The project examines whether outcomes differ across groups and combinations of applicant characteristics, helping identify patterns that may deserve closer scrutiny.

### 4. Causal structure exploration
A causal discovery step is used to investigate how variables may relate to one another, giving a more structural view than simple correlation alone.

### 5. User feedback analysis
The project also analyses how participants used and responded to the explanatory tools, including which views they inspected most often and how they judged fairness.

## Repository structure
- `Home Credit Default Risk_Everything Else.ipynb`  
  Main modelling, prediction, confidence, and fairness analysis workflow.

- `Home Credit Default Risk_Causal Analysis.ipynb`  
  Causal discovery analysis and graph-based exploration of relationships between variables.

- `Feedback Analysis.ipynb`  
  Analysis of participant interactions and feedback from the user study.

## Methods used
This project includes:
- data preprocessing and missing-value handling,
- feature selection,
- normalisation,
- XGBoost classification,
- confidence scoring,
- fairness analysis,
- feature-combination analysis,
- causal discovery,
- user interaction analysis.

## What a non-technical reader should take away
This is not just a model that predicts loan outcomes. It is a project about making machine-learning decisions **more understandable, more inspectable, and easier to question**.

## Limitations
This repository is best understood as an applied project on interpretable and fairness-aware decision support. Any reported performance or fairness results should be read alongside:
- dataset limitations,
- preprocessing choices,
- sampling choices,
- and the difference between exploratory analysis and real-world deployment.

## Future improvements
Possible next steps include:
- turning the notebooks into a small interactive app,
- adding clearer visual explanations,
- improving documentation for dataset and setup,
- and validating all final metrics in one reproducible pipeline.
