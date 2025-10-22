---
layout: page
permalink: /DS05M5/
---

## M3 - Probability Distributions
- **01 - Random Numbers and Probability Distributions**
- **02 - State your Hypothesis**
- **03 - Normal Distribution**
- **04 - T distribution**
- **05 - Probability of Getting a High or Low Teaching Evaluation**

## 01 - Course Introduction

<div style="display:grid; grid-template-columns: 6fr 4fr;"><div markdown="1" style="min-width:0;">
    
- **Topic01** - Fundamental Concepts of **Probability** and **Random Variables**  
- **Topic02** - Structure and Interpretation of **Probability Distributions**  
- **Topic03** - Application of **Cumulative Distribution Function (CDF)**  
- **Topic04** - Modeling with **Normal Distribution** using **Mean** and **Standard Deviation**

</div><div style="text-align:center;">
    <img src="/images/M101.jpg">
</div></div>


### 01 - Define Software Engineering

<div style="display:grid; grid-template-columns: 6fr 4fr;"><div markdown="1" style="min-width:0;">

- **Probability Distribution** models all potential values a **Random Variable** may assume along with their corresponding **Probabilities**.
- **Probability Distribution** assigns a **Probability Value** to each possible **Outcome** of a **Random Variable**.  
    - Example: Rolling two dice produces outcomes ranging from **2 to 12**.  
- **Outcome Frequencies** determine **Distribution Shape**.  
    - **Sum = 2**: occurs once (**1/36 = 0.028**).  
    - **Sum = 3**: occurs twice (**2/36 = 0.056**).  
    - **Sum = 4**: occurs three times (**3/36 = 0.083**).  
    - **Sum = 5**: occurs four times (**4/36 = 0.111**).  
    - **Sum = 7**: occurs six times (**6/36 = 0.167**), representing the most **Frequent Outcome**.  
- **Total Probability** across all outcomes always **Sums to 1**, ensuring **Completeness** of the probability model.  
- **Probability of Getting 12** (both dice show six) equals **1/36 = 0.028**.  
- **Probability of Getting More than 12** equals **0**, since **12** is the **Maximum Possible Sum**.  
- **Probability Distribution** models all potential values a **Random Variable** may assume along with their corresponding **Probabilities**.
- **Probability Distribution** assigns a **Probability Value** to each possible **Outcome** of a **Random Variable**.  
    - Example: Rolling two dice produces outcomes ranging from **2 to 12**.  
- **Outcome Frequencies** determine **Distribution Shape**.  
    - **Sum = 2**: occurs once (**1/36 = 0.028**).  
    - **Sum = 3**: occurs twice (**2/36 = 0.056**).  
    - **Sum = 4**: occurs three times (**3/36 = 0.083**).  
    - **Sum = 5**: occurs four times (**4/36 = 0.111**).  
    - **Sum = 7**: occurs six times (**6/36 = 0.167**), representing the most **Frequent Outcome**.  
- **Total Probability** across all outcomes always **Sums to 1**, ensuring **Completeness** of the probability model.  
- **Probability of Getting 12** (both dice show six) equals **1/36 = 0.028**.  
- **Probability of Getting More than 12** equals **0**, since **12** is the **Maximum Possible Sum**.

</div><div style="text-align:center;">
    <img src="/images/M102.jpg">
</div></div>

### Topic02 - Course Introdution

<div style="display:grid; grid-template-columns: 6fr 4fr;"><div markdown="1" style="min-width:0;">

- **Probability Distribution** models all potential values a **Random Variable** may assume along with their corresponding **Probabilities**.
- **Probability Distribution** assigns a **Probability Value** to each possible **Outcome** of a **Random Variable**.  
    - Example: Rolling two dice produces outcomes ranging from **2 to 12**.  
- **Outcome Frequencies** determine **Distribution Shape**.  
    - **Sum = 2**: occurs once (**1/36 = 0.028**).  
    - **Sum = 3**: occurs twice (**2/36 = 0.056**).  
    - **Sum = 4**: occurs three times (**3/36 = 0.083**).  
    - **Sum = 5**: occurs four times (**4/36 = 0.111**).  
    - **Sum = 7**: occurs six times (**6/36 = 0.167**), representing the most **Frequent Outcome**.  
- **Total Probability** across all outcomes always **Sums to 1**, ensuring **Completeness** of the probability model.  
- **Probability of Getting 12** (both dice show six) equals **1/36 = 0.028**.  
- **Probability of Getting More than 12** equals **0**, since **12** is the **Maximum Possible Sum**.  

</div><div style="text-align:center;">
    <img src="/images/M102.jpg"><img src="/images/M103.jpg">
</div></div>
  
### Topic03 - How to Learn

<div style="display:grid; grid-template-columns: 6fr 4fr;"><div markdown="1" style="min-width:0;">

