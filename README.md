# Breast_Cancer_detection_KNN

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-learn" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
</div>

<h1 align="center">
  <br>
  <a href="https://github.com/your-username/breast-cancer-detection-knn"><img src="https://raw.githubusercontent.com/Anandp711/Weather-prediction-using-multiple-models/main/Assets/images/header.png" alt="Breast Cancer Detection with KNN" width="600"></a>
  <br>
  Breast Cancer Detection with K-Nearest Neighbors (KNN) 🩺
  <br>
</h1>

<div align="center">
  <p>
    A machine learning project leveraging the K-Nearest Neighbors (KNN) algorithm for accurate breast cancer diagnosis.
  </p>
</div>

<br>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#features">Features</a></li>
    <li><a href="#dataset">Dataset</a></li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#model-performance">Model Performance</a></li>
    <li><a href="#contributing">Contributing</a></li>
  </ol>
</details>

---

## <a id="about-the-project"></a> 📚 About The Project

This project implements the **K-Nearest Neighbors (KNN)** algorithm for the critical task of breast cancer detection. Utilizing a dataset of breast cancer features, the notebook demonstrates a complete machine learning pipeline from data loading and preprocessing to model training, prediction, and evaluation. The aim is to classify tumors as either malignant (M) or benign (B) with high accuracy, providing a foundational example for medical diagnostics using machine learning.

---

## <a id="features"></a> ✨ Features

* **Data Loading & Initial Cleaning**: Loads the breast cancer dataset (`data.csv`) and performs essential cleaning steps, including handling missing values and dropping irrelevant columns.
* **Target Variable Encoding**: Transforms the categorical 'diagnosis' feature (M/B) into numerical format using `LabelEncoder` for model compatibility.
* **Data Splitting**: Divides the dataset into training and testing sets to evaluate the model's generalization capability robustly.
* **Feature Scaling**: Applies `StandardScaler` to normalize numerical features, which is particularly important for distance-based algorithms like KNN to ensure all features contribute equally to the distance calculation.
* **KNN Model Training & Optimization**: Trains the `KNeighborsClassifier` and iterates through different values of `n_neighbors` (from 1 to 5) to find the optimal `k` for best performance.
* **Accuracy Evaluation**: Calculates and presents the accuracy score for each `k` value, allowing for a clear comparison of model performance.

---

## <a id="dataset"></a> 📊 Dataset

The project uses a breast cancer dataset, typically named `data.csv`, which includes various features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. These features describe characteristics of the cell nuclei present in the image.

**Key Columns:**
* `id` (patient ID)
* `diagnosis` (M = malignant, B = benign - **Target Variable**)
* **Numerous numerical features** such as `radius_mean`, `texture_mean`, `perimeter_mean`, `area_mean`, `smoothness_mean`, `compactness_mean`, `concavity_mean`, `concave points_mean`, `symmetry_mean`, `fractal_dimension_mean`, and their `_se` (standard error) and `_worst` (largest/worst) counterparts.

---

📈 Model Performance
The KNN model was evaluated for different values of n_neighbors (k). The accuracy scores are as follows:

n_neighbors (k)	Accuracy Score
1	95.61%
2	94.74%
3	96.49%
4	96.49%
5	96.49%

Export to Sheets
The highest accuracy of 96.49% was achieved with n_neighbors values of 3, 4, and 5. This indicates the model's strong capability in classifying breast cancer effectively.
