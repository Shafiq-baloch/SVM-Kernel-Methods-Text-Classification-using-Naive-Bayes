# Day 5 Report — AI Internship

**Topic:** Support Vector Machines (SVM), Kernel Methods & Text Classification using Naive Bayes  
**Name:** Shafiq ur Rehman  
**Day:** 5  
**Date:** 07 June 2026  
**Technology Stack:** Python, Scikit-learn, Pandas, Matplotlib, TF-IDF  

---

## 🎯 Objective

The objective of Day 5 was to:

- Understand Support Vector Machines (SVM) and kernel methods  
- Train and compare different SVM kernels (Linear, RBF, Polynomial)  
- Visualize decision boundaries for classification  
- Build a text classification system using TF-IDF and Naive Bayes  
- Evaluate model performance using precision, recall, and F1-score  

---

## 📘 Part 1: Support Vector Machine (SVM)

### 🔹 Concept Understanding

Support Vector Machine (SVM) is a supervised machine learning algorithm used for classification. It works by finding the optimal hyperplane that separates different classes with the maximum margin.

**Key concepts learned:**
- Hyperplane: Decision boundary separating classes  
- Support Vectors: Data points closest to the boundary  
- Margin: Distance between classes  
- Kernel Trick: Technique to transform data into higher dimensions for non-linear separation  

---

### 🔹 Kernels Studied

**1. Linear Kernel**
- Used when data is linearly separable  

**2. RBF Kernel (Radial Basis Function)**
- Used for non-linear data  
- Creates flexible decision boundaries  

**3. Polynomial Kernel**
- Uses polynomial transformation for classification  

---

### 🔹 Implementation Summary

- Dataset: Iris dataset (150 samples, 3 classes)  
- Features: 4 numerical features  
- Train-test split applied  
- Models trained using Scikit-learn SVC  

---

### 🔹 Results

| Model            | Accuracy |
|------------------|----------|
| Linear SVM       | 1.00     |
| RBF SVM          | 1.00     |
| Polynomial SVM   | 1.00     |

---

### 🔹 Observation

All kernels achieved 100% accuracy due to the simplicity and linear separability of the Iris dataset.

- Linear kernel was sufficient  
- RBF and Polynomial did not significantly improve performance  

---

### 🔹 Decision Boundary Visualization

A 2D decision boundary was plotted using sepal length and sepal width.

- Clear separation of Setosa class  
- Partial overlap between Versicolor and Virginica  
- Linear hyperplanes dividing feature space  

---

## 📘 Part 2: Text Classification using Naive Bayes

### 🔹 Concept Understanding

Naive Bayes is a probabilistic classification algorithm based on Bayes’ Theorem. It assumes independence between features.

**Applications:**
- Spam detection  
- Sentiment analysis  
- Document classification  

---

### 🔹 TF-IDF Vectorization

Text data was converted using TF-IDF:

- TF: Term Frequency  
- IDF: Inverse Document Frequency  

This helps highlight important words and reduce common word impact.

---

### 🔹 Model Used

- Algorithm: Multinomial Naive Bayes  
- Dataset: SMS Spam Collection  
- Classes: Spam / Ham  

---

### 🔹 Evaluation Metrics

| Metric     | Score  |
|------------|--------|
| Accuracy   | 0.9668 |
| Precision  | 1.00   |
| Recall     | 0.7533 |
| F1 Score   | 0.8593 |

---

### 🔹 Observation

- Perfect precision: no normal messages were marked as spam  
- Lower recall: some spam messages were missed  
- Model is strong but can be improved with tuning  

---

## 🧠 Key Learnings

- SVM builds optimal decision boundaries using margin maximization  
- Kernel trick enables non-linear classification  
- TF-IDF converts text into meaningful numerical features  
- Naive Bayes is effective for text classification  
- Precision and recall give deeper insight than accuracy  

---

## ⚙️ Tools & Libraries Used

- Python  
- Scikit-learn (SVC, MultinomialNB, TF-IDF Vectorizer)  
- Pandas  
- Matplotlib  
- NumPy  

---

## 📌 Conclusion

Day 5 covered both geometric classification (SVM) and probabilistic text classification (Naive Bayes).

The implementation reinforced:
- Kernel methods  
- NLP preprocessing  
- Model evaluation techniques  

The SMS spam classifier demonstrated a full ML pipeline from raw text to prediction.
