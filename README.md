# Business-case-Credit-Score
### Insights: 
- There are 12500 number of unique customers
 -   Every unique customer has 8 records in the data.
    -   There are equal 12500 number of records in the data spread through the 8 above mentioned months
    -   The most number of records are for the age 18 to 45. 
    - The starting entry for -500 could be place holder used by them for missing value or just anamoly in the dataset.
-  These are the anamolies of the dataset.
  -   Almost all the records are distributed similarly amongst the each occupation, meaning people from all the occupation are interested. 
  - The first ____ could be a place holder or anamoly in the dataset
-  The Architect draws max avg monthly salary (4103.738453). 
- The Journalist draws min avg monthly salary (3864.083734).
 -   Max monthly salary is between 4050 and 4100.
-   The Lawyer makes the most salary annually (196902.095402). 
- The Teacher makes the least salary annually (162108.368540).
 -   Customer CUS_0x294b has 10 number of banks, which is the highest. 
 -  Some of the count is negative which could be the anamolies in the data or just a place holder for null enteries.
 -   Customer CUS_0x1d6f has 11 number of credit cards, which is the highest. 
 - Customer CUS_0x7ce5 has 0 number of credit cards, which is the least.
-   The customer CUS_0x4d1c has highest number of loans 9. 
- The customer CUS_0x6da9 has least number of loans 0.
 -  The customer CUS_0xac39 has 28 delayed number, highest number of dealyed payment.
  -   The customer CUS_0x392a has highest number of inquiries 17.
  - The customer CUS_0xc5ee has 4998.07 outstanding debt, which is the highest debt.
  - The customer CUS_0x4c5 has 0.23 outstanding debt, which is the lowest debt.
  - The customer CUS_0x6698 has avg credit utilization of 43.774821 which is the highest. 
  -  The customer CUS_0xc600 has avg credit utilization of 23.698861 which is the lowest.
  - The mean of the credit utilization is about 40%.
  - There are 6261 types of loan that the customers have.
  - Low_spent_Small_value_payments accounts for the highest num. of types of payment behaviour. 
  -  !@9#%8 presents the anamolies in the dataset or just the placeholder used for null values.
  - 52.3 % of the records have customer who pays the minimum amount. 
  -  35.7 % of the records have customer who doesn't pay minimum amount.
  - The customer CUS_0xa1ec has the highest Total EMI per month (1779.103254). 
  - The customer CUS_0x6da9 has the lowest Total EMI per month (0).
  - According to credit score nearly 85K rows here(i.e. the customer maybe duplicate) are credit-worthy. 
  - According to credit score nearly 15K rows here(i.e. the customer maybe duplicate) are not credit-worthy.

### Recommendations:
-   Develop Financial Literacy Programs: Focus Areas: Emphasize education on manag ing personal finances, debt reduction, and long-term investments. Target Group: Lower income groups (earning less than ￿50,000 annually) and individuals with lower monthly in hand salaries. Potential Benefits: Increased customer engagement, improved financial health, 40 and reduced loan defaults. 
-  Create Income-Based Loan Products: Flexible Loan Options: Offer micro-loans or small personal loans with lower EMIs for customers earning less than ￿8,000 monthly. Tailored Interest Rates: Use the insight that most customers have manageable outstanding debts and low EMIs to provide competitive interest rates. 
-  Encourage Credit Utilization Management: Promote Responsible Credit Use: Given that most customers’ credit utilization ratio is between 25-39%, provide tips or products that help optimize credit use. Credit Counseling: For those with higher utilization, introduce services to help improve their credit score, which could lead to better loan terms. 
-  Offer Specialized Investment Plans: Low-Entry Investment Options: Since most cus tomers invest around ￿100 per month, introduce financial products like mutual funds or savings plans that have low entry points and incentives for incremental growth. Investment Educa tion: Create workshops or materials to educate customers on how they can gradually increase their monthly investment amounts. 
-  Incentivize Credit Mix Improvement: Rewards for Diverse Credit Use: Since most people maintain a standard credit mix, offer rewards or reduced interest rates for customers who diversify their credit types (e.g., combining personal loans, credit cards, etc.). 
-  Encourage Debt Repayment Beyond Minimums: Awareness Campaign: Educate cus tomers on the benefits of paying more than the minimum amount due to reduce overall interest paid and improve credit scores. Automated Payment Plans: Introduce automatic payment systems where customers can choose to pay slightly more than the minimum, helping them reduce debt faster. 
-  Personalized Financial Planning Tools: Mobile Banking Tools: Create a feature that allows customers to set financial goals, track debt repayment, and monitor credit utilization in real-time. Advisory Services: Offer personalized financial advice through in-app chat or f inancial advisory sessions to help customers better manage income, investments, and debt. 
-  Improve Risk Assessment: Customized Credit Risk Models: Since weak correlations exist between income, debt, and credit utilization, refine lending criteria to assess creditworthiness based on a combination of factors, rather than solely on income or debt levels. Data-Driven Lending: Utilize advanced analytics and AI tools to predict customer behavior, helping to assess risk more accurately and avoid loan defaults.
 
### Business Problem:


To conduct a thorough exploratory data analysis (EDA) and deep analysis of a comprehensive dataset containing basic customer details and extensive credit-related information. The aim is to create new, informative features, calculate a hypothetical credit score, and uncover meaningful patterns, anomalies, and insights within the data.
  
### Dataset:
[Dataset](https://github.com/AbhinavTalmale/Business-case-Credit-Score/tree/main/Dataset)

**Data Description:**

| Column Name               | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| ID                        | Represents a unique identification of an entry                             |
| Customer_ID               | Represents a unique identification of a person                            |
| Month                     | Represents the month of the year                                           |
| Name                      | Represents the name of a person                                            |
| Age                       | Represents the age of the person                                           |
| SSN                       | Represents the social security number of a person                         |
| Occupation                | Represents the occupation of the person                                    |
| Annual_Income             | Represents the annual income of the person                                 |
| Monthly_Inhand_Salary     | Represents the monthly base salary of a person                             |
| Num_Bank_Accounts         | Represents the number of bank accounts a person holds                      |
| Num_Credit_Card           | Represents the number of other credit cards held by a person               |
| Interest_Rate             | Represents the interest rate on credit card                                |
| Num_of_Loan               | Represents the number of loans taken from the bank                         |
| Type_of_Loan              | Represents the types of loan taken by a person                             |
| Delay_from_due_date       | Represents the average number of days delayed from the payment date        |
| Num_of_Delayed_Payment    | Represents the average number of payments delayed by a person              |
| Changed_Credit_Limit      | Represents the percentage change in credit card limit                      |
| Num_Credit_Inquiries      | Represents the number of credit card inquiries                             |
| Credit_Mix                | Represents the classification of the mix of credits                        |
| Outstanding_Debt          | Represents the remaining debt to be paid (in USD)                         |
| Credit_Utilization_Ratio  | Represents the utilization ratio of credit card                            |
| Credit_History_Age        | Represents the age of credit history of the person                        |
| Payment_of_Min_Amount     | Represents whether only the minimum amount was paid by the person          |
| Total_EMI_per_month       | Represents the monthly EMI payments (in USD)                              |
| Amount_invested_monthly   | Represents the monthly amount invested by the customer (in USD)            |
| Payment_Behaviour         | Represents the payment behavior of the customer (in USD)                  |
| Monthly_Balance           | Represents the monthly balance amount of the customer (in USD)            |