- **Main Ideas:**
    - **Cumulative Distribution Function (CDF)** measures the **Probability** that a random variable takes a value **Less Than or Equal To** a specified number.

- **Core Notes:**  
    - **CDF** aggregates **Individual Probabilities** up to a specific **Value Threshold**.  
        - Example: **Probability of Getting ≤ 6** equals **0.417**, while **≥ 6** equals **0.58**.  
    - **CDF Graphs** visualize cumulative probabilities across all outcomes, showing how **Probabilities Accumulate** to **1**.  

</div><div style="text-align:center;">
    <img src="/images/M104.jpg">
</div></div>

## 02 - What is Software Engineering?

<div style="display:grid; grid-template-columns: 6fr 4fr;"><div markdown="1" style="min-width:0;">

- **Topic01** - Definition and Purpose of **Statistical Hypothesis Testing**  
- **Topic02** - Formulation of **Null Hypothesis (H₀)** and **Alternative Hypothesis (Hₐ)**  
- **Topic03** - Comparison of **Mean Scores** between Two Entities  

</div><div style="text-align:center;">
    <img src="/images/M104.jpg"><img src="/images/M105.jpg">
</div></div>

### Topic01 - Define Software Engineering

<div style="display:grid; grid-template-columns: 6fr 4fr;"><div markdown="1" style="min-width:0;">

- **Main Ideas:**
    - **Statistical Hypothesis Testing** is used to compare the **Averages** or **Means** of two entities to determine if a significant difference exists.

- **Core Notes:**  
    - **Hypothesis Testing** provides a framework to test whether observed differences between two **Sample Means** are due to **Random Variation** or a **True Difference**.  
    - Example: Comparing **Average Points per Game** between **Michael Jordan** and **Wilt Chamberlain**.  
    - **Michael Jordan** averaged **30.12 Points per Game**, while **Wilt Chamberlain** averaged **30.06 Points per Game**.  
    - Despite the similarity of these averages, a **Formal Statistical Test** is required to evaluate if the difference is **Statistically Significant**.  

</div><div style="text-align:center;">
    <img src="/images/M103.jpg">
</div></div>

### Topic02 - Software Crisis

<div style="display:grid; grid-template-columns: 6fr 4fr;"><div markdown="1" style="min-width:0;">

- **Main Ideas:**
    - **Null Hypothesis (H₀)** assumes no difference between means, while **Alternative Hypothesis (Hₐ)** assumes a difference or directional effect.

- **Core Notes:**  
    - **Null Hypothesis (H₀)**: Represents the assumption that there is **No Difference** between the averages.  
        - Expressed as **μ_J = μ_C**, where **μ_J** is the mean score of **Michael Jordan** and **μ_C** is the mean score of **Wilt Chamberlain**.  
        - Example: If the **Averages are the Same**, the **Difference between the Means** equals **Zero**.  
    - **Alternative Hypothesis (Hₐ)**: Suggests that the averages are **Not Equal**.  
        - Expressed as **μ_J ≠ μ_C**, indicating that **Jordan’s** and **Chamberlain’s** average scores differ.  
    - **Three Possible Hypothesis Structures include:**  
        - **Two-Tailed Test:**  
            - **H₀:** μ_J = μ_C  
            - **Hₐ:** μ_J ≠ μ_C  
        - **One-Tailed Test (Greater Than):**  
            - **H₀:** μ_J ≥ μ_C  
            - **Hₐ:** μ_J < μ_C  
        - **One-Tailed Test (Less Than):**  
            - **H₀:** μ_J ≤ μ_C  
            - **Hₐ:** μ_J > μ_C  
    - **Selection of Test Type** depends on the **Research Question** or **Expectation** regarding the relationship between the two means.  

</div><div style="text-align:center;">
    <img src="/images/M102.jpg">
</div></div>

### Topic03 - Other Projects

<div style="display:grid; grid-template-columns: 6fr 4fr;"><div markdown="1" style="min-width:0;">

- **Main Ideas:**
    - **Comparison of Means** helps determine whether performance differences between two subjects are **Statistically Significant** or due to **Random Chance**.

- **Core Notes:**  
    - **Average Comparison** involves evaluating the **Difference Between Mean Values** of two groups.  
    - **Numerical Example:**  
        - **Michael Jordan’s Average:** 30.12 points.  
        - **Wilt Chamberlain’s Average:** 30.06 points.  
        - The observed difference is small, requiring **Hypothesis Testing** to verify its **Statistical Relevance**.  
    - **Interpretation of Results:**  
        - If the **Null Hypothesis** is rejected, it implies a **Statistically Significant Difference** between the two averages.  
        - If not rejected, the **Observed Difference** could be due to **Random Variation**.  

</div><div style="text-align:center;">
    <img src="/images/M104.jpg">
</div></div>
