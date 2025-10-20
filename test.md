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

<div style="display:flex; grid-template-columns: 6fr 4fr;"><div style="flex:1; min-width:0;" markdown="1">

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

</div><div style="flex:1; min-width:0; text-align:center;"><br><img src="/images/DS01M101.jpg" style="max-width:100%; border-radius:10px;"></div></div>

### Topic02 - Structure and Interpretation of Probability Distributions

<div style="display:flex; grid-template-columns: 6fr 4fr;"><div style="flex:1; min-width:0;" markdown="1">

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

</div><div style="flex:1; min-width:0; text-align:center;"><br><img src="/images/DS01M102.jpg" style="max-width:100%; border-radius:10px;"></div></div>
  
### Topic03 - Application of Cumulative Distribution Function (CDF)

<div style="display:flex; grid-template-columns: 6fr 4fr;"><div style="flex:1; min-width:0;" markdown="1">

- **Main Ideas:**
    - **Cumulative Distribution Function (CDF)** measures the **Probability** that a random variable takes a value **Less Than or Equal To** a specified number.

- **Core Notes:**  
    - **CDF** aggregates **Individual Probabilities** up to a specific **Value Threshold**.  
        - Example: **Probability of Getting ≤ 6** equals **0.417**, while **≥ 6** equals **0.58**.  
    - **CDF Graphs** visualize cumulative probabilities across all outcomes, showing how **Probabilities Accumulate** to **1**.  

</div><div style="flex:1; min-width:0; text-align:center;"><br><img src="/images/DS01M103.jpg" style="max-width:100%; border-radius:10px;"></div></div>

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
- **Topic02** - Mathematical Formulation of **Normal Distribution Function**  
- **Topic03** - Concept and Simplification of **Standard Normal Distribution**  
- **Topic04** - Generation of **Normal Distribution Curve** Using **Python**

### Topic01 - Definition and Characteristics of Normal Distribution
- **Main Ideas:**
    - **Normal Distribution** is a fundamental concept in statistics, commonly used across academic, scholarly, and professional analyses.

- **Core Notes:**  
    - **Normal Distribution** represents how data points are distributed symmetrically around the **Mean**.  
    - The curve is **Bell-Shaped**, showing higher frequency near the **Mean** and tapering off symmetrically on both sides.  
    - Many **Statistical Models** assume that underlying data follows a **Normal Distribution**.  
    - The curve visually describes how **Random Variables** behave under normal conditions.  

### Topic02 - Mathematical Formulation of Normal Distribution Function
- **Main Ideas:**
    - **Normal Distribution Function** mathematically models the probability density of a random variable based on its **Mean** and **Standard Deviation**.

- **Core Notes:**  
    - The function is expressed as:  
        - $f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$  
    - **Parameters:**  
        - **x:** Random Variable (data point).  
        - **μ (Mu):** Mean, representing the central value of data.  
        - **σ (Sigma):** Standard Deviation, representing data spread.  
    - **Constants:**  
        - **π (Pi):** Approximated as 3.142 or 22/7.  
        - **e:** Exponential constant used for calculating continuous probability.  
    - **Interpretation of Components:**  
        - The **Exponent Term** $-\frac{(x-\mu)^2}{2\sigma^2}$ defines the shape and symmetry of the curve.  
        - The **Denominator** $\sigma \sqrt{2\pi}$ ensures total probability equals 1.  
    - Example: The **Mean** and **Standard Deviation** are derived from data, while **x** varies over possible values.  

### Topic03 - Concept and Simplification of Standard Normal Distribution
- **Main Ideas:**
    - **Standard Normal Distribution** is a special case of **Normal Distribution** with a **Mean (μ) = 0** and **Standard Deviation (σ) = 1**.

- **Core Notes:**  
    - When **μ = 0** and **σ = 1**, the equation simplifies to:  
        - $f(x) = \frac{1}{\sqrt{2\pi}} e^{-\frac{x^2}{2}}$  
    - **Simplification Process:**  
        - Replace **μ** with 0, making $(x - μ)$ become $x$.  
        - Replace **σ** with 1, removing its influence since multiplying or dividing by 1 has no effect.  
    - **Purpose:**  
        - Used to create a **Universal Distribution Model** for standardized variables.  
    - Example: When **x** ranges from -4 to 4, substituting these values generates the **Standard Normal Curve**.  

### Topic04 - Generation of Normal Distribution Curve Using Python
- **Main Ideas:**
    - **Python Libraries** can simulate and visualize the **Standard Normal Distribution Curve** effectively.

- **Core Notes:**  
    - **Tools Used:**  
        - **Matplotlib:** for graphical visualization.  
        - **NumPy:** for array creation and numerical computation.  
        - **SciPy.stats:** for probability density function using **norm.pdf**.  
    - **Implementation Details:**  
        - Define **x-values** between -4 and 4 using increments of 0.1.  
        - Calculate **Probability Density** using the **norm.pdf** function.  
        - Use **Matplotlib** to plot the **Standard Normal Curve**.  
    - Example: The generated **Bell Curve** represents data centered around a **Mean of 0** with a **Standard Deviation of 1**.  

