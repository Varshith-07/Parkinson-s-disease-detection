# 🧠 Parkinson's Disease Detection using Machine Learning

This project aims to build a machine learning model to detect **Parkinson’s Disease** using vocal and biomedical features extracted from patient voice recordings.

---

## 📌 Problem Statement

Parkinson's Disease is a progressive nervous system disorder that affects movement. Early diagnosis is crucial for better treatment outcomes. This project uses supervised learning techniques on a CSV dataset to classify whether a person has Parkinson's or not based on various biomedical voice features.

---

## 📂 Dataset

- **Source**: UCI Machine Learning Repository (Parkinson’s dataset)
- **Size**: 195 samples × 24 columns
- **Target Column**: `status`  
  - `1` = Parkinson's Positive  
  - `0` = Healthy

---

## 🧪 Project Workflow

### 1. 📥 Import Libraries
Essential libraries like `NumPy`, `pandas`, `sklearn`, etc. were used.

### 2. 📊 Data Exploration & Preprocessing
- Loaded CSV dataset using `pandas`
- Checked for nulls (none present)
- Explored dataset with `.info()` and `.describe()`
- Set `X` (features) and `Y` (target)
- Standardized features using `StandardScaler`

### 3. 🧾 Train-Test Split
- Split dataset into training (65%) and testing (35%)
- Used `train_test_split` from `sklearn`

### 4. 🤖 ML Models Used
Trained and evaluated the following classification models:

| Model               | Training Accuracy | Test Accuracy |
|--------------------|-------------------|---------------|
| Support Vector Machine (SVM) | 92.06% | 88.41% |
| Logistic Regression          | 87.30% | 76.81% |
| K-Nearest Neighbors (KNN)    | 96.83% | 91.30% |
| Decision Tree                | 100%   | 76.81% |

### 5. 📈 Evaluation Metrics
Used:
- **Accuracy**
- **Confusion Matrix**
- **Precision, Recall, F1-Score**

---

## ✅ Results & Conclusion

- **KNN** gave the best test performance with **91.30% accuracy** and balanced precision-recall.
- **SVM** also showed strong generalization with **88.41%** test accuracy.
- **Decision Tree** overfit the training data (100% train accuracy) with a drop in test performance.
- Logistic Regression performed reasonably but had relatively lower precision for class 0 (healthy).

---

## 🚀 How to Run

1. Clone the repository or open the Colab notebook.
2. Ensure dataset `parkinsons data.csv` is available in your environment.
3. Run all cells in order.
4. Observe model performances and confusion matrices.

---

## 🛠️ Libraries Used

- `pandas`
- `numpy`
- `sklearn` (SVM, KNN, LogisticRegression, DecisionTree, metrics, preprocessing)

---

## 📌 Future Improvements

- Use feature selection or dimensionality reduction (e.g., PCA)
- Try ensemble models like Gradient Boosting or XGBoost
- Incorporate cross-validation to prevent overfitting

---

## 👤 Author

- **[Your Name]**  
- Machine Learning Enthusiast | Open to Collaboration

---

## 📄 License

This project is for educational purposes.

