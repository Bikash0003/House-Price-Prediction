# 🏡 House Prices Prediction using TensorFlow Decision Forests

This project demonstrates how to use **TensorFlow Decision Forests (TF-DF)** to predict house prices using structured/tabular data. It provides a simple and effective baseline using tree-based models like Random Forests without requiring much feature engineering.

---

## 📌 Objective

To build a regression model that can predict house prices based on various property features using a Random Forest model implemented in TF-DF.

---

## 🔧 Tools & Libraries

- TensorFlow v2.11  
- TensorFlow Decision Forests v1.2  
- pandas, seaborn, matplotlib  
- Jupyter Notebook / Google Colab

---


---

## 🧠 Workflow

### 1. Import Libraries  
Loaded all required libraries like `tensorflow_decision_forests`, `pandas`, `seaborn`, etc.

### 2. Load & Inspect Dataset  
- Read CSV
- Dropped unnecessary columns (`Id`)
- Visualized `SalePrice` distribution

### 3. Data Splitting  
- Used custom code to split 70% training and 30% validation
- No manual preprocessing needed (TF-DF handles it)

### 4. Model Training  
- Trained `RandomForestModel` with 300 trees
- Used `fit()` method on the TF dataset

### 5. Evaluation  
- Evaluated model using **Out-of-Bag (OOB)** and **validation dataset**
- Visualized RMSE vs number of trees

### 6. Feature Importance  
- Used `NUM_AS_ROOT` metric  
- Top features: `OverallQual`, `GarageCars`, `ExterQual`, `Neighborhood`

### 7. Prediction & Submission  
- Prepared test dataset  
- Generated predictions  
- Exported final results to `submission.csv`

---

## 📈 Results & Insights

- No preprocessing needed for missing/categorical data
- TF-DF's RandomForest outperformed baseline models
- Visualizations made it easier to understand decision logic

---

## 📂 Output Files

- `sales_prediction_model.ipynb` – Full notebook
- `submission.csv` – Final predictions for Kaggle
- `README.md` – Documentation

---

## 🚀 Future Improvements

- Hyperparameter tuning
- Experimenting with `GradientBoostedTreesModel`
- Feature engineering for improved performance

---

## 🧑‍💻 Author

**Bikash Poudel**  
📧 yugal.poudel@gmail.com  
🌐 [GitHub](https://github.com/Bikash0003)

---
