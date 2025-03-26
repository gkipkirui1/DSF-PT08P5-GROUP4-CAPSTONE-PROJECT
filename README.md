# 📌Building an Intelligent Fraud Detection System
![Fraud](https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT/blob/main/images/fraud1.jpg)

---

* Students name: 

* Student pace: Part Time

* Scheduled project review date/time: 

* Instructor name: Daniel Ekale &  Samuel Karu

* Github post URL: https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT

---

# 📌Project Overview 
---
According to INTERPOL (2024), fraud trends vary by region, with West and Southern Africa experiencing increased romance baiting scams, while Asia faces telecommunication fraud where criminals impersonate law enforcement or bank officials. Commercial banks and health insurers are the most affected financial institutions, with identity fraud accounting for 45% of reported cases in 2023 and projected to reach 50% by year-end (Retail Banker International, 2024). The growing use of technology has enabled sophisticated fraud schemes at lower costs, with scam-related frauds rising by 56% in 2024, surpassing digital payment fraud (PYMNTS, 2024). Scams now constitute 23% of fraudulent transactions, with relationship and product scams driving financial losses. In Kenya, financial fraud is escalating, exposing vulnerabilities in the banking sector (Kenyan Wall Street, 2024). A major case involved Kiwipay Kenya Limited, where Ksh2.3 billion ($19.48 million) was frozen due to suspected debit card fraud. The Central Bank of Kenya (CBK, 2025) attributes the surge in fraud to increased ICT adoption, low financial security awareness, and emerging cyber threats. Mobile and internet banking channels remain highly targeted, emphasizing the need for stronger security protocols and public education to combat digital financial fraud.

Kenya has experienced a massive shift to digital banking and mobile transactions, with platforms like M-Pesa, PesaLink, and internet banking becoming dominant. However, this digitization has also led to an increase in financial fraud cases, such as:

* ATM and Card Fraud: Criminals use card skimming devices to steal customer information.
* SIM Swap Fraud: Fraudsters gain control of a victim’s SIM card to access mobile banking accounts.
* Social Engineering Attacks: Scammers impersonate banks to trick customers into revealing sensitive information.
* Account Takeovers: Unauthorized individuals gain access to banking credentials and conduct fraudulent transactions.
  
In Kenya, several fraud cases have made headlines, including:

* KCB Bank SIM Swap Scam (2021) – Customers lost millions after fraudsters illegally swapped SIM cards to gain access to their mobile banking.
* Equity Bank Card Cloning (2022) – A group of criminals was arrested for skimming debit card details from unsuspecting users.
* M-Pesa Fraud Rings (2023) – Multiple fraud cases involved con artists deceiving individuals into sending money via M-Pesa through fake job offers and lottery scams.
  
To combat these threats, banks need an intelligent, adaptive fraud detection system that can identify fraudulent transactions in real time while minimizing false alarms.

# 📌Business Problem 
---
The Central Bank of Kenya (CBK) has highlighted key risk factors, including the rapid adoption of digital financial services, low consumer awareness of financial security, and emerging cyber threats that continue to evolve. Furthermore, scam-related frauds, identity theft, and card skimming have intensified, leading to substantial financial losses and undermining public trust in the financial sector. In response to these challenges, we aim to develop a robust fraud detection and prevention model that leverages advanced technologies such as machine learning, artificial intelligence, and real-time transaction monitoring. This model will enhance the ability of financial institutions in Kenya to detect fraudulent activities proactively, mitigate risks, and strengthen cybersecurity measures ensuring real-time fraud prevention and minimizing financial losses.

## 📌Project Objectives
---
The objective of this project is to develop a model to:

1. Analyse card transaction patterns with a view to detect fraud

2. Come up with a predictive models that can accurately classify transactions as fraudulent or legitimate

3. Study how demographics including age and gender impact fraud risks.

4. Identify peak fraud periods based on transactions date and transactions time.

5. Establish a model that can detect suspicious card frauds in real time

## 📌Target Audience
---
This project is designed for:

1. Banks and Financial Institutions classified as Tier one banks in Kenya, seeking to enhance their fraud prevention mechanisms.

2. Mobile Money Operators like Safaricom (M-Pesa), Airtel Money, and Telkom T-Kash looking to secure transactions from mobile fraudsters.

3. Regulatory Bodies and Government agencies, including the Central Bank of Kenya (CBK) and Communications Authority of Kenya, ensuring compliance with digital fraud policies.