### 📌 Takeaways
- **Normal Distribution** is foundational in both theoretical and applied statistics.  
- **Mathematical Representation** combines constants **π**, **e**, and parameters **μ**, **σ**, and **x**.  
- **Standard Normal Distribution** simplifies analysis by fixing **Mean = 0** and **Standard Deviation = 1**.  
- **Python Libraries** such as **NumPy**, **Matplotlib**, and **SciPy.stats** allow efficient visualization of the **Normal Curve**.  
- **Bell-Shaped Curve** illustrates how data symmetrically clusters around the **Mean**, representing natural variation.  

## 04 - T distribution

### 🎯 Objectives
- **Topic01** - Historical Background and Significance of **Student’s T-Distribution**  
- **Topic02** - Relationship Between **T-Distribution** and **Normal Distribution**  
- **Topic03** - Application of **T-Test** in Comparing Sample Means  
- **Topic04** - Assumptions and Implementation of **Independent Sample T-Test**  

### Topic01 - Historical Background and Significance of Student’s T-Distribution
- **Main Ideas:**
    - **Student’s T-Distribution** was developed by **William Sealy Gosset** and remains a cornerstone of inferential statistics, especially for small sample analysis.

- **Core Notes:**  
    - **William Sealy Gosset** published the **T-Distribution** in 1908 under the pseudonym **"Student"** in the journal **Biometrika**.  
    - He worked at **Guinness Brewery** in **Dublin, Ireland**, conducting experiments with **Small Samples of Barley**.  
    - **Employer Restrictions** prevented him from publishing under his real name.  
    - His contributions were later overshadowed by other statisticians such as **Ronald Fisher** and **Egon Pearson**, despite his foundational role.  
    - The book *The Cult of Statistical Significance* highlights **Gosset’s** influence and the evolution of **Statistical Significance Testing**.  

### Topic02 - Relationship Between T-Distribution and Normal Distribution
- **Main Ideas:**
    - **T-Distribution** describes the distribution of **Sample Means** drawn from a population, whereas **Normal Distribution** describes the **Population Mean** itself.

- **Core Notes:**  
    - **Normal Distribution:** Represents the **Population Mean** and assumes an **Infinite Sample Size**.  
    - **T-Distribution:** Represents the **Mean of Samples** drawn from the **Population** and accounts for **Sampling Variability**.  
    - The **Shape of the T-Distribution** depends on **Degrees of Freedom (df)**.  
        - When **df = 1**, the T-distribution is **Wider and Flatter** than the Normal Distribution.  
        - As **df Increases**, the **T-Distribution** becomes **More Similar** to the **Normal Distribution**.  
    - Example: When plotted, the **Normal Distribution Curve (Blue)** and **T-Distribution Curve** converge as the sample size grows.  

### Topic03 - Application of T-Test in Comparing Sample Means
- **Main Ideas:**
    - **T-Test** utilizes the **T-Distribution** to evaluate whether the means of two groups differ significantly.

- **Core Notes:**  
    - **T-Test** is a statistical method that relies on the **T-Distribution** to test **Differences in Means**.  
    - Example: A **Comparison of Teaching Evaluation Scores** for **Male** and **Female Instructors** at the **University of Texas**.  
        - **Blue Bar:** Represents **Female Instructors’ Average Scores**.  
        - **Orange Bar:** Represents **Male Instructors’ Average Scores**.  
        - Observation: Average score for females is slightly lower, approximately **4**, but the difference appears small.  
    - The **Research Question:** Is the difference in average evaluation scores **Statistically Significant**?  
    - **Null Hypothesis (H₀):** There is **No Difference** between male and female evaluation scores.  
    - **Alternative Hypothesis (Hₐ):** There **Is a Difference** between male and female evaluation scores.  
    - **Alpha Level (α):** Set at **0.05** to determine significance.  
    - If the **P-Value < 0.05**, the **Null Hypothesis is Rejected**, indicating a **Significant Difference** in scores based on gender.  

### Topic04 - Assumptions and Implementation of Independent Sample T-Test
- **Main Ideas:**
    - **T-Test Assumptions** ensure the validity of comparing means using the **T-Distribution**.

- **Core Notes:**  
    - **Assumptions Required for T-Test:**  
        - The **Measurement Scale** must be **Continuous** or **Ordinal**.  
        - The **Sample Data** must be **Randomly Selected** from the population.  
        - The **Data Distribution** should be **Approximately Normal**.  
        - **Homogeneity of Variance** must be satisfied to prevent bias toward larger samples.  
    - **Testing Procedure in Python:**  
        - Use the **`scipy.stats.ttest_ind()`** function from the **SciPy** library.  
        - Input: Two independent samples (e.g., **Female Evaluation Scores** and **Male Evaluation Scores**).  
        - Output: **T-Statistic** and **P-Value**.  
        - Example: If the returned **P-Value < 0.05**, conclude a **Statistical Difference** between the two groups.  

