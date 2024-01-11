# Vodafone's Crystal Ball : A Machine Learning Approach to Analyze Customer Churn



## Table of Content 
- [Project Description](#project-description)
- [Data sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Cleaning/Preparation](#data-cleaning)

- [Exporatory Data Analysis](#exporatory-data-analysis)
- [Results/Findings](#results)
- [Recommendation](#recommendation)
- [Reference](#reference)
  
## Project Description
The goal of this project is to develop a supervised machine learning model to analyze customer attrition within the Vodafone telecom company. The model will utilize any provided dataset to generate new observations by accurately determining whether a customer is likely to churn or not. This initiative aims to provide valuable insights into customer behavior, enabling the identification of potential churn and facilitating strategic interventions to retain customers effectively. The outcome of the project will contribute to a more informed and proactive approach to customer relationship management within Vodafone.
## Data sources 
Thanks to Azubi Africa for providing me with access to this dataset. The data for this project was divided into three distinct parts.
The initial dataset was stored in a Microsoft SQL Server. I established a remote connection to it using the **pyodbc** library.
The second dataset for this project was sourced from a GitHub repository and was formatted as a CSV file.
The third dataset, intended to serve as the test dataset, was found on OneDrive, also in CSV format.

  ## Tools Used
Tools Used in the Project:
#### Programming Language:
- Python
#### Integrated Development Environment (IDE):
 - VSCode: A general-purpose IDE with robust support for Python development.
#### Libraries and Frameworks:
- scikit-learn 
- Pandas
- NumPy
#### Data Visualization:
- Matplotlib
- Seaborn
#### Version Control:
- Git: Essential for version control, collaboration, and tracking changes in code.
### The data set includes information about:

* Customers who left within the company  — the column is called Churn.
* Services that each customer has signed up for — phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
* Customer account information — how long they’ve been a customer (Tenure ), contract, payment method, paperless billing, monthly charges, and total charges
* Demographic info about customers — gender, age range, and if they have partners and dependents
Demographics
CustomerID: A unique ID that identifies each customer.
* Senior Citizen: Indicates if the customer is older: Yes, No
* Dependents: Indicates if the customer lives with any dependents: Yes, No. Dependents could be children, parents, grandparents, etc.
* Tenure in Months: Indicates the total amount of months that the customer has been with the company 
* total charges is  equal to each tenue times monthly charges.
* Multiple Lines: Indicates if the customer subscribes to multiple telephone lines with the company: Yes, No
  #### Data Cleaning/Preparation
  1. **Clean the Data:**
   - Fix issues like missing values and incorrect data types in the dataset.
   - Use Simple Imputer to fill in missing values and correct data types.

2. **Create a Pipeline:**
   - Set up a systematic process (pipeline) to automatically apply the same corrections to new datasets.

3. **Prepare for Machine Learning:**
   - Convert categorical data to numerical format using OneHot Encoder and Label Encoder for efficient machine learning model training.

     #### Model  Selection & Evaluation
     Step 1: Data Preparation

- Split the data into training and evaluation sets, allocating 80% for training and the remaining for evaluation.

Step 2: Model Training
- Train five machine-learning models: RandomForest, DecisionTree, GradientBoosting, KNN, and SupportVector classifiers.

Step 3: Dataset Balancing and Optimization
- Address the imbalanced target column using both RandomSampler and SMOTE, with SMOTE showing better performance.
- Implement feature selection to enhance model performance.
- Conduct hyperparameter tuning using RandomizedSearchCV.

Step 4: Model Evaluation
- Assess the model's performance using the f1-score metric.
- Evaluate the AUC-ROC curve to visually summarize the models' ability to distinguish between classes.
- Plot the ROC curve for each model with their respective AUC scores to analyze performance.

  #### Results
  The GradientBoosting classifier emerged as the top-performing model after modeling and hyperparameter optimization. It predicted 591 customers as likely to churn and 1409 as unlikely to churn. The company should focus on reaching out to the 591 predicted churners, implementing measures to retain them, crucial for maximizing revenue in the upcoming financial year.

  
     
