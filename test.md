---
layout: page
permalink: /DS09M3/
---

## M3 - Probability Distributions
- **01 - Random Numbers and Probability Distributions**
- **02 - State your Hypothesis**
- **03 - Normal Distribution**
- **04 - T distribution**
- **05 - Probability of Getting a High or Low Teaching Evaluation**

## 01 - Random Numbers and Probability Distributions

### 🎯 Objectives
- **Topic01** - Fundamental Concepts of **Probability** and **Random Variables**  
- **Topic02** - Structure and Interpretation of **Probability Distributions**  
- **Topic03** - Application of **Cumulative Distribution Function (CDF)**  
- **Topic04** - Modeling with **Normal Distribution** using **Mean** and **Standard Deviation**

### Topic01 - Fundamental Concepts of Probability and Random Variables
- **Main Ideas:**
    - **Probability** quantifies the likelihood of an event occurring within a range from 0 to 1.
    - **Random Variables** represent numerical outcomes dependent on random events in a defined **Probability Space**.

- **Core Notes:**  
    - **Probability** measures the **Likelihood** of an event occurring, expressed as a value between **0** and **1**.  
        - Example: The **Chance of Rain** being **45%** corresponds to a **Probability Value** of **0.45**.  
    - **Random Variable** defines a quantity whose **Possible Values** depend on **Random Events**.  
        - It functions as a **Mapping** from outcomes to values within a **Probability Space**.  
    - **Probability Space** includes all **Possible Outcomes** of a random experiment.  
        - Example: For one die, there are **6 Possible Outcomes** (1 to 6).  
        - Example: For two dice, there are **36 Possible Outcomes** (6 × 6).  

### Topic02 - Structure and Interpretation of Probability Distributions
- **Main Ideas:**
    - **Probability Distribution** models all potential values a **Random Variable** may assume along with their corresponding **Probabilities**.

- **Core Notes:**  
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

### Topic03 - Application of Cumulative Distribution Function (CDF)
- **Main Ideas:**
    - **Cumulative Distribution Function (CDF)** measures the **Probability** that a random variable takes a value **Less Than or Equal To** a specified number.

- **Core Notes:**  
    - **CDF** aggregates **Individual Probabilities** up to a specific **Value Threshold**.  
        - Example: **Probability of Getting ≤ 6** equals **0.417**, while **≥ 6** equals **0.58**.  
    - **CDF Graphs** visualize cumulative probabilities across all outcomes, showing how **Probabilities Accumulate** to **1**.  

### Topic04 - Modeling with Normal Distribution using Mean and Standard Deviation
- **Main Ideas:**
    - **Normal Distribution** describes continuous random variables characterized by **Mean** and **Standard Deviation**.

- **Core Notes:**  
    - **Normal Distribution** provides a **Theoretical Model** for real-world continuous data.  
        - Example: A **Histogram of Age** can be fitted with a **Normal Curve**.  
    - **Parameters of Normal Distribution:**  
        - **Mean (μ)** represents the **Central Value** (example: **48.37 years**).  
        - **Standard Deviation (σ)** measures **Dispersion** (example: **9.8 years**).  
    - **Fitting a Normal Curve** aligns **Empirical Data** with a **Theoretical Probability Model**.  

### 📌 Takeaways
- **Probability** quantifies uncertainty as a numerical measure between **0** and **1**.  
- **Random Variables** translate random outcomes into measurable quantities within a **Probability Space**.  
- **Probability Distributions** illustrate the structure of possible outcomes and their likelihoods.  
- **Cumulative Distribution Function** accumulates probabilities up to a defined threshold, forming the foundation for further statistical analysis.  
- **Normal Distribution** models real-world continuous data using **Mean** and **Standard Deviation** to describe central tendency and variability.  

## 02 - State your Hypothesis

### 🎯 Objectives
- **Topic01** - Definition and Purpose of **Statistical Hypothesis Testing**  
- **Topic02** - Formulation of **Null Hypothesis (H₀)** and **Alternative Hypothesis (Hₐ)**  
- **Topic03** - Comparison of **Mean Scores** between Two Entities  

### Topic01 - Definition and Purpose of Statistical Hypothesis Testing
- **Main Ideas:**
    - **Statistical Hypothesis Testing** is used to compare the **Averages** or **Means** of two entities to determine if a significant difference exists.

- **Core Notes:**  
    - **Hypothesis Testing** provides a framework to test whether observed differences between two **Sample Means** are due to **Random Variation** or a **True Difference**.  
    - Example: Comparing **Average Points per Game** between **Michael Jordan** and **Wilt Chamberlain**.  
    - **Michael Jordan** averaged **30.12 Points per Game**, while **Wilt Chamberlain** averaged **30.06 Points per Game**.  
    - Despite the similarity of these averages, a **Formal Statistical Test** is required to evaluate if the difference is **Statistically Significant**.  

### Topic02 - Formulation of Null Hypothesis (H₀) and Alternative Hypothesis (Hₐ)
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

### Topic03 - Comparison of Mean Scores between Two Entities
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

