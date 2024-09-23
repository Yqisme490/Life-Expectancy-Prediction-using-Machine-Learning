# Life Expectancy Prediction using Machine Learning
**Overview**

This project aims to predict life expectancy using various machine learning techniques. Starting with Linear Regression as the baseline model, we progressively enhance the model by implementing Polynomial Regression, Feature Scaling, and Regularization techniques. The model was trained and validated on a dataset containing life expectancy and health-related attributes from various countries.

**Key Features:**

* **Exploratory Data Analysis (EDA):** Analyzed the distribution, relationships, and correlations of the features with life expectancy.
* **Baseline Model:** Used Linear Regression as the starting model to predict life expectancy.
* **Polynomial Regression:** Improved the model to capture non-linear relationships.
* **Feature Scaling and Normalization:** Applied to reduce the effect of outliers and improve model performance.
* **Ridge Regularization (L2):** Applied to mitigate overfitting and multicollinearity.
* **Model Evaluation:** Performance metrics such as R² Score and Mean Squared Error (MSE) were used to evaluate model performance.

**Dataset**

* The dataset contains health indicators such as Adult Mortality, HIV-AIDS, GDP, and Schooling, among others, for predicting life expectancy.
* Target Variable: Life Expectancy.
* Predictors: Various health and socio-economic features.

**Methodology**

1. **Exploratory Data Analysis (EDA):**

* Identified key relationships between predictors and the target variable (life expectancy).
* Addressed class imbalance and outliers, and analyzed linear and non-linear relationships.
2. **Baseline Model:**

* A simple Linear Regression model was implemented as the baseline, achieving an R² score of 0.75 and MSE of 20.97.
  * ![image](https://github.com/user-attachments/assets/2e68f7ef-210a-4f35-8568-68c3fa05c773)
* The model's residuals had a mean close to 0, indicating decent performance but room for improvement.

3. **Feature Removal:**
* Removed unimportant variables such as Population, Country, and Thinness5-9years based on their low impact on life expectancy.

4. **Polynomial Regression:**

* Fitted a 2nd-degree Polynomial Regression to better capture non-linear relationships, which improved the R² score to 0.79.

5. **Feature Scaling and Normalization:**

* Applied to all predictors and observed a slight performance improvement, especially after scaling highly skewed variables.
  * ![image](https://github.com/user-attachments/assets/c38ac00f-d00c-441c-8a8c-fefb2677d9a3)


6. **Regularization (Ridge Regression):**

* Added L2 regularization to reduce overfitting and improve generalization, resulting in an R² score of 0.84 and a lower MSE of 13.30.
  * ![image](https://github.com/user-attachments/assets/3e4c57ff-a858-4c98-a522-6a319b4f67e0)
  * ![image](https://github.com/user-attachments/assets/146c14e9-5fcc-459f-aba8-e6ddf4bfe025)

**Results**

* Baseline Model: R² = 0.75, MSE = 20.97.
* Polynomial Regression (Scaled): R² = 0.79, MSE = 17.35.
* Polynomial Ridge Regression (Final Model): R² = 0.84, MSE = 13.30.
* The final model significantly improved prediction accuracy and reduced errors compared to the baseline model.

**Technology Stack**
* Python
* Scikit-learn
* Pandas
* Matplotlib / Seaborn (for visualizations)
