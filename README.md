# 🚦 Road Collisions Prediction — ML Project

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/CatBoost-Best_Model-FF6600?style=for-the-badge&logoColor=white"/>
  <img src="https://img.shields.io/badge/Accuracy-92.6%25-27AE60?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <a href="https://saadawy-ai-road-collision-severity-app-app-h222ed.streamlit.app/">
    <img src="https://img.shields.io/badge/Live_Demo-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
  </a>
</p>

---

## 📌 Overview

This project analyzes real-world road collision data to predict accident severity using Machine Learning.

The project covers the complete Data Science workflow:

Data Cleaning & Preprocessing
Exploratory Data Analysis (EDA)
Feature Engineering
Model Training & Comparison
Hyperparameter Tuning
Model Evaluation
Deployment using Streamlit
🎯 Objective

Predict collision severity and identify the most important factors contributing to road accidents to support traffic safety decision-making.

---

## 🌐 Live Demo

> Try the interactive dashboard — no installation needed!

**👉 [Launch Streamlit App](https://road-collision-severity-app.streamlit.app/)**

Enter collision details (location, time, day type) and get an instant severity prediction with probability breakdown.

---

## 📂 Dataset

| Property    | Details                                     |
|-------------|---------------------------------------------|
| Format      | CSV                                         |
| Features    | Dates, locations, road conditions, weather, vehicle types, and more |
| Target      | Accident severity (3 classes: 0, 1, 2)      |
| Source      | [Download from Google Drive](https://drive.google.com/file/d/1r8EhD7sdkFjap78wLj76f8t2fTuN6owZ/view?usp=sharing) |

---

## 🛠️ Technologies & Tools

| Category        | Tools                                      |
|-----------------|--------------------------------------------|
| Language        | Python 3.10+                               |
| Data Processing | Pandas, NumPy                              |
| Visualization   | Matplotlib, Seaborn                        |
| Modeling        | Scikit-learn, CatBoost                     |
| Environment     | Jupyter Notebook                           |
| Deployment      | Streamlit Cloud                            |

---

## 🔄 Project Workflow

```
1. Data Cleaning & Preprocessing
       ↓
2. Exploratory Data Analysis (EDA)
       ↓
3. Feature Engineering
       ↓
4. Model Training
       ↓
5. Hyperparameter Tuning
       ↓
6. Model Evaluation
       ↓
7. Model Deployment
```

---

## 📊 Results

### Best Model: CatBoost

| Metric           | Score  |
|------------------|--------|
| **Accuracy**     | **92.6%** |
| Weighted F1-Score | 0.92  |
| Macro F1-Score   | 0.88   |
| Weighted Precision | 0.93 |
| Weighted Recall  | 0.93   |

### Classification Report (Per Class)

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0 (Minor)  | 1.00 | 0.75 | 0.85 | 205    |
| 1 (Serious) | 1.00 | 0.70 | 0.82 | 3,274  |
| 2 (Slight) | 0.91 | 1.00 | **0.95** | 10,534 |
| **Weighted Avg** | **0.93** | **0.93** | **0.92** | 14,013 |

> 🔑 The model achieves **perfect precision (1.00)** on classes 0 and 1, and **perfect recall (1.00)** on the dominant class 2.

---

## 📱 Application Preview

### Prediction Dashboard

![Prediction Dashboard](Images/Prediction%20Insights%20Dashboard.png)

### Sample Prediction Output

![Prediction Output](Images/Model%20Prediction%20Output.png)

---

## 📈 Model Visualizations

### Collision Severity Distribution

Understanding the distribution of collision severity classes reveals the significant class imbalance present in the dataset.

![Collision Severity Distribution](Images/Collision%20Severity%20Distribution.png)

---

### Correlation Heatmap

Correlation analysis was used to identify relationships between numerical features and detect potential dependencies.

![Correlation Heatmap](Images/Correlation%20Heatmap.png)

---

### Distribution of Important Features

Visualization of the most influential features used by the model to predict collision severity.

![Distribution of Important Features](Images/Distribution%20of%20Important%20Features.png)

---

### Learning Curve

The learning curve demonstrates the model's generalization performance and helps identify potential overfitting or underfitting issues.

![Learning Curve](Images/Learning%20Curve.png)

---

### ROC Curve

Multi-class ROC analysis evaluating the model's ability to distinguish between different collision severity classes.

![ROC Curve](Images/ROC%20Curve.png)

---

### Precision-Recall Curve

Precision-Recall analysis provides a more informative evaluation for the imbalanced dataset, especially for minority classes.

![Precision-Recall Curve](Images/Precision-Recall%20Curve.png)

---

---

## 🗂️ Repository Structure

```
Road-Collisions-ML/
│
├── Dataset/          # Dataset files
├── Notebook/         # Jupyter notebooks (EDA + Modeling)
├── Images/           # EDA plots and figures
├── README.md         # Project documentation
└── requirements.txt  # Python dependencies
```

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/Saadawy-AI/Road-Collisions-ML.git
cd Road-Collisions-ML
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Download the dataset
Place the CSV file inside the `Dataset/` folder.  
[📥 Download Dataset](https://drive.google.com/file/d/1r8EhD7sdkFjap78wLj76f8t2fTuN6owZ/view?usp=sharing)

### 4. Open the notebook
```bash
jupyter notebook
```
Navigate to `Notebook/` and run the cells in order.

---

## 🔍 Key Insights

- Road conditions, time of day, and vehicle type are among the strongest predictors of accident severity.
- The dataset is **highly imbalanced** (class 2 dominates with ~75% of samples), which influenced model selection and evaluation strategy.
- CatBoost outperformed baseline models by natively handling categorical features and class imbalance more effectively.

---

## ⚠️ Challenges

- Handling a highly imbalanced dataset where the majority of collisions belong to the Slight severity class.
- Managing categorical features with varying cardinality levels.
- Engineering meaningful temporal features from raw date and time attributes.
- Maintaining strong model performance while reducing overfitting risk.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👤 Author

**Mohamed Saadawy**  
📎 [GitHub](https://github.com/Saadawy-AI) · [LinkedIn](https://linkedin.com/in/muhammad-saadawy) · [Portfolio](https://saadawy-ai.github.io/My-Portfolio/)

---

> *This project is part of my Data Science & Machine Learning portfolio.*