### 📌 Takeaways
- **Hypothesis Testing** enables systematic comparison between two **Population Means**.  
- **Null Hypothesis (H₀)** assumes equality between the means, while **Alternative Hypothesis (Hₐ)** posits inequality or directional difference.  
- **Michael Jordan** and **Wilt Chamberlain** serve as an example to illustrate hypothesis structures for comparing **Average Scores**.  
- **Three Hypothesis Scenarios** include equal, greater than, and less than comparisons, forming the basis for **Two-Tailed** and **One-Tailed Tests**.  
- **Statistical Analysis** determines whether the observed difference in means reflects a real effect or random variation.  

## 03 - Normal Distribution

### 🎯 Objectives
- **Topic01** - Definition and Characteristics of **Normal Distribution**  
- **Topic02** - Mathematical Representation of **Normal Distribution Function**  
- **Topic03** - Concept and Derivation of **Standard Normal Distribution**  
- **Topic04** - Generation of **Normal Curve** Using **Python Libraries**

### Topic01 - Definition and Characteristics of Normal Distribution
- **Main Ideas:**
    - **Normal Distribution** is one of the most widely used statistical distributions, represented by a **Bell-Shaped Curve**.

- **Core Notes:**  
    - **Normal Distribution** forms the foundation of many **Statistical Analyses** and **Real-World Applications**.  
    - **Bell-Shaped Curve** represents the **Symmetry** and **Central Tendency** of data.  
    - A large body of **Academic**, **Scholarly**, and **Professional Work** assumes that data follows a **Normal Distribution**.  
    - The curve visually depicts how **Data Points** are distributed around the **Mean**.  

### Topic02 - Mathematical Representation of Normal Distribution Function
- **Main Ideas:**
    - **Normal Distribution Function** mathematically expresses how probabilities are distributed across values of a **Random Variable**.

- **Core Notes:**  
    - **Formula Structure:**  
        - \( f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}} \)  
    - **Parameters of the Function:**  
        - **x:** Random Variable representing data values.  
        - **μ (Mu):** Mean of the distribution, derived from data.  
        - **σ (Sigma):** Standard Deviation representing data spread.  
    - **Constant Terms:**  
        - **π (Pi):** 3.142 or 22/7.  
        - **Exponential Function (e):** Represents continuous probability decay.  
    - **Key Components:**  
        - The **Exponent Term** \(-(x - μ)^2 / (2σ^2)\) defines how probabilities decrease symmetrically around the mean.  
        - The **Denominator Term** \(\sigma \sqrt{2\pi}\) ensures the total probability equals 1.  
    - Example: When **μ** and **σ** are obtained from actual data, the resulting curve models that dataset’s **Probability Distribution**.  

### Topic03 - Concept and Derivation of Standard Normal Distribution
- **Main Ideas:**
    - **Standard Normal Distribution** is a special case of the **Normal Distribution** with **Mean = 0** and **Standard Deviation = 1**.

- **Core Notes:**  
    - **Transformation:** By substituting **μ = 0** and **σ = 1**, the general normal distribution simplifies to:  
        - \( f(x) = \frac{1}{\sqrt{2\pi}} e^{-\frac{x^2}{2}} \)  
    - **Simplification Steps:**  
        - **μ = 0** removes the mean adjustment (x - μ → x).  
        - **σ = 1** simplifies the scaling factors since multiplying or dividing by 1 has no effect.  
    - **Purpose:** Establishes a **Universal Reference Distribution** used for **Z-Scores** and **Standardization** in statistics.  
    - Example: When **x** varies from **-4 to 4**, substituting these values generates the **Standard Normal Bell Curve**.  

### Topic04 - Generation of Normal Curve Using Python Libraries
- **Main Ideas:**
    - **Python Libraries** can be used to simulate and visualize the **Standard Normal Distribution**.

- **Core Notes:**  
    - **Python Libraries Used:**  
        - **Matplotlib:** for generating graphical visualizations.  
        - **NumPy:** for numerical operations and creating data arrays.  
        - **SciPy.stats:** for accessing the **norm.pdf** function that computes **Probability Density Values**.  
    - **Implementation Steps:**  
        - Use **x-values** from **-4 to 4** in increments of **0.1**.  
        - Compute **Probability Density** using the **norm.pdf** function.  
        - Plot results with **Matplotlib** to generate the **Standard Normal Curve**.  
    - Example: The generated plot visually represents the **Bell-Shaped Curve** associated with the **Standard Normal Distribution**.  

### 📌 Takeaways
- **Normal Distribution** underpins a vast range of **Statistical Models** and **Real-World Data Analyses**.  
- **Mathematical Formulation** uses parameters **Mean (μ)** and **Standard Deviation (σ)** to define the curve’s shape.  
- **Standard Normal Distribution** serves as a simplified reference with **μ = 0** and **σ = 1**.  
- **Python Libraries** such as **NumPy**, **Matplotlib**, and **SciPy.stats** allow efficient generation and visualization of the **Normal Curve**.  
- **Bell-Shaped Curve** symbolizes data symmetry and the natural clustering of observations around the mean.  

## 04 - T distribution
## 05 - Probability of Getting a High or Low Teaching Evaluation