4. Individual bank customers and corporate clients who require a secure and reliable banking system free from fraudulent activities.
   

# 📌Data Source and Description 
---
The data was sourced from https://www.kaggle.com/datasets/marusagar/bank-transaction-fraud-detection

The variables in the dataset are *Customer_ID*, *Customer_Name*, *Gender* , *Age* ,*State*, *City*, *Bank_Branch*, *Account_Type*, *Transaction_ID*, *Transaction_Date*, *Transaction_Time*, *Transaction_Amount*, *Merchant_ID*, *Transaction_Type*, *Merchant_Category*, *Account_Balance*, *Transaction_Device*, *Transaction_Location*, *Device_Type*, *Is_Fraud*, *Transaction_Currency*, *Customer_Contact*, *Transaction_Description* and *Customer_Email*. 

The numerical columns in the dataset are: ['Age', 'Transaction_Amount', 'Account_Balance', 'Is_Fraud']

The categorical columns in the dataset are: ['Customer_ID', 'Customer_Name', 'Gender', 'State', 'City', 'Bank_Branch', 'Account_Type', 'Transaction_ID', 'Transaction_Date', 'Transaction_Time', 'Merchant_ID', 'Transaction_Type', 'Merchant_Category', 'Transaction_Device', 'Transaction_Location', 'Device_Type', 'Transaction_Currency', 'Customer_Contact', 'Transaction_Description', 'Customer_Email']

# 📌Installations  

