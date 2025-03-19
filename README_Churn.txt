
#  Telco Customer Churn Prediction  

This project aims to predict customer churn for a telecom company using machine learning models such as **Random Forest**, **XGBoost**, and **Neural Networks**. The goal is to maximize recall since predicting customer churn accurately is crucial for business retention strategies.  

---

## **Project Overview**  
Customer churn is a major challenge for telecom companies. Retaining customers is more cost-effective than acquiring new ones. This project builds and evaluates various machine learning models to identify customers likely to churn, helping the business take proactive measures.  

---

## **Dataset**  
- **Source:** Kaggle — [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)  
- **Size:** ~7,000 records  
- **Features:**  
    - Customer demographics  
    - Contract details  
    - Payment information  
    - Internet and phone services  
- **Target:** `Churn` (Yes/No)  

---

## **Goal**  
- **Maximize Recall** → Minimize false negatives (correctly identify customers likely to churn).  
- **Handle Class Imbalance** → Techniques like `SMOTE` and `scale_pos_weight` were used.  

---

## **Models Tested**  
✅ Logistic Regression  
✅ Random Forest (Top Performer)  
✅ XGBoost (Strong Performance with Minimal Tuning)  
✅ Neural Network  


---

## **Performance Highlights**  
| Model               | Recall | Precision | F1-Score | ROC AUC |
|---------------------|--------|-----------|-----------|---------|
| **Random Forest**   | 0.83   | 0.61      | 0.55      | 0.78    |
| **XGBoost**         | 0.78   | 0.68      | 0.73      | 0.80    |
| Neural Network      | 0.72   | 0.48      | 0.61      | 0.75    |

---

##  **Approach**  
1. **Exploratory Data Analysis (EDA):**  
   - Handled missing values  
   - Visualized correlations and customer trends using **Plotly**  

2. **Feature Engineering:**  
   - One-hot encoding for categorical variables  
   - Extracted top features using feature importance from Random Forest  

3. **Model Training:**  
   - Addressed class imbalance using `scale_pos_weight`  
   - Early stopping to prevent overfitting  

4. **Threshold Tuning:**  
   - Optimized decision threshold for better recall  

5. **Model Evaluation:**  
   - Precision, Recall, F1-Score, and ROC AUC metrics  
   - Confusion matrix analysis  

---

##  **Key Findings**  
- **Random Forest** was the most effective at predicting churn with the highest recall.  
- **XGBoost** performed exceptionally well with minimal fine-tuning.  
- Class imbalance influenced the performance of all models, but ensemble methods handled it better.  

---

## **Future Work**  
- Further fine-tuning of XGBoost to push recall higher  
- Test more complex Neural Networks (if hardware allows)  
- Include customer feedback for sentiment analysis  
- Explore advanced resampling techniques for better class balance  

---

## **Setup and Installation**  
### 1. **Clone the Repository**  
```bash
git clone https://github.com/ArkapratimDas0707/telco-churn-prediction.git
cd telco-churn-prediction
```

### 2. **Create and Activate Virtual Environment**  
```bash
python -m venv venv
source venv/bin/activate   # MacOS/Linux
.
env\Scripts ctivate    # Windows
```

### 3. **Install Dependencies**  
```bash
pip install -r requirements.txt
```

### 4. **Run the Project**  
```bash
python main.py
```

---

## **Plots & Visualizations**  
Interactive plots are available in the `/plots` folder.  
To view interactive Plotly charts, open `plots.html` or use **GitHub Pages**.  

---

## **Contributing**  
Feel free to fork the repository and submit pull requests. For major changes, open an issue first to discuss the proposal.  

---

## **Author**  
**[Arkapratim Das]**  
📧 [arkapratimdas70@gmail.com]
🌐 [https://www.linkedin.com/in/arkapratimdas]  

---

##  **License**  
This project is licensed under the **MIT License**.  
