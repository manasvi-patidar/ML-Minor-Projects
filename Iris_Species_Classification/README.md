# 🌸 Iris Species Classification | Supervised Machine Learning

A supervised machine learning project that predicts the species of an Iris flower
from its physical measurements, using **KNN**, **Logistic Regression** and **Naive Bayes**.

---

## 📌 Problem Statement

A botanical research centre wants to automate Iris species identification, since manual identification from sepal/petal measurements is slow, error-prone and not scalable.

**Goal:** Train KNN, Logistic Regression and Naive Bayes classifiers on the flower measurements, compare their performance and identify the best algorithm.

---

## 📊 Dataset

- **File:** `Iris.csv`
- **Samples:** 150

| Feature            | Description                                  |
| ------------------ | -------------------------------------------- |
| `SepalLengthCm`    | Length of sepal (cm)                         |
| `SepalWidthCm`     | Width of sepal (cm)                          |
| `PetalLengthCm`    | Length of petal (cm)                         |
| `PetalWidthCm`     | Width of petal (cm)                          |
| `Species` (target) | Iris-setosa, Iris-versicolor, Iris-virginica |

---

## 🤖 Models Used

- K-Nearest Neighbours (KNN)
- Logistic Regression
- Gaussian Naive Bayes

---

## 📈 Results

> **Note:** Models were trained on 50% of the dataset (75 samples) and evaluated on the full dataset (150 samples).

| Model                   | Accuracy   | Misclassified Samples                         |
| ----------------------- | ---------- | --------------------------------------------- |
| **Logistic Regression** | **1.0000** | 0 / 150                                       |
| KNN                     | 0.9933     | 1 / 150 (1 versicolor predicted as virginica) |
| Naive Bayes             | 0.9933     | 1 / 150 (1 virginica predicted as versicolor) |

---

## 🏆 Conclusion

- **Logistic Regression is the best performer** with 100% accuracy.
- KNN and Naive Bayes are very close at 99.33%, each making just one error.

---

## 🛠️ Tech Stack

- Python 3
- pandas
- scikit-learn
- Jupyter Notebook

---

## Author

**Manasvi Patidar**
