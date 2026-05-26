# Prompt Quality Assessment Framework

> **UNT Summer Research Program 2025** | Applied Prompt Engineering Research
> 
> Advisor: Prof. Sagnik Ray Choudhury | University of North Texas

## Overview

An ML-based ensemble framework for automated AI prompt quality assessment, developed under Prof. Sagnik Ray Choudhury at the University of North Texas. Processed **17,393 real-world prompts** from the LMSYS Chatbot Arena dataset to derive scientifically validated quality dimension weights using an ensemble of 11 machine learning models.

## Key Results

| Metric | Value |
|--------|-------|
| Automated Scoring Accuracy | **66.7%** (exceeds human baseline) |
| R² Score (all 11 models) | **0.572** (identical convergence) |
| GPT-4 Validation Accuracy | **77.3%** |
| GPT-4 F1 Score | **83.0%** |
| GPT-4 Precision | **89.7%** |
| Bootstrap Stability | **±0.02** across 1,000 iterations |

- ✅ 66.7% automated scoring accuracy (exceeding human baseline)
- ✅ 11 ML models all converged to identical R² = 0.572
- ✅ GPT-4 validation: 77.3% accuracy, 83.0% F1 score, 89.7% precision
- ✅ Bootstrap stability: weights within ±0.02 across 1,000 iterations
- ✅ Framework adopted by PhD students for LLM optimization research

## Quality Dimensions (Final Weights)

| Dimension | Weight | Priority |
|-----------|--------|----------|
| Completeness | 29.5% | 1st |
| Specificity | 24.7% | 2nd |
| Ethical Safety | 17.8% | 3rd |
| Logical Coherence | 17.6% | 4th |
| Clarity | 10.4% | 5th |

## Methodology

- **Dataset:** 17,393 prompts from LMSYS Chatbot Arena
- **Raters:** 3 independent evaluators, 300 prompts each
- **Bias Correction:** Rank-based normalization to eliminate rater subjectivity
- **ML Models:** Linear Regression, Ridge, Lasso, Elastic Net, Random Forest, Gradient Boosting, SVR, Neural Network, XGBoost, Bayesian Ridge, Decision Tree
- **Validation:** 70/30 train-test split + 1,000 bootstrap iterations
- **External Validation:** GPT-4 API cross-validation on held-out prompt set

## Tech Stack

```
Python | Scikit-learn | PyTorch | Pandas | NumPy | SHAP | GPT-4 API | OpenAI
```

## Enterprise Applications

Designed for integration with:
- **Conversational AI assistants** — Automated quality gating for LLM prompts
- **Employee support workflows** — HR/ITSM prompt standardization (ServiceNow context)
- **LLM output quality control** — Pre-deployment prompt validation pipelines

## Research Impact

> *"The framework's dimension weights provide a reproducible, bias-corrected standard for evaluating prompt quality at scale — validated against both statistical models and frontier LLMs."*

- Published quality weighting methodology currently in use by UNT PhD students
- Contributes to the emerging field of systematic prompt engineering evaluation

---

> 🔗 **Researcher:** [Kalyankumar Sandireddy](https://kalyankumar-sandireddy.online) | [LinkedIn](https://www.linkedin.com/in/kalyankumar-sandireddy-400681176)
> 
> 📧 kalyandel04@gmail.com | M.S. Computer Science, UNT (Graduating May 2026)