1. Clone the repository:  
   ```bash
   git clone git@github.com:gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT.git
 
2.Navigate to the project Directory  
  <pre><code>cd DSF-PT08P5-GROUP4-CAPSTONE-PROJECT</code></pre>
  

3.Install the required dependencies  
   <pre><code>pip install -r requirements.txt</code></pre>

# 📌Data Understanding and Preparation 
---
1. The dataset has 200000 rows and 24 columns.

2. The dataset has 2 columns with Float data type, 2 column with integer data type and 20 columns with categorical data types.

3. The Transaction_Date and Transaction_Time columns are indicated as object data type. For analysis and feature engineering processes, the data types for the two columns will be converted to Datetime format.

4. The Fraud Transaction dataset has no missing values.

5. The dataset has no duplicate rows.

5. The descriotive analysis of the categorical data was: 

    * The mean age, transaction amount and account Balance is 44 years, 49538 INR and 53437 INR respectively.
   
    * The standard deviation of the age transaction amount is 15 years, 28551 INR and 27399 INR respectively.
   
    * The minimum age and maximum age is 18 and 70 years.
  
# 📌 Vizualization
---
![Plot Showing distribution of the Class Feature(Fraud and Non Fraud Cases)](https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT/blob/main/images/Plot%20Showing%20distribution%20of%20the%20Class%20Feature(Fraud%20and%20Non%20Fraud%20Cases).png)

* For the class 0 indicating (Non-fraud cases) which is 94.956% of the data while for class 1 (fraud cases) 5.044% of the data. This shows existence of class imbalance that we need to address during modelling.

![Analysis of Fraud Cases by Gender.png](https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT/blob/main/images/Analysis%20of%20Fraud%20Cases%20by%20Gender.png)

* The distribution points to a slightly higher number of reported fraud cases affecting **males** as compared to **females**.

![Distribution of Fraud and Non Fraud Cases by Categorical Features.png](https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT/blob/main/images/Distribution%20of%20Fraud%20and%20Non%20Fraud%20Cases%20by%20Categorical%20Features.png)

* The count plot shows that there are more non-fraudulent transactions for both genders, but the proportion of fraudulent transactions is slightly higher among males compared to females. This suggests that gender may play a role in the likelihood of fraud, warranting further investigation into behavioral patterns.
* The line graph illustrates the fraud rate by age, indicating that the fraud rate tends to increase with age, peaking in the middle age range (around 40-50 years). This suggests that older customers may be more susceptible to fraud, which could be due to various factors such as financial literacy or exposure to fraud schemes.
* The distribution of fraudulent transactions across different devices is relatively equal, indicating that there may not be a significant difference in fraud occurrence based on the device used.

![Number of Fraudulent over time](https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT/blob/main/images/Analysis%20of%20Fraud%20Cases%20Over%20Time.png)

* Top 3 Peak Fraud Periods:
* 
Peak 1: Start = 2025-01-06 06:00:00, End = 2025-01-06 12:00:00, Count = 107

Peak 2: Start = 2025-01-29 00:00:00, End = 2025-01-29 06:00:00, Count = 106

Peak 3: Start = 2025-01-26 18:00:00, End = 2025-01-27 00:00:00, Count = 106

* Given that the dataset was sourced from India, we researched on what was unique during the peak fraud periods. We established that on 6/01/2025 was Guru Gobind Singh's Birthday, a holiday celebrated in some states in India. Similarly, 26/01/2025 was Republic Day (G); a national holiday in India. India also observed lunar new year on 29/01/2025, one of the most important celebrations of the year among East and Southeast Asian cultures.

![Distribution of Fraud and Non Fraud Cases by Numerical Features](https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT/blob/main/images/Distribution%20of%20Fraud%20and%20Non%20Fraud%20Cases%20by%20Numerical%20Features.png)

* The boxplots for numerical features by Is_Fraud indicate that there is no significant difference in the distributions of these features between fraudulent and non-fraudulent transactions. Both categories show similar ranges and medians, suggesting that the numerical features do not provide strong discriminatory power for identifying fraudulent transactions. This could imply that other factors, possibly categorical or behavioral, may be more relevant in predicting fraud.


![Correlation Matrix](https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT/blob/main/images/Correlation%20Analysis%20of%20Numerical%20Features.png)
The correlation matrix shows very weak linear relationships (correlation coefficients near zero) among variables, indicating minimal direct association. Most variables are linearly independent, suggesting that changes in one do not strongly affect others. This implies that non-linear patterns or additional feature engineering may be necessary for predictive modeling.

![Analysis of Transaction Amount Targeted by Fraud](https://github.com/gkipkirui1/DSF-PT08P5-GROUP4-CAPSTONE-PROJECT/blob/main/images/Analysis%20of%20Transaction%20Amount%20Targeted%20by%20Fraud)

* On the nalysis of Transaction Amount Targeted by Fraud a total transactions amount of 497.1157 Million Indian Rupees were reported to have been targetted by Fraud

# 📌Exploratory Data Analysis (EDA)
---
1. Univariate Analysis
     * For the class 0 indicating **(Non-fraud cases)** which is 94.956% of the data while for class 1 **(fraud cases)** 5.044% of the data.
     * The transaction type with the highest cases of fraud is: **Transfer**. 
     * The state with the highest fraud cases is: **Lakshadweep**.
     * The distribution points to a slightly higher number of reported fraud cases affecting **males** as compared to **females**.
     * The transaction device with the highest fraud cases is: **ATM Booth Kiosk** while the transaction device with the lowest fraud cases is: **POS Terminal**. 
     * The age distribution shows a more uniform spread, with a slight concentration in the **middle age range (around 30-50 years)**. This suggests that the bank's customer base is primarily composed of middle-aged individuals.

2. Bivariate Analysis
     * On the analysis on Analysis of Fraud Cases over Time the Peak Fraud Period: is between 2025-01-06 06:00:00 and 2025-01-06 12:00:00.
     * On the nalysis of Transaction Amount Targeted by Fraud a total transactions amount of 497.1157 Million Indian Rupees were reported to have been targetted by Fraud.
     * The boxplots for numerical features by Is_Fraud indicate that there is no significant difference in the distributions of these features between fraudulent and non-fraudulent transactions. Both categories show similar ranges and medians, suggesting that the numerical features do not provide strong discriminatory power for identifying fraudulent transactions. This could imply that other factors, possibly categorical or behavioral, may be more relevant in predicting fraud.
     * On Distribution of Fraud and Non Fraud Cases by Gender, Age, Account Type and Device Type:
       
         > There are more non-fraudulent transactions for both genders, but the proportion of fraudulent transactions is slightly higher among males compared to females. This suggests that gender may play a role in the likelihood of fraud, warranting further investigation into behavioral patterns.
       
         > In fraud rate by age, indicating that the fraud rate tends to increase with age, peaking in the middle age range (around 40-50 years). This suggests that older customers may be more susceptible to fraud, which could be due to various factors such as financial literacy or exposure to fraud schemes.
       
         > The distribution of fraudulent transactions across different devices is relatively equal, indicating that there may not be a significant difference in fraud occurrence based on the device used.
  
3. Multivariate Analysis
    * Visualization of Relationships Among Numerical Features Using Pairplot
    * Feature Correlation Analysis for Understanding Relationships

# 📌Data Preparation
---
In this step, we prepared our data for Modelling. The following steps were undertaken:

  * Remove Unnecessary columns which we deem less important for our modelling.
  * Data Transformation. This involved Standard Scaling and Label Encoding.
  * We also checked for outliers as skewed data may have an effect on our modelling process.
  * We will also handled class imbalance since our class feature is highly imbalanced.
  * First, we removed unnecessary columns from our dataframe because:
      > State and City since it has been combined under Transaction_Location column.
      
      > Customer and transaction related columns that may not impact on our models.
      
      > Age_group as it was feature engineered for EDA purposes.
      
      > Column 'transaction_datetime' is not needed as we have Transaction_Day and Transaction_Hour to represent the same information as transaction_datetime.
      
  * After dropping the column the dataset has 200000 rows and 16 columns.
  * The target variable (Is_Fraud) have outliers. However, these are not actual outliers but rather representations of fraud (Is_Fraud = 1) and non-fraud (Is_Fraud = 0) which is a binary classification.
    
# 📌 Machine Learning Models
---
> In this section, we built and optimize classification models for our task. This process involved several key steps, including:
  * Creating Pipelines that incorporate preprocessing steps such as feature scaling.
  * Defining Features and the Target Variable for model training. 
  * Splitting the Data into training and testing sets. 
  * Training Multiple Models on the training dataset. 
  * Identifying the Best-Performing Model based on evaluation metrics. 
  * Tuning the Best Model using hyperparameter optimization. 
  * Evaluating Model Performance to assess effectiveness and generalization.

> The accuracy score of our baseline Logistic Regression Model is 0.50575. 
> Alternative models we have considered for our project:

## Model Performance Comparison

| Classifier                        | Test Accuracy | AUC        |
|------------------------------------|--------------|------------|
| Decision Tree Classifier          | 0.9002       | 0.4991     |
| Random Forest Classifier          | 0.9489       | 0.5001     |
| KNeighbors Classifier             | 0.9478       | 0.4999     |
| Bagging Classifier                | 0.9489       | 0.5108     |
| AdaBoost Classifier               | 0.3253       | 0.5047     | 
| Gradient Boosting Classifier      | 0.6432       | 0.5088     |
| XGBoost Classifier                | 0.7325       | 0.5081     |
**Best Model:** 🏆 **Random Forest Classifier** (Accuracy: **0.9489**) 

> To address the issue of class imbalance, we have exclusively used class weights. Other alternative that was available is use of SMOTE but this may result to overfitting resulting from introducing synthetic data.
> 
* Model evaluation:
  
    1. Accuracy, Precision, Recall, F1-score
    2. Confusion Matrix
    3. ROC-AUC Curve

 # 📌Results and Performance
 ---

* Summarize the findings from the models:
  
    1. Best performing model based on metrics
    2. Model comparison table
    3. Example visualization of results

# 📌 Conclusion
---

* There seem to be a minor difference in the number of fraud cases between genders suggesting that the fraud occurences is relatively balanced across the genders.

* For customers at the age 19-30 and 51 - 60 years show significantly higher numbers of fraud cases which further indicates that individuals in the age groups are more vulnerable to fraud.

* The transaction type with the highest number of frauds is Transfer with 2,073 cases reported, followed closely by credit transactions with 2048 cases.

* The ATM Booth Kiosk, the ATM and the Self-service Machine channels posed the highest risk of fraud among the transaction devices.

* The peak periods of fraud incidents are during holidays.

# 📌 Recommendations
---

* Financial institutions to use fraud by age-group analysis to perform risk assessment to inform and come up with awareness campaigns towards the targeted group to reduce chances of fraud.

* Financial institution to do a deeper analysis on the how to establish controls to mitigate risks of fraud in areas with highest frequency including transfers and credit transactions.

* More controls need to be established on the ATM Booth Kiosk, the ATM and the Self-service Machine as they reported the most frauds.

* Financial institution should heighten monitoring of fraudulent activities during holidays and special days marked in the country.

* Understanding the distribution of fraud cases by age group can aid in risk assessment and the development of targeted fraud prevention strategies. Financial institutions and security agencies can use this information to implement age-specific awareness campaigns and security measures.

* Understanding the distribution of fraud cases by gender can help in designing targeted fraud prevention strategies. For example, if females have a higher number of fraud cases, awareness campaigns and security measures can be tailored specifically for female users.

---
