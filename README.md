# Customer-Demography

1. Introduction

Customer data analysis is essential for understanding purchasing behaviors, income distribution, and customer segmentation. In this report, we analyze a retail dataset, perform exploratory data analysis (EDA), preprocess data, and build a machine learning model to predict customer age groups.

2. Data Loading and Preprocessing
   
2.1 Loading the Dataset

The dataset is loaded using Pandas, and initial inspection is performed to check for missing values and data consistency.

2.2 Handling Missing Values

Any missing values in the dataset are identified and handled appropriately to ensure data integrity.
If missing values exist, strategies such as mean/mode imputation or removal of incomplete records are employed.

2.3 Creating Age Groups

To categorize customers based on age, we define the following age groups:
Young: Age < 30
Middle Age: 30 ≤ Age < 50
Senior: Age ≥ 50

2.4 Encoding Categorical Variables

Label encoding is used to convert categorical variables like occupation and income level into numerical values.
One-hot encoding is applied to categorical features to prepare them for machine learning models.

3. Exploratory Data Analysis (EDA)
   
3.1 Distribution of Income Levels

A bar chart is plotted to show the distribution of customers across different income levels.
This helps in identifying the most common income groups among customers.

3.2 Purchase Frequency by Age Group

A bar chart is generated to compare how frequently customers from different age groups make purchases.
Insights from this visualization can help in targeting specific age groups for marketing campaigns.

3.3 Favorite Product Category by Age Group

The favorite product category of each age group is visualized using a bar chart.
Helps in determining product preferences based on age segmentation.

3.4 Age Distribution Analysis

A histogram and boxplot are used to visualize the age distribution of customers.
Identifies key trends such as the average age, spread, and presence of outliers.

3.5 Filtering Specific Customer Groups

Engineers in the dataset are filtered and displayed to analyze their buying behavior.
Middle-aged customers are identified separately for further analysis.

4. Machine Learning Model for Age Group Prediction

4.1 Model Selection

A Random Forest Classifier is chosen for its ability to handle both categorical and numerical data efficiently.

4.2 Splitting the Data

The dataset is divided into training (80%) and testing (20%) sets.
The dependent variable is the age group, while independent variables include income level, occupation, and purchase frequency.

4.3 Model Training

The RandomForestClassifier is trained using the training dataset.
The model learns to predict the age group based on various customer attributes.

4.4 Model Evaluation

A classification report is generated, displaying key performance metrics:
Accuracy: Measures the overall correctness of the model.
Precision, Recall, and F1-Score: Provide insights into how well the model predicts each class.
Confusion Matrix: Helps in identifying misclassifications.

5. Predictions on New Customer Data

A new customer sample is created with specified attributes, and the trained model predicts their likely age group. This feature is useful for targeted marketing and customer segmentation strategies.

6. Conclusion

This analysis provides key insights into customer segmentation based on age, income, and purchasing behavior. The machine learning model effectively predicts customer age groups, which can aid businesses in making data-driven decisions. Future improvements can include fine-tuning hyperparameters, testing other classification models, and incorporating more features for enhanced accuracy.

7. Recommendations

Businesses should use targeted marketing strategies based on age group preferences.
Further data collection can improve model performance.
Implement real-time data analytics to track changing customer behaviors dynamically.
End of Report
