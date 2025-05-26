📌 ADHD Diagnosis - Stage 2 (Modelling & Explainability)

Project Overview
----------------
This phase of the project focuses on training, evaluating, and explaining machine learning models 
for predicting ADHD diagnosis using a hybrid dataset combining socio-demographic and functional connectome features.

The models are evaluated based on accuracy, fairness (especially across gender), and explainability in compliance with NHS & GDPR expectations.

Files Included
--------------
📂 ADHD_Stage2/
│-- README.txt                          # This file
│-- stage2.ipynb                        # Final modelling notebook
│-- data.ipynb                          # Preprocessed Stage 1 and feature engineering
│-- 📂 Data/
│   ├── final_hybrid_dataset.csv        # Fully cleaned hybrid dataset
│   ├── train_dataset.csv               # Final training set (after split)
│   ├── test_dataset.csv                # Final test set (after split)
│-- 📂 Reports/
│   ├── SHAP plots                      # Feature explanation plots for LR & MLP
│   ├── confusion_matrices.png          # Visual comparison of model predictions

Models Implemented
------------------
1️⃣ Random Forest (RF)
- Tree-based model with strong performance
- Accuracy: 84.0%, F1 Score: 0.83
- Cross-validated and analyzed using permutation feature importance

2️⃣ Logistic Regression (LR)
- Interpretable baseline model with elasticnet regularization
- Accuracy: 83.0%, F1 Score: 0.83
- SHAP explainability included

3️⃣ MLP Neural Network (SOTA)
- Deep learning model with BatchNorm, Dropout
- Accuracy: 86.1%, F1 Score (ADHD): 0.90
- Highest performer with best gender balance
- Manual 5-fold CV confirms robustness (Mean F1: 0.8038)
- SHAP used for feature explainability

Gender-Based Fairness
----------------------
✔ Gender-specific diagnosis charts included
✔ Fairness table shows significant improvement in ADHD detection among females in MLP
✔ Male: 102 diagnosed | Female: 45 diagnosed

How to Run the Notebook
-----------------------
1️⃣ Environment:
Ensure the following libraries are installed:
pandas, numpy, seaborn, matplotlib, sklearn, shap, tensorflow

2️⃣ Open stage2.ipynb and run all cells in order.

3️⃣ Visual outputs:
- Confusion matrices, classification reports
- SHAP plots and gender distribution visualizations

Conclusion
----------
✔ MLP Neural Network outperformed RF and LR
✔ Bias evaluation confirms gender fairness
✔ SHAP ensures model explainability for NHS deployment
✔ Final model is deployment-ready and aligned with real-world ADHD screening goals
