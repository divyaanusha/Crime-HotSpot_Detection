# 🚓 Crime Incident Analysis & Prediction using PySpark

This project uses real-world police incident data to analyze, visualize, and predict crime types using Apache Spark. It includes:
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Balancing (Oversampling/Undersampling)
- Model Training & Evaluation (Logistic Regression, Random Forest, GBT)
- Scalable pipeline using PySpark

---

---

## 🔍 Problem Statement

Given crime incident records, can we:
- Understand trends over time, location, and day of the week?
- Predict whether an incident belongs to a **high-priority crime type** (e.g., burglary)?
- Evaluate and compare model performance in a scalable manner?

---

## ⚙️ Technologies Used

| Tool           | Purpose                             |
|----------------|-------------------------------------|
| **Apache Spark (PySpark)** | Scalable data processing and ML |
| **Pandas & Matplotlib**   | Lightweight EDA and visualization |
| **MLlib**                 | ML modeling (LogReg, RF, GBT)    |
| **Docker (optional)**     | Containerization                |
| **Jupyter Notebook**      | Prototyping & visualization     |

---

## 🧪 Features & Workflow

### ✅ Data Preprocessing
- Clean column names
- Handle missing values with `Imputer`
- Extract date features: year, month, day, hour, weekday

### 📊 EDA & Visualization
- Crime counts by weekday, year, location type
- Top crime types
- Trends over time

### 🧠 Feature Engineering
- `StringIndexer` for categorical labels
- Vectorization and scaling of features using `VectorAssembler` + `MinMaxScaler`

### 🔁 Balancing the Dataset
- Oversample minority class
- Undersample majority class

### 🔍 ML Modeling
- Logistic Regression
- Random Forest
- Gradient-Boosted Trees
- Evaluation: Accuracy, Precision, Recall, F1 Score

---

## 📈 Results Summary

| Model                  | Accuracy | Precision | Recall | F1 Score |
|------------------------|----------|-----------|--------|----------|
| Logistic Regression    | 98.32%   | 96.67%    | 98.32% | 97.49%   |
| Random Forest          | 98.57%   | 97.17%    | 98.57% | 97.87%   |
| Gradient-Boosted Trees | 98.32%   | 96.67%    | 98.32% | 97.49%   |

---

## 📊 Visualizations

![Model Metrics](path/to/model-metrics-plot.png)

---

## 📦 Installation & Usage

### 1. Clone the Repository
```bash
git clone https://github.com/<anusha>/crime-analysis-pyspark.git
cd crime-analysis-pyspark

2. Install Dependencies


pip install -r requirements.txt
3. Run the Spark Script


spark-submit scripts/spark_pipeline.py
4. (Optional) Launch Jupyter Notebook


jupyter notebook notebooks/eda_visualization.ipynb
📚 Dataset
The dataset used is Police_Incidents.csv, which includes:

Time, location, and type of incident

Complainant details

Geospatial coordinates


🧑‍💻 Author
Divya Anusha
LinkedIn | GitHub


