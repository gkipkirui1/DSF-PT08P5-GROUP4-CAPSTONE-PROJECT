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

The variables in the dataset are *Customer_ID*, *Customer_Name*, *Gender* , *Age* ,*State*, *City*, *Bank_Branch*, *Account_Type*, *Transaction_ID*, *Transaction_Date*, *Transaction_Time*, *Transaction_Amount*, *Merchant_ID*, *Transaction_Type*, *Merchant_Category*, *Account_Balance*, *Transaction_Device*, * Transaction_Location*, *Device_Type*, *Is_Fraud*, *Transaction_Currency*, *Customer_Contact*, *Transaction_Description* and *Customer_Email* 


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



# 📌Exploratory Data Analysis (EDA)
---
1. Univariate Analysis
     * For the class 0 indicating **(Non-fraud cases)** which is 94.956% of the data while for class 1 **(fraud cases)** 5.044% of the data.
     * The transaction type with the highest cases of fraud is: **Transfer**. 
     * The state with the highest fraud cases is: **Lakshadweep**.
     * The distribution points to a slightly higher number of reported fraud cases affecting **males** as compared to **females**.
     * The transaction device with the highest fraud cases is: **ATM Booth Kiosk** while the transaction device with the lowest fraud cases is: **POS Terminal**. 
     * The age distribution shows a more uniform spread, with a slight concentration in the **middle age range (around 30-50 years)**. This suggests that the bank's customer base is primarily composed of middle-aged individuals.

# 📌 Machine Learning Models
---
* Models applied:
    1. Logistic Regression
    2. Decision Trees
    3. Random Forest
    4. XGBoost
       
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


# 📌 Recommendations
---
