**PROJECT OVERVIEW**
This project applies supervised machine learning algorithms, Logistic Regression and Random Forest to predict the probability of clients subscribing for a term deposit.

**Objective**
To build a realiable prediction model which helps identify clients that are more likely to subscribe to a bank term deposit, thereby enabling efficient decision making and targeted marketing.

**KEY STEPS AND TECHNIQUES**
1. **Data Cleaning**:
a)Handled missing values using mode imputation and
b)Removed columns that had over 50% of missing values to retain data quality.

 2.**Feature engineering**: 
 Created two new features to the dataset
a)**recency_bucket**: categories how recently a client was contacted, thus indicating how warm a lead is.
b) **age_group**: categories client data by age, capturing age-specific client behaviour.

3. **Exploratory Data Analysis (EDA)**: Generated basic statistics and visualisations to understand the key relationships and patterns of the dataset.

4. **Model Training and Evaluation**: Built and trained Random Forest and Logistric Regression models, compared their performances using precison. accuracy, recall, F1, ROC-AUC metrics. These metrics helped me determine which model performed better for the prediction task.

5.**Results**
Both models were trained and evaluated on an 80:20 split of the dataseta and although both achieved high accuracy due to class imbalance, the Random Forest model demonstrated a stronger overall performance.
**Key Findings**
**Accuracy**:Both models achieved ~89% accuracy, but this metric was less meaningful because most clients did not subscribe to the term deposit.

**Precision**:Moderate for both models (0.62–0.65), indicating reasonable correctness in the positive predictions made.

**Recall**:Random Forest identified more actual subscribers (0.2439) compared to Logistic Regression (0.1767), making it more effective for detecting the positive class.

**F1 & ROC-AUC**: Random Forest outperformed Logistic Regression on both F1-score and ROC-AUC, indicating better ranking ability and balanced performance.

**Training Time**: Logistic Regression trained significantly faster (~0.64s), while Random Forest required longer time (~13.6s) due to its ensemble structure.
