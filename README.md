# Transformer-Fault-Diagnosis
# Transformer Fault Diagnosis Using Machine Learning  

## Overview  
This project explores **resampling techniques** to address class imbalance in **Dissolved Gas Analysis (DGA)** for power transformers. Various ML models (**SVM, DT, RF, LR, KNN**) were trained and evaluated using metrics like **AUC, Precision, Recall, F1-Score**.  

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
Key findings indicate **Random Forest** as the top-performing classifier, with **SMOTE-ENN** emerging as the best resampling method.  

## Installation & Usage  
To run the notebook:  
```bash
git clone https://github.com/your-username/Transformer-Fault-Diagnosis.git  
cd Transformer-Fault-Diagnosis  
pip install -r requirements.txt  
jupyter notebook  

