# XAI-Interpretable-ML II: Understanding Interpretability using imodels

## Overview  

This repository features demos of different interpretable machine learning models from the imodels library, using the Iris dataset. The aim is to understand how these models make decisions when classifying iris flower species based on their features.  

## Dataset  

The Iris dataset consists of 150 samples from three species of iris flowers: Setosa, Versicolor, and Virginica. Each sample has four features:  
- Sepal Length  
- Sepal Width  
- Petal Length  
- Petal Width  

The target labels are the species of the flowers.  

## Models Used  

This demo repository uses three models from the `imodels` library:  
1. **Skope Rules Classifier**  
2. **Optimal Rule List Classifier**  
3. **Boosted Rules Classifier**

---

### 1. Skope Rules Classifier  

The Skope Rules Classifier generates interpretable rules that accurately classify data by identifying the most important features.  

![image](https://github.com/user-attachments/assets/f3eb6804-62a8-49d6-98d0-72f0aa9fdf65)  

Accuracy: 67.92%  
Precision: 0.52  
Recall: 0.68  
F1 Score: 0.57  

The Skope Rules Classifier performed decently but struggled with precision, leading to false positives.  

---

### 2. Optimal Rule List Classifier  

The Optimal Rule List Classifier combines the interpretability of rule-based models with effective classification, creating a list of optimal rules for data classification.  

![image](https://github.com/user-attachments/assets/29f776da-e4b0-494b-892e-7b24d5eee247)  

Accuracy: 67.92%  
Precision: 0.52  
Recall: 0.68  
F1 Score: 0.57  

The Optimal Rule List Classifier showed the same accuracy as Skope, its low precision indicates it misclassified a good number of positive cases.  

---

### 3. Boosted Rules Classifier  

The Boosted Rules Classifier improves accuracy through an ensemble of rules generated iteratively. It focuses on correcting misclassifications from previous rounds.  

![image](https://github.com/user-attachments/assets/79fca3f9-9d04-4873-8472-d8cf2a0bc658)  

Accuracy: 88.68%  
Precision: 0.92  
Recall: 0.89  
F1 Score: 0.88  

The Boosted Rules Classifier outperformed the others, achieving high accuracy and effectively identifying species.
