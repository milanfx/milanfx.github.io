---
layout: page
permalink: /DE06Lab05/
---

# 🧩 Lecture Notes: Decision Trees for Machine Learning

### 🎯 Objectives
- Define and explain what a Decision Tree is and how it functions  
- Describe how to train, grow, and prune a Decision Tree model  
- Explain how Decision Trees learn using splitting criteria such as entropy and information gain  

### Decision Trees Overview
- **Main idea:**  
  - A Decision Tree is a supervised learning algorithm used for classification and regression.  
  - It can be visualized as a flowchart where internal nodes represent tests on features, branches represent test outcomes, and leaf nodes represent class labels.  
- **Details:**  
  - Each data point passes through the tree based on feature conditions until it reaches a leaf node.  
  - The final leaf determines the class or predicted value of that data point.  
  - Decision Trees are interpretable and can handle both categorical and numerical data.  
- **Teaching tip:**  
  - Use a simple tree diagram to show how decisions “flow” from root to leaves.

### Building a Decision Tree
- **Main idea:**  
  - Decision Trees are built recursively by selecting the best feature at each node to split the data.  
- **Details:**  
  - Start with labeled training data at a root node.  
  - Select a feature that best separates the classes based on a splitting criterion.  
  - Split the data into subsets along this feature, passing each subset to a new node.  
  - Continue until all nodes contain pure classes, features are exhausted, or a stopping rule is reached.  
- **Teaching tip:**  
  - Compare the tree-growing process to “20 Questions”: each question (split) aims to reduce uncertainty.

### Stopping Criteria and Pruning
- **Main idea:**  
  - A tree stops growing when specific conditions (stopping criteria) are met.  
  - Pruning removes unnecessary branches to prevent overfitting.  
- **Details:**  
  - Common stopping criteria include:
    - Maximum depth reached  
    - Minimum number of samples per node or per leaf exceeded  
    - Maximum number of leaf nodes reached  
  - Pruning simplifies the model, improves generalization, and enhances interpretability.  
- **Teaching tip:**  
  - Demonstrate how pruning reduces a complex tree into a simpler, more general structure.

### Example: Predicting Medication Response
- **Main idea:**  
  - Example dataset: patient features (age, gender, blood pressure, cholesterol) and target (drug A or B).  
- **Details:**  
  - The tree might split first by age (young, middle-aged, senior).  
  - If middle-aged → drug B; if young and male → drug B; if senior with high cholesterol → drug A.  
  - Each split corresponds to a test condition learned from data.  
- **Teaching tip:**  
  - Draw a sample tree to illustrate how specific patient profiles lead to different predictions.

### Splitting Criteria
- **Main idea:**  
  - The algorithm uses a metric to decide which feature provides the best split.  
- **Details:**  
  - **Entropy:** measures randomness or impurity of a node.  
    - Entropy = 0 means all samples belong to one class.  
    - Entropy = 1 means classes are evenly mixed.  
  - **Information Gain:** measures reduction in entropy after a split.  
    - Information Gain = Entropy(before) − Weighted Entropy(after).  
    - The goal is to choose features that yield the **highest information gain**.  
  - **Gini Impurity:** another popular split metric; measures how often a randomly chosen element would be incorrectly labeled.  
- **Teaching tip:**  
  - Emphasize that both entropy and Gini work similarly: they prefer splits that produce purer subsets.

### Interpretability and Advantages
- **Main idea:**  
  - Decision Trees are highly interpretable and transparent models.  
- **Details:**  
  - You can visualize how decisions are made at each node.  
  - The order of feature splits provides insight into feature importance.  
  - Trees require little data preprocessing and can handle non-linear relationships.  
- **Teaching tip:**  
  - Highlight that interpretability makes Decision Trees ideal for domains like healthcare or finance where understanding model logic is crucial.

### 📌 Takeaways
- Decision Trees classify data by recursively splitting it based on feature conditions  
- Stopping and pruning prevent overfitting and improve generalization  
- Entropy and Information Gain measure the quality of splits, aiming to maximize purity  
- Decision Trees are interpretable and reveal which features are most predictive  
- They provide an intuitive, visual framework for understanding decision boundaries


