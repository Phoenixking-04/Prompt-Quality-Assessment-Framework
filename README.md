# Prompt Quality Assessment Framework

> UNT Summer Research Program 2025 | 
> Applied Prompt Engineering Research

## Overview

An ML-based ensemble framework for automated AI prompt 
quality assessment, developed under Prof. Sagnik Ray 
Choudhury at the University of North Texas. Processed 
17,393 real-world prompts from the LMSYS Chatbot Arena 
dataset to derive scientifically validated quality weights.

## Key Results

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

- Dataset: 17,393 prompts from LMSYS Chatbot Arena
- Raters: 3 independent evaluators, 300 prompts each
- Bias Correction: Rank-based normalization
- ML Models: Linear, Ridge, Lasso, Elastic Net, 
  Random Forest, Gradient Boosting, SVR, Neural Network,
  XGBoost, Bayesian Ridge, Decision Tree
- Validation: 70/30 split + 1,000 bootstrap iterations

## Tech Stack

Python | Scikit-learn | PyTorch | Pandas | NumPy | 
SHAP | GPT-4 API | OpenAI

## Enterprise Applications

Designed for: conversational AI assistants, automated 
employee support workflows, LLM output quality control
