# **𝐋𝐨𝐚𝐧 𝐄𝐥𝐢𝐠𝐢𝐛𝐢𝐥𝐢𝐭𝐲 𝐏𝐫𝐞𝐝𝐢𝐜𝐭𝐢𝐨𝐧**

**Analytical Platform:**
*The project was built using the standard Python data science ecosystem. Key technologies included Pandas and NumPy for data handling, the Scikit-learn library for all machine learning tasks, and Matplotlib/Seaborn for data visualization.*

**Data Ingestion:**
*The project began by ingesting the Loan Eligibility Prediction.csv dataset. This step included quickly assessing data integrity, confirming no missing values, and prepping the raw features for the subsequent exploratory phase.*

**Initial Data Overview:**
*Initial checks confirmed the presence of 13 key features, including demographic, income, and loan-specific details. Categorical features like Gender, Married, and Property_Area were identified as critical inputs for the predictive models.*

**EDA**

**Univariate Analysis & Visualization:**
*Examined the distribution and frequency of individual variables, such as Applicant_Income and the highly imbalanced target variable, Loan_Status. Visualizations confirmed the need for careful feature scaling and classification metric choice.*

**Bivariate Analysis & Visualization:**
*Focused on the relationship between pairs of features and the target. A key finding was the strong correlation between Credit_History (1) and loan approval, which proved to be the single most influential factor in eligibility.*

**Multivariate Analysis & Visualization:**
*Explored complex relationships, such as the impact of Applicant_Income and Coapplicant_Income combined across different Property_Area types. This step provided a richer understanding of how multiple variables interact to influence loan outcomes.*

**Machine Learning**

**Classification Task / X_Encoded / Regression Task:**
*The project defined a dual objective: a Classification Task to predict Loan_Status (Y/N) and a Regression Task to predict Loan_Amount. All categorical features were successfully transformed using encoding methods (X_Encoded) for model readiness.*

**Classification Model Training and F1 Score Evaluation:**
*A classification model was trained to predict loan eligibility. Evaluation utilized the F1 Score—a critical metric for balanced assessment—due to the observed class imbalance in the target variable, ensuring reliable performance reporting.*

**Train and Evaluate Regression Model 1 (Linear Regression):**
*The first model provided a baseline understanding of linearity in predicting Loan Amount. It was evaluated using standard metrics like $R^2$ and error terms (MAE, MSE, RMSE) to establish its predictive power against the dataset features.*

**Train and Evaluate Regression Model 2 (Random Forest Regressor):**
*The Random Forest model was trained to capture complex, non-linear feature interactions in the data. This model inherently handles feature importance and provides a robust benchmark against the simpler linear model.*

**Train and Evaluate Regression Model 3 (Gradient Boosting Regressor):**
*The final regression model leveraged the power of boosting to sequentially correct prediction errors. This model is often highly performant in predictive tasks and provided the final, high-performance ceiling for comparison.*

**Compare Regression Models and Identify the Best:**
*A comprehensive analysis of all three models showed that Linear Regression surprisingly yielded the best fit. This model was selected as optimal due to its superior performance metrics across the board.*

**Best Regression Model Identification:**
*Linear Regression was identified as the best performing model, achieving the highest R-squared value of $0.4122$ and the lowest error metrics (MAE, MSE, RMSE). Its simplicity combined with the highest explained variance makes it the most favorable choice.*

**Summary:**
*The project successfully delivered strong predictive models for both loan eligibility and loan amount. Key takeaways included the dominance of Credit History in classification and the surprising efficacy of the Linear Regression model in predicting loan amount.*
