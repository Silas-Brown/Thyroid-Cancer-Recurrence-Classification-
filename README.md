# Thyroid Cancer Prediction  

## (1) Overview  

This project builds a **binary classification model** to predict the recurrence of thyroid cancer. 

✅ **Dataset:** 383 patients, 16 features  
✅ **Goal:** Predict recurrence of thyroid cancer  
✅ **Result:** PR_AUC of final model is 97%
---

## (2) Methodology  

### 🔹 2.1 Data Processing    
  - **Medical history and attributes:** → Ranked, one-hot encoded, age is continous  
  - **Data Cleaning:** Missing values imputed using KNN


### 🔹 2.2 Feature engineering
  - **Interaction terms** To test if the effects of a variable depends on other variables
  - **Ranking a feature by different metrics** One by size of tumour, the other by aggression of tumour

### 🔹 2.3 Selecting performance metric and a model
  - **Wide range of classification models trained:** Multiple performance metrics are examined for each model
  - **PR_AUC selected:** On the basis of imbalanced data and a focus on the positive class (cancer)
  - **Linear SVM selected:** Highest PR_AUC of 99.3%

### 🔹 2.4 Feature pruning  
  - **Generated 95% CIs for coefficients using bootstrapping:** Eliminated features whose CIs contained zero
### 🔹 2.5 Validation on pruned model
  - **Features reduced from 21 to 7**
  - **Performance largely maintained on our most valued metric:** PR_AUC = 97%
---

## (3) Implementation  

### **🔗 Full Implementation in Colab:**  
https://colab.research.google.com/drive/1HBJ4vNzhE8wzPqZq5misDjRNLTYPL31i?usp=sharing
---

## (4) Future Improvements  
🔹 Test deep learning methods    
---

## (5) Contact  
📧 Email: **silasaverybrown@gmail.com**  
💡 LinkedIn: [Silas Brown](https://www.linkedin.com/in/silas-brown/) 
