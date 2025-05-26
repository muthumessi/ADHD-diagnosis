🧠 ADHD Diagnosis using fMRI and Socio-Emotional Data
Supporting early and fair ADHD detection with explainable AI
📌 Overview
This project was developed as part of my MSc Computer Science coursework at the University of Essex. The goal is to build an explainable machine learning system to assist in diagnosing ADHD in adolescents using functional MRI brain imaging, socio-demographic, emotional, and parenting data.

The challenge was not just to build accurate models, but to detect gender bias, ensure fairness, and make model predictions interpretable — especially given that female ADHD cases are often underdiagnosed in real-world healthcare.

🎯 Objectives
Predict ADHD diagnosis and biological sex using multi-modal data

Identify and address potential gender bias in model performance

Build explainable AI models using SHAP/LIME

Present results to a simulated NHS review board, focused on trust, utility, and fairness

🛠️ Tools & Technologies
Languages & Libraries: Python, Pandas, NumPy, Scikit-learn, Seaborn, SHAP, LIME

Notebook Environment: Jupyter Notebook

Techniques:

Exploratory Data Analysis (EDA)

Data Cleaning & Preprocessing

Train/Test split with Cross-Validation

Model selection (Random Forest, Logistic Regression, etc.)

Performance metrics: Accuracy, Precision, Recall, F1 Score

Explainability: SHAP (TreeExplainer), LIME (tabular classifier)

Bias & fairness evaluation

📊 Dataset
The dataset was provided by the university as part of a real-world simulation. It includes:

fMRI brain imaging data (functional activity patterns)

Demographic information (age, sex, family background)

Emotional and parenting factors

Due to GDPR and assignment policy, the dataset is not included in this repo. Please contact me for details.

🧪 Model Development Workflow
Data Exploration

Class imbalance analysis

Gender distribution

Correlation heatmaps and visualizations

Preprocessing

Handling missing values

Feature encoding & standardization

Dimensionality reduction (if applied)

Model Training

Trained multiple models (Random Forest, Logistic Regression, SVM)

Evaluated using k-fold cross-validation

Tuned hyperparameters for optimal performance

Explainability

Used SHAP to interpret feature impact

LIME used for local instance-level explanation

Gender-bias breakdown in feature influence

Evaluation & Ethics

Compared model performance across genders

Reflected on bias, utility, and limitations

Presented findings to a simulated NHS panel

🏆 Key Results
Achieved consistent prediction performance with Random Forest (balanced accuracy)

SHAP analysis revealed key predictive features differed across genders

Identified areas where the model underperforms for female samples, enabling transparency

Final presentation received distinction-level feedback (80%+) from academic reviewers

📁 Folder Structure (Recommended)
plaintext
Copy
Edit
📦adhd-diagnosis-ml
 ┣ 📂notebooks
 ┃ ┣ 📜stage1.ipynb
 ┃ ┣ 📜stage2.ipynbb
 ┣ 📂reports
 ┃ ┗ 📜nhs_presentation.pdf
 ┣ 📜README.md
 ┣ 📜requirements.txt
 ┗ 📜.gitignore
🧠 Future Improvements
Apply deep learning models (CNNs/RNNs) if raw fMRI imaging becomes available

Explore bias mitigation algorithms

Extend pipeline for real-time clinical integration

🤝 Let's Connect
If you’re interested in this work or want to collaborate on similar healthcare + AI projects, feel free to reach out via LinkedIn.
