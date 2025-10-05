---
layout: page
permalink: /DE06Lab05/
---

# 🧩 Lecture Notes: Classification in Supervised Learning

### 🎯 Objectives
- Describe the classification method within supervised learning  
- Discuss real-world applications and use cases of classification  
- List common classification algorithms and explain multi-class prediction strategies  

### Understanding Classification
- **Main Ideas:**  
  - Classification is a type of **supervised machine learning** that predicts labels for new data.  
  - Labels represent **categorical variables** with discrete values.  
  - The model learns the relationship between features (inputs) and class labels (outputs) during training.  
- **Key Details:**  
  - The goal of supervised learning is to interpret data correctly to answer a specific question.  
  - As data is input, the model adjusts to fit the algorithm and classifies each sample into a category.  
  - The process ensures data-driven predictions that are consistent and contextually accurate.  
- **Extra Notes:**  
  - Reinforce that classification requires **labeled training data** to learn effectively.  
  - Mention that evaluation of classification models often involves metrics like **accuracy**, **precision**, and **recall**.

### Applications and Use Cases
- **Main Ideas:**  
  - Classification has widespread applications across industries and domains.  
  - It can be used whenever data can be mapped between features and discrete categories.  
- **Key Details:**  
  - **Common applications:**  
    - Email filtering (spam vs. not spam)  
    - Speech-to-text and handwriting recognition  
    - Biometric identification  
    - Document classification  
  - **Business examples:**  
    - *Churn prediction:* identify customers likely to discontinue a service  
    - *Customer segmentation:* categorize customers by behavior or demographics  
    - *Marketing response prediction:* forecast which customers will respond to a campaign  
  - **Bank loan example:**  
    - Train a model on historical loan default data (age, income, credit debt).  
    - Predict if a new applicant is likely to default → *binary classification* (default vs. non-default).  
  - **Healthcare example:**  
    - Predict which of multiple drugs (A, B, or C) a patient may respond to → *multi-class classification*.  
- **Extra Notes:**  
  - Highlight that classification models support **decision-making** in both operational and strategic contexts.  
  - Encourage thinking about **ethical implications** — e.g., fairness and bias in model outcomes.

### Classification Algorithms
- **Main Ideas:**  
  - Various algorithms can be used to build classification models, depending on data size and complexity.  
- **Key Details:**  
  - **Common classification algorithms:**  
    - Naive Bayes  
    - Logistic Regression  
    - Decision Trees  
    - K-Nearest Neighbors (KNN)  
    - Support Vector Machines (SVM)  
    - Neural Networks  
  - Some algorithms (e.g., Logistic Regression, KNN, Decision Trees) natively support **multi-class classification**.  
  - Others are inherently binary and require strategies to handle multiple classes.  
- **Extra Notes:**  
  - Emphasize that algorithm selection depends on data characteristics, interpretability needs, and computation cost.  
  - Encourage comparing multiple algorithms using validation techniques like **cross-validation**.

### Multi-Class Prediction Strategies
- **Main Ideas:**  
  - Binary classifiers can be extended to handle more than two classes using structured strategies.  
  - The two main approaches are **One-vs-All (OvA)** and **One-vs-One (OvO)**.  
- **Key Details:**  
  - **One-vs-All (OvA):**  
    - Builds *k* binary classifiers (one per class).  
    - Each classifier predicts whether a sample belongs to its target class or not.  
    - Data points not assigned by any classifier may represent **outliers or noise**.  
  - **One-vs-One (OvO):**  
    - Builds classifiers for every pair of classes.  
    - Each model distinguishes between two specific classes.  
    - The final label is chosen by a **voting scheme** — the class with the most “wins” across classifiers.  
    - If a tie occurs, votes may be **weighted by confidence** or probability.  
  - **Example:**  
    - For three classes (A, B, C):  
      - OvA builds 3 classifiers (A vs. rest, B vs. rest, C vs. rest).  
      - OvO builds 3 classifiers (A vs. B, A vs. C, B vs. C).  
- **Extra Notes:**  
  - ROC (Receiver Operating Characteristic) curves can also evaluate classifier performance.  
  - Multi-class strategies improve flexibility but increase computational cost.  
  - Encourage exploring algorithm libraries (e.g., scikit-learn) for built-in OvA and OvO implementations.

### 📌 Takeaways
- Classification is a **supervised learning** approach that predicts categorical outcomes.  
- It is used across fields such as finance, marketing, and healthcare.  
- Common algorithms include **Naive Bayes, Logistic Regression, Decision Trees, KNN, SVM, and Neural Networks**.  
- Binary classifiers can be extended for multi-class problems using **One-vs-All** or **One-vs-One** strategies.  
- Model choice and evaluation depend on use case, interpretability, and data characteristics.


