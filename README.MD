# Breast Cancer Diagnosis using Machine Learning 🎗️

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

## 📌 Project Overview

This project is a machine learning analysis designed to classify breast cancer tumors as either **Malignant** (cancerous) or **Benign** (non-cancerous). Using the **Breast Cancer Wisconsin (Diagnostic) Dataset**, we trained and evaluated three distinct classification models to assist medical professionals in early diagnosis.

The system utilizes quantitative features computed from digitized images of a fine needle aspirate (FNA) of a breast mass to predict the diagnosis with high accuracy.

## 🔗 Project Links

* **Kaggle Notebook:** [View Project on Kaggle](https://www.kaggle.com/code/charithapiyumal/breast-cancer-diagnosis-using-machine-learning)
* **GitHub Repository:** [View Project on GitHub](https://github.com/DarkPhoenix2016/Breast-Cancer-Diagnosis-ML-Project)

---

## 🚀 Workflow

The project follows a standard data science pipeline, from data extraction to model evaluation.

```mermaid
graph LR
    A["Raw Dataset"] --> B["Preprocessing"]
    B --> C["EDA & Visualization"]
    C --> D{"Model Training"}
    D --> E["Logistic Regression"]
    D --> F["Support Vector Machine"]
    D --> G["Neural Network"]
    E --> H["Evaluation Metrics"]
    F --> H
    G --> H
    H --> I["Final Prediction"]
````

-----

## 📂 Repository Structure

The project is organized as follows:

```text
Breast_Cancer_Project/
│
├── data/                   # Contains the dataset (breast_cancer_data.csv)
├── images/                 # Generated plots (Confusion Matrices, Heatmaps)
├── notebooks/              # Jupyter Notebooks containing the source code
│   └── Breast_Cancer_Analysis.ipynb
├── README.md               # Project Documentation
└── requirements.txt        # Python dependencies
```

-----

## 📊 Key Results

We trained three models and optimized them using **GridSearchCV**. The **Logistic Regression** model proved to be the most effective for this specific dataset, achieving perfect sensitivity (Recall).

| Model | Accuracy | Precision | Recall | F1 Score |
| :--- | :--- | :--- | :--- | :--- |
| **Logistic Regression** | **99.12%** | **98.61%** | **100.0%** | **99.30%** |
| Support Vector Machine (SVM) | 98.25% | 97.26% | 100.0% | 98.61% |
| Neural Network (MLP) | 98.25% | 98.59% | 98.59% | 98.59% |

> **Note:** A Recall of 100% means the model successfully identified **all** malignant cases in the test set without any False Negatives.

-----

## 🛠️ Installation & Usage

### 1\. Clone the Repository

```bash
git clone [https://github.com/DarkPhoenix2016/Breast-Cancer-Diagnosis-ML-Project.git](https://github.com/DarkPhoenix2016/Breast-Cancer-Diagnosis-ML-Project.git)
cd Breast-Cancer-Diagnosis-ML-Project
```

### 2\. Install Dependencies

Ensure you have Python installed. Install the required libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3\. Run the Analysis

Launch Jupyter Notebook to view the code and run the cells:

```bash
jupyter notebook notebooks/Breast_Cancer_Analysis.ipynb
```

-----

## 📈 Visualizations

The analysis includes detailed visualizations to understand the data:

  * **Correlation Heatmap:** Identifies relationships between cell features (e.g., Radius vs. Area).
  * **Class Distribution:** Checks for dataset imbalance.
  * **Confusion Matrices:** Visualizes the performance of each model.

-----

## 🔮 Future Improvements

  * **Deep Learning:** Implement Convolutional Neural Networks (CNNs) to analyze raw histology images directly.
  * **Web Deployment:** Create a Streamlit or Flask web app to allow doctors to input data manually.
  * **Explainability:** Integrate SHAP values to explain *why* a specific prediction was made.

-----

## 👨‍💻 Author

**Charitha Piyumal**

  * Student @ Horizon Campus - IT Faculty

-----

## 📜 License

This project is open-source and available under the MIT License.

````