Breast Cancer Classification using SVM
📌 Project Overview
This project implements a Support Vector Machine (SVM) classifier to predict whether a breast tumor is malignant (cancerous) or benign (non-cancerous) using the Breast Cancer Wisconsin (Diagnostic) Dataset.

The model is trained on 30 features (like mean radius, mean texture, etc.) and evaluated for performance. Additionally, a 2D decision boundary visualization is provided for better interpretability.

🛠 Technologies & Libraries Used
Python

Scikit-learn (SVC, StandardScaler, train_test_split)

Matplotlib (for visualization)

NumPy (for numerical operations)

📊 Key Steps & Methodology
1. Data Loading & Preprocessing
Dataset loaded from sklearn.datasets.

Features are scaled using StandardScaler (SVM is sensitive to feature scales).

Data split into 80% training and 20% testing.

2. Model Training (SVM with Linear Kernel)
Linear SVM (kernel='linear') trained on all 30 features.

Hyperparameter C=1.0 (controls regularization).

3. Model Evaluation
Accuracy score

Confusion matrix

Classification report (precision, recall, F1-score)

4. Decision Boundary Visualization
A 2D plot of the decision boundary for the first two features (mean radius vs. mean texture).

 How to Run the Code
Install dependencies:

bash
pip install numpy matplotlib scikit-learn
Run the Jupyter Notebook / Python script:

bash
python breast_cancer_svm.py
(or execute in a Jupyter notebook)

🌟 Key Learnings
✔ SVM works well for binary classification tasks with proper feature scaling.
✔ Visualizing decision boundaries helps in model interpretability.
✔ Scikit-learn provides easy-to-use tools for model evaluation.

📂 Project Structure
text
breast-cancer-svm/
├── breast_cancer_svm.py  # Main Python script
├── README.md             # Project documentation
└── requirements.txt      # Dependencies (optional)
🔗 Useful Links
Scikit-learn SVM Documentation

Breast Cancer Dataset Info

Helps in understanding how SVM separates malignant vs. benign cases.

📈 Results
The trained SVM model achieves:
✅ High accuracy (~95-98%) on the test set.
✅ Clear separation between malignant and benign cases in the decision boundary plot.
