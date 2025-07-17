
# 🧮 Customer Churn Prediction using KNIME

## 📌 Project Overview

This project focuses on predicting customer churn using a classification approach in KNIME. The goal is to identify customers who are likely to discontinue their service, enabling the business to take proactive retention measures.

---

## 🛠️ Tools & Technologies

- **Platform:** KNIME Analytics Platform
- **Models Used:** Logistic Regression, Decision Tree, Random Forest
- **Evaluation:** ROC Curve, Accuracy Scoring
- **Visualization:** Histograms, Pie Charts

---

## 📂 Workflow Breakdown

### 1. **Data Import & Preprocessing**
- **CSV Reader:** Imported raw customer dataset.
- **Number to String:** Converted numeric categorical values into readable string labels.
- **Color Manager:** Applied color coding for target classes.
- **Partitioning:** Split data into training and test sets for model evaluation.

### 2. **Model Training & Prediction**
Three classification models were built and evaluated:

#### ✅ Logistic Regression
- Trained on partitioned data using **Logistic Regression Learner**
- Predictions generated using **Predictor**
- Evaluated using **Scorer** and **ROC Curve (AUC)**

#### 🌳 Decision Tree
- Built using **Decision Tree Learner**
- Predictions and evaluation followed the same structure as above

#### 🌲 Random Forest
- Ensemble model trained using **Random Forest Learner**
- Applied predictions and evaluated performance similarly

### 3. **Post-processing & Filtering**
- Used **Column Filters** and **Row Filters** to clean and isolate prediction results
- Applied **Rule Engine** nodes to label results for visualization

### 4. **Result Merging & Visualization**
- Combined outputs from all models using **Concatenate**
- Visualized results using:
  - **Pie Chart**: Churn distribution
  - **Histograms**: Feature or prediction distribution
  - **ROC Curves**: Model performance comparison

---

## 📊 Key Outcomes

- Compared performance of 3 models for churn classification
- Evaluated models based on AUC-ROC and prediction accuracy
- Built a modular, reusable KNIME workflow for business use cases
- Created easy-to-interpret visual summaries of model outputs

---

## 📎 Files & Resources

- 🔗 KNIME Workflow File: `customer_churn_knime_workflow.knwf`
- 🖼️ Screenshots of workflow & visualizations:  (./Screenshot%202025-07-12%20154137.png)
  


---

*This project was built as part of my learning journey in predictive analytics and model evaluation using visual tools like KNIME.*
