# 🎓 Student Performance Analysis and Classification

This project explores and analyzes student performance data from two datasets (`student-mat.csv` and `student-por.csv`) and uses machine learning models to classify students based on various features. The goal is to evaluate and compare different classifiers (SVM, KNN, and Naive Bayes) on their ability to predict student performance.

## 📁 Project Structure

- `Final_Mini_Project.ipynb`: The main Jupyter notebook containing the entire code, analysis, visualizations, and model training.
- `student-mat.csv`: Dataset related to mathematics students.
- `student-por.csv`: Dataset related to Portuguese language students.

## 📊 Dataset Overview

The datasets contain student-related information such as:

- Demographic: Age, Sex, Address
- Family: Family size, Parents' education, Guardian
- Academic: Study time, Grades (G1, G2, G3), Failures
- Social: Free time, Going out, Alcohol consumption (Dalc, Walc)
- Support: School support, Paid classes, Internet

Both datasets are labeled for classification:
- `label = 1`: Math students
- `label = 0`: Portuguese students

## 🧠 ML Models Used

- ✅ **Support Vector Machine (SVM)** with RBF kernel (wrapped in `OneVsRestClassifier` with `Bagging`)
- ✅ **K-Nearest Neighbors (KNN)** with `k=3`
- ✅ **Naive Bayes (GaussianNB)**

Each model is trained and evaluated using:
- Confusion matrix
- Accuracy score (Train & Test)
- Average precision-recall score

## 📈 Evaluation Results

| Model       | Train Accuracy | Test Accuracy | Precision-Recall |
|-------------|----------------|---------------|------------------|
| SVM         | 82.22%         | 80.00%        | 0.76             |
| KNN         | 76.00%         | 62.50%        | 0.63             |
| Naive Bayes | 75.11%         | 87.50%        | 0.88             |

> 🔍 Naive Bayes performed best on the test set based on accuracy and precision-recall.
