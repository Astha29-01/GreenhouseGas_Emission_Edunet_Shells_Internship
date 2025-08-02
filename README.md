# 🌱 Greenhouse Gas Emission Prediction (IBM SkillsBuild - Week 2)

This project is part of the IBM SkillsBuild Virtual Internship program in collaboration with Edunet Foundation. The task was to build a machine learning model that predicts **Supply Chain Emission Factors with Margins** using various descriptive and quality metrics from industrial emission data.

---

## 📁 Dataset

- **Source:** Provided as part of internship resources
- **File:** `SupplyChainEmissionFactorsforUSIndustriesCommodities.csv`
- **Data Summary:** Annual supply chain emission data (2010–2016) categorized by U.S. industries and commodities.
- **Target Variable:** `Supply Chain Emission Factors with Margins`

---

## 🎯 Problem Statement

Develop a regression model that can predict *Supply Chain Emission Factors with Margins* based on descriptive metrics such as:
- Substance
- Unit
- Reliability
- Temporal, Geographical, and Technological Correlation
- Data Collection Method

---

## 🧪 Methodology

1. **Data Cleaning**  
   - Removed irrelevant columns (`Unnamed: 7`)  
   - Dropped rows with missing values

2. **Feature Engineering**  
   - Selected numeric columns as model inputs  
   - Target: `Supply Chain Emission Factors with Margins`

3. **Model Training**  
   - Trained 3 models:  
     - Linear Regression  
     - Decision Tree Regressor  
     - Random Forest Regressor  

4. **Evaluation Metrics**  
   - Root Mean Squared Error (RMSE)  
   - Mean Absolute Error (MAE)  
   - R² Score

5. **Hyperparameter Tuning**  
   - Tuned Random Forest using `GridSearchCV` for optimal performance

6. **Visualization**  
   - RMSE Comparison Plot  
   - Actual vs Predicted (before & after tuning)  
   - Residual Distribution  
   - Feature Importance Plot

7. **Model Saving**  
   - Saved best Random Forest model using `joblib` as:  
     `best_random_forest_model.pkl`

---

## ⚙️ Tools and Technologies Used

- **Python** – General-purpose programming language  
- **Pandas** – Data analysis and manipulation  
- **NumPy** – Numerical computing with arrays  
- **Matplotlib** – Basic data visualization  
- **Seaborn** – Statistical plotting library  
- **Scikit-learn** – Machine learning model library  
- **Jupyter Notebook** – Interactive coding environment  
- **Joblib** – Model saving and loading  
- **GitHub** – Version control and collaboration

---

## 📈 Results & Insights

- Random Forest Regressor **outperformed** Linear and Decision Tree models
- **Tuned RF Model** achieved higher R² and lower RMSE
- Feature importance showed key variables contributing to emissions
- Final model is ready for **deployment in sustainability tools**

---

## 💾 How to Run

1. Clone the repository  
2. Open `greenhouse.ipynb` in Jupyter Notebook  
3. Make sure the CSV file is in the same folder  
4. Run all cells to retrain or test the model  
5. Model is saved as `best_random_forest_model.pkl`

---

## 🏁 Conclusion

This project successfully demonstrates how machine learning can support environmental sustainability through accurate emissions forecasting. By identifying key contributing factors, the model helps guide **data-driven policy and industrial decisions**.

---

## 👩‍💻 Author

**Avilipsa Mahapatra**  
IBM SkillsBuild Virtual Internship (Edunet Foundation)
