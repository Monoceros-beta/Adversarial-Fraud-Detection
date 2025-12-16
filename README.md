# Adversarial-Fraud-Detection
Quantifying Model Vulnerability to Data Poisoning in Financial Fraud Detection: Threshold Collapse and Feature Sensitivity

**Current Status:** This repository is under active development. The README and code structure are being iteratively refined to include full experimental details.

## Adversarial Robustness Evaluation Framework for Financial Fraud Detection

### Abstract
This research investigates the vulnerability of AI-based financial fraud detection models to data poisoning attacks. The primary objectives are to identify:
1. The **poisoning threshold** at which supervised models (e.g., XGBoost, RF) fail.
2. **Feature-level sensitivities** exploited by adversarial attackers (via SHAP analysis).
3. Lightweight **sanitization strategies** (e.g., Isolation Forest) for detecting and mitigating poisoned data in high-stakes financial environments.

### Repository Structure & Status
This repository is organized into modular notebooks.

| File | Status | Description |
|------|--------|-------------|
| **`01_data_preparation_baseline.ipynb`** | **Completed** | Includes data cleaning pipeline, feature engineering, and baseline training for XGBoost, Random Forest, and Isolation Forest. |
| **`02_adversarial_evaluation_preliminary.ipynb`** | **In Progress** | Preliminary implementation of Label Flipping attacks. **Runs successfully.** Extending the module to include full Feature Manipulation experiments and extensive SHAP visualizations. |

### Key Findings (Preliminary)
Based on initial experiments:
- **Performance Collapse Threshold:** Identified a critical failure point at **30% label pollution**.
- **Model Vulnerability:** XGBoost demonstrated high sensitivity to label noise, with AUC dropping from **0.97** to **0.55**.

### Tech Stack
- **Languages:** Python
- **Libraries:** Scikit-learn, XGBoost, SHAP, Pandas, NumPy
