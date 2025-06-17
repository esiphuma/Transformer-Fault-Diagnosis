# Condition Monitoring of Power Transformers Using AI: Addressing Class Imbalance  

## Overview  

Power transformers are essential assets in electrical grids, ensuring stable energy distribution. Over time, aging transformers become prone to faults, increasing maintenance costs and the risk of failures. **Artificial Intelligence (AI)** enhances fault diagnosis through **machine learning**, enabling predictive maintenance and reducing downtime.  

However, most **Dissolved Gas Analysis (DGA) datasets** suffer from **class imbalance**, where most transformers are categorized as "Good," while fewer cases exist in "Fair" or "Poor" conditions. This imbalance leads to biased machine learning models that struggle to accurately detect minority fault conditions.  

This project applies **five AI models** (**SVM, Decision Tree, Random Forest, Logistic Regression, and KNN**) to transformer condition classification. To address imbalance, multiple **resampling techniques** (**SMOTE, ADASYN, Random Oversampling, SMOTE-ENN, etc.)** were explored. Models were evaluated using **AUC, Precision, Recall, F1-Score** to determine the best-performing classifier and resampling method.  

## Dataset  

The dataset used in this study can be accessed here: [Dissolved Gas Analysis of Transformer Dataset](https://www.kaggle.com/datasets/bantipatel20/dissolved-gas-analysis-of-transformer). It contains gas concentration and electrical parameters for transformer condition classification (**Good, Fair, Poor**).  

## Resampling Methods  

To handle imbalance, the following techniques were applied:  
- **Oversampling:** SMOTE, ADASYN, Random Oversampling  
- **Undersampling:** Random Undersampling, Cluster Centroids  
- **Hybrid Methods:** SMOTE-Tomek, SMOTE-ENN, SVM-SMOTE  

## Model Development  

The models were trained on balanced datasets using various **resampling methods**, fine-tuned for optimal performance.  

## Results  

Key findings indicate **Random Forest** as the top-performing classifier, with **SMOTE-ENN** emerging as the best resampling method for improving fault detection accuracy.  

## Installation & Usage  

To run the notebook:  
```bash
git clone https://github.com/your-username/Transformer-Fault-Diagnosis.git  
cd Transformer-Fault-Diagnosis  
pip install -r requirements.txt  
jupyter notebook  


