# Child Mind Institute - Problematic Internet Usage

**Project Overview:**
In today’s digital age, excessive internet use among children and adolescents has emerged as a pressing concern. The phenomenon is closely linked to mental health challenges, including anxiety and depression. Recognizing the need for early identification and intervention, this project focuses on predicting problematic internet usage using physical activity and behavioral data. Leveraging data from the **Healthy Brain Network (HBN)**, the objective was to create a machine learning model capable of predicting the **Severity Impairment Index (SII)**, a metric that quantifies internet usage-related challenges.

**Dataset Description:**
The dataset, curated by the **Healthy Brain Network**, includes clinical and behavioral data from over 5,000 participants aged 5 to 22. The dataset captures a wide array of features, which are grouped as follows:

- **Demographics:** Basic information about participants, including age and sex.
- **Internet Use Behavior:** Details such as daily hours spent online or on digital devices.
- **Clinical Assessments:** Metrics like the **Children’s Global Assessment Scale (CGAS)**, a numeric scale used by mental health professionals to rate psychological and social functioning.
- **Physical Activity Patterns:** Information about the physical activity levels of participants, which can serve as a predictor for digital behavior.

**Methodology:**
The project followed a structured approach to data preprocessing, exploratory data analysis, feature engineering, and model building. Below are the major steps:

1. **Data Cleaning and Preprocessing:**
   - Missing values were handled using imputation techniques suitable for both numerical and categorical data.
   - Outliers in internet usage hours and CGAS scores were identified and appropriately treated.
   - Data was normalized to ensure uniformity across different feature scales.

2. **Exploratory Data Analysis (EDA):**
   - Visualized the distribution of SII scores across age and gender groups.
   - Analyzed correlations between physical activity levels, internet usage, and mental health indicators.
   - Identified patterns suggesting a link between sedentary behavior and high SII scores.

3. **Feature Engineering:**
   - Created derived features, such as screen time per age group and activity-to-screen time ratios.
   - Encoded categorical variables using label encoding and one-hot encoding techniques.

4. **Model Building:**
   - A variety of supervised machine learning models were employed, including:
     - **Logistic Regression**
     - **Random Forest Classifier**
     - **Gradient Boosting Machines (GBM)**
     - **XGBoost**
   - The models were evaluated using metrics like accuracy, precision, recall, F1-score, and ROC-AUC to ensure robust performance.

5. **Hyperparameter Tuning:**
   - Grid search and randomized search techniques were utilized to optimize model parameters, improving predictive accuracy and generalizability.

6. **Validation and Testing:**
   - The dataset was split into training and testing sets using an 80:20 ratio.
   - K-fold cross-validation was applied to mitigate overfitting and assess model stability.

**Key Results:**
- The best-performing model achieved an accuracy of over **85%** in predicting the Severity Impairment Index (SII).
- Significant predictors included hours of daily internet usage, CGAS scores, and age.
- Models demonstrated strong consistency across validation folds, indicating reliability.

**Challenges and Solutions:**
- **Imbalanced Data:** The dataset exhibited an unequal distribution of SII scores across classes. This was addressed using SMOTE (Synthetic Minority Over-sampling Technique) to balance the classes.
- **Feature Correlation:** High correlation among certain features posed multicollinearity challenges, which were mitigated by feature selection and dimensionality reduction techniques like PCA.

**Impact:**
This project contributes to the growing body of research aimed at understanding the behavioral and clinical factors associated with excessive internet use. By accurately predicting SII scores, the model can:

- Aid mental health professionals in identifying at-risk individuals early.
- Support targeted interventions to promote healthier internet usage habits.
- Provide valuable insights for policymakers and educators to develop awareness campaigns.

**Tools and Technologies Used:**
- **Programming Languages:** Python (pandas, NumPy, scikit-learn, Matplotlib, Seaborn, XGBoost)
- **Libraries for Preprocessing and Modeling:** Scikit-learn, imbalanced-learn (SMOTE), XGBoost
- **Visualization Tools:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

**Future Scope:**
- Expand the model to incorporate additional behavioral and environmental factors, such as family dynamics or academic performance.
- Explore the use of deep learning models to capture complex patterns in the data.
- Collaborate with educational institutions to deploy the model in real-world settings for validation and refinement.

**Conclusion:**
This project underscores the potential of data science to address pressing societal issues. By analyzing behavioral patterns and clinical metrics, we can take meaningful steps toward mitigating the adverse effects of excessive internet use among children and adolescents. The insights and tools developed here pave the way for proactive measures to ensure better mental health outcomes in the digital era.

