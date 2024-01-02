# Vodafone's Crystal Ball : A Machine Learning Approach to Analyze Customer Churn

## Business Understanding
This project aims to analyze and predict customer churn in Vodafone, a telecom organization. The primary goal is to develop a robust churn prediction model to identify customers likely to leave and understand the reasons behind churn. The dataset is divided into three parts: train dataset, evaluation dataset, and test dataset.

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

 
