# Titanic Data Analysis

**Project Overview:**

This project delves into the tragic Titanic disaster by analyzing the factors that contributed to passenger survival. It leverages the power of data science to uncover insights and build a predictive model using logistic regression.

**Data:**

The analysis is based on the "titanic.csv" file, which contains a wealth of information about the passengers on board, including:

* **Pclass:** Passenger class (1st, 2nd, or 3rd)
* **Sex:** Gender (male or female)
* **Age:** Age in years
* **SibSp:** Number of siblings/spouses aboard
* **Parch:** Number of parents/children aboard
* **Fare:** Ticket fare
* **Embarked:** Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
* **Survived:** Whether the passenger survived (0 = No, 1 = Yes)

**Methodology:**

The project follows a structured approach:

1. **Data Loading and Exploration:** The Titanic dataset is loaded and explored using descriptive statistics and visualizations to understand its structure and identify potential patterns.
2. **Data Cleaning and Preprocessing:** Missing values are handled (e.g., age imputation), categorical variables are encoded (e.g., sex, embarked), and relevant features are selected for analysis.
3. **Exploratory Data Analysis (EDA):**  The data is visually analyzed to reveal relationships between variables and their impact on survival. This includes analyzing survival rates by passenger class, gender, age, and other factors.
4. **Feature Engineering:** New features are created or transformed to potentially improve the model's predictive power.
5. **Model Building:** A logistic regression model is trained to predict passenger survival based on the available features.
6. **Model Evaluation:** The model's performance is assessed using metrics such as accuracy, precision, recall, and an F1-score. The classification report is used to understand the model's strengths and weaknesses in predicting different classes.

**Key Findings:**

* **Socioeconomic Status:** Passengers in higher classes (1st and 2nd) had a significantly higher survival rate than those in 3rd class.
* **Gender:** Women were much more likely to survive than men, highlighting the "women and children first" protocol.
* **Age:** Children had a higher survival rate, while the elderly were less likely to survive.
* **Fare:**  The fare paid correlated with survival, suggesting those who paid more had better access to lifeboats or were in safer areas of the ship.

**Model Performance:**

The logistic regression model achieved the following performance metrics:

|                    | precision| recall | f1-score | support |
|--------------------|----------|--------|----------|---------|
| 0 (Did Not Survive)| 0.83     | 0.90   | 0.86     | 163     |
| 1 (Survived)       | 0.82     | 0.71   | 0.76     | 104     |

* **Accuracy:** 0.83
* **Overall Interpretation:** The model performs well, especially in predicting non-survival, but has some room for improvement in predicting survival cases.

**File Structure:**

* `titanic.csv`: The dataset used for the analysis.
* `titanic_analysis.ipynb`: Jupyter Notebook containing the complete code for data preprocessing, analysis, and modeling.
* `README.md`: This file, providing project details.

**How to Run the Analysis:**

1. **Clone the Repository:** `git clone https://github.com/brucelee31072004/titanic-data-analysis.git`
2. **Install Libraries:** `pip install pandas numpy matplotlib seaborn scikit-learn`
3. **Open and Run:** Open the `titanic_analysis.ipynb` notebook in Jupyter and execute the cells to reproduce the analysis and model results.

**License:**

This project is licensed under the MIT License - see the LICENSE file for details.

**Contributing:**
Feel free to contribute to this project by submitting issues, suggesting improvements, or proposing new analyses!
