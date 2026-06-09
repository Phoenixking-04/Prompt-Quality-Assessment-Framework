# 🧠 Prompt Quality Assessment Framework
> UNT Summer Research Program 2025

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)]()
[![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)]()

## Overview
Scientifically validated ML framework for automated AI prompt quality assessment developed under Prof. Sagnik Ray Choudhury at UNT. Processes 17,393 real-world prompts from the LMSYS Chatbot Arena dataset using an ensemble of 11 ML models.

## 🏆 Results

| Metric | Result |
|--------|--------|
| Automated Scoring Accuracy | 66.7% |
| GPT-4 Validation Accuracy | 77.3% |
| GPT-4 F1 Score | 83.0% |
| GPT-4 Precision | 89.7% |
| Dataset Size | 17,393 prompts |
| ML Models | 11 ensemble methods |
| Bootstrap Stability | ±0.02 (1,000 iterations) |
| Cross-Validation R² | 0.572 |

## Quality Dimensions (Final Weights)

| Dimension | Weight | Rank |
|-----------|--------|------|
| Completeness | 29.5% | 1st |
| Specificity | 24.7% | 2nd |
| Ethical Safety | 17.8% | 3rd |
| Logical Coherence | 17.6% | 4th |
| Clarity | 10.4% | 5th |

## Files
- `prompt-score.ipynb` - Core scoring with GPT-3.5/4
- `SHP.ipynb` - Stanford Human Preferences pipeline
- `SHP_2.ipynb` - SHP deduplication workflow

## 11 ML Models
Linear Regression | Ridge | Lasso | Elastic Net | Random Forest | Gradient Boosting | SVR | Neural Network | XGBoost | Bayesian Ridge | Decision Tree

All 11 converged to R² = 0.572 - validating the bias correction approach.

## How to Run
```bash
git clone https://github.com/Phoenixking-04/Prompt-Quality-Assessment-Framework.git
pip install openai pandas numpy scikit-learn torch datasets matplotlib seaborn tqdm
export OPENAI_API_KEY=your_key_here
jupyter notebook prompt-score.ipynb
```

---
> 🔗 Developer: [Kalyankumar Sandireddy](https://kalyankumar-sandireddy.online)