### 📌 Takeaways
- **Student’s T-Distribution** is crucial for analyzing small sample data and estimating population parameters.  
- **William Sealy Gosset**, under the pseudonym **Student**, pioneered the **T-Distribution**, shaping modern statistical inference.  
- **T-Distribution** approximates the **Normal Distribution** as **Degrees of Freedom** increase.  
- **T-Test** applies the **T-Distribution** to determine whether two sample means differ significantly.  
- **Assumptions** such as **Normality**, **Random Sampling**, and **Equal Variance** are essential for the accuracy of **T-Test Results**.  
- **Python’s SciPy Library** provides efficient implementation of **Independent Sample T-Tests** for empirical data analysis.  

## 05 - Probability of Getting a High or Low Teaching Evaluation

### 🎯 Objectives
- **Topic01** - Concept and Computation of **Standardization (Z-Score)**  
- **Topic02** - Determination of **Probability from Normal Distribution Tables**  
- **Topic03** - Calculation of **Probability for Specific Teaching Evaluation Scores**  
- **Topic04** - Implementation of **Probability Computation** Using **Python**

### Topic01 - Concept and Computation of Standardization (Z-Score)
- **Main Ideas:**
    - **Standardization** converts a variable into a **Z-Score** with a **Mean of 0** and a **Standard Deviation of 1**, allowing comparison within the **Normal Distribution**.

- **Core Notes:**  
    - **Standardization Formula:**  
        - $Z = \frac{X - \mu}{\sigma}$  
        - Where **X** is the raw score, **μ** is the mean, and **σ** is the standard deviation.  
    - Example: For a **Teaching Evaluation Score** of **4.5**,  
        - **Mean (μ)** = 3.998  
        - **Standard Deviation (σ)** = 0.554  
        - $Z = \frac{4.5 - 3.998}{0.554} = 0.906$  
    - **Z-Score Interpretation:**  
        - **Z = 0.906** represents how many **Standard Deviations** the score is above the mean.  
    - When standardized, data centers around a **Mean of 0** with most values between **-3** and **+3** on the **X-Axis**.

### Topic02 - Determination of Probability from Normal Distribution Tables
- **Main Ideas:**
    - **Standard Normal Tables** allow estimation of probabilities for a given **Z-Score** without computational tools.

- **Core Notes:**  
    - **Normal Distribution Table:** Lists **Cumulative Probabilities** corresponding to **Z-Scores**.  
    - Accuracy of the table is typically to **Two Decimal Places**.  
        - Example: **Z = 0.906** is rounded to **0.91**.  
    - For **Z = 0.91**, the **Cumulative Probability** is **0.8186**.  
    - **Graphical Representation:**  
        - The **Shaded Area Under the Curve** corresponds to the probability of obtaining a value **Less Than or Equal To** a given **Z**.  

### Topic03 - Calculation of Probability for Specific Teaching Evaluation Scores
- **Main Ideas:**
    - Probabilities can be computed for scores **Less Than** or **Greater Than** a specific value based on **Z-Score** and **Normal Distribution** properties.

- **Core Notes:**  
    - **Given Values:**  
        - Mean = 3.998, Standard Deviation = 0.554, and Score (X) = 4.5.  
    - **Probability of Score ≤ 4.5:**  
        - Using **Z = 0.906**, the **Probability** = 0.8186 or **81.76%**.  
        - Represented as the **Gray Shaded Area** under the **Normal Curve** to the left of **Z = 0.91**.  
    - **Probability of Score > 4.5:**  
        - Since the **Total Area Under the Curve = 1**,  
            - $P(X > 4.5) = 1 - 0.8176 = 0.1824$  
            - Equivalent to **18.24%**, represented by the **Right-Side Shaded Area**.  
    - **Relationship:**  
        - $P(X ≤ 4.5) + P(X > 4.5) = 1$.  

### Topic04 - Implementation of Probability Computation Using Python
- **Main Ideas:**
    - **Python** provides statistical functions to calculate probabilities directly from the **Normal Distribution**.

- **Core Notes:**  
    - **Library Used:** `scipy.stats`  
    - **Function:** `norm.cdf()` (Cumulative Distribution Function) computes the **Left-Side Probability**.  
        - Example: `norm.cdf(4.5, 3.998, 0.554)` returns **0.8176** for **P(X ≤ 4.5)**.  
    - To compute the **Right-Side Probability (P(X > 4.5))**, subtract the result from 1:  
        - $1 - P(X ≤ 4.5) = 0.1824$.  
    - **Output:** Confirms that **Probability of Evaluation > 4.5 = 18.24%**, consistent with manual calculation.  

### 📌 Takeaways
- **Standardization** transforms data into **Z-Scores** for comparison within the **Standard Normal Distribution**.  
- **Normal Tables** enable estimation of probabilities without computational tools, typically accurate to two decimal places.  
- **Probability of a Value** is represented as the **Area Under the Normal Curve**, summing to **1** for all outcomes.  
- **Python’s SciPy Library** simplifies probability computation using **norm.cdf()** for cumulative probabilities.  
- **Teaching Evaluation Example** demonstrates practical computation of probabilities for real-world datasets.  
