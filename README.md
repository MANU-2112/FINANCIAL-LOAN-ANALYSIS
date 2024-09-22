## Project Background
APEX FINANCIAL, is a mid-sized financial institution that provides a range of loan products, including personal, auto, and home loans. With a growing customer base, the company has expanded rapidly but is now encountering issues in managing its loan portfolio effectively.

Despite growing demand for loans, the company has observed an increase in loan defaults and inconsistent approval rates. This has led to rising financial risks and uncertainty in forecasting repayment timelines.

Insights and recommendations are provided on the following key areas:

1. **Factors contributing to loan approval**: Explored borrower characteristics (e.g., employment status, income) and loan conditions like loan amount, interest rates that correlate with high default rates.
2. **Improved loan approval decisions**: Analyzed historical data to identify patterns and factors that influence successful loan repayments, helping to refine the loan approval process.
3. **Segment the customer base**: Deep dive into segments of borrowers (by income levels, loan types) are most and least risky, allowing for better-targeted loan offerings.
4. **Enhance risk management**: Provided actionable insights according to MTD and MoM percentages to monitor risk management and areas to focus on.



Targeted SQL queries regarding various business questions can be found here. [Link](https://drive.google.com/file/d/1opjiqFX8QVN-fAyCf8hzsUyZH_ZCA8s4/view?usp=drive_link)

An interactive PowerBI dashboard used to report and explore trends can be found here. [Link](https://app.powerbi.com/groups/me/reports/15fda782-82d6-4b63-ae2a-d422413270f3/b1d7243543fe61f61797?experience=power-bi)
 
 

## Data Structure & Initial Checks
The company's provided database structure as seen below consists of two tables: Employee and Financial_Loan tables with a total row count of 39,577 records. A description of each table is as follows:

![Screenshot 2024-09-23 005602](https://github.com/user-attachments/assets/368d4beb-1472-456a-849d-8f2df9f9d28d)


## Executive Summary
#### Summary of Findings:
The financial loan analysis shows strong performance with $473.1M received and a 15.8% Month-over-Month increase in repayments. Good loans make up 86.2% of the portfolio, while **bad loans represent 13.8%, signaling some risk with defaults or delayed payments**. Loan issuance grew by 13.0% MoM, but the **rising interest rates (+3.5%) may affect future demand, requiring careful risk management.**

Below is the summary page from the PowerBI dashboard.This also contains level 2 and level 3 metrics. The dashboard can be accessed above.   

![Screenshot 2024-09-23 010517](https://github.com/user-attachments/assets/0fc73e4f-34a6-4ab4-83e1-1bc285399679)

## Insights Deep Dive

KPI's:
1. There were 38.6K loan applications, with a Month-to-Date (MTD) increase of 4.3K. This **reflects growing demand for loans, which can increase business opportunities and revenue**. 
   The 6.9% Month-over-Month (MoM) increase indicates a **rising trend in loan requests, potentially due to seasonal factors or effective marketing.**

2. A total of $435.8M was funded, with $54.0M funded MTD. This showcases **significant loan disbursement activity, translating into immediate revenue from interest payments.**
   The 13.0% MoM growth highlights a strong increase in loan funding, indicating robust loan processing and customer acquisition.

3. Total repayment received stands at $473.1M. This metric is crucial for cash flow management and **signals efficient collections and positive borrower behavior.**
   A 15.8% MoM increase in repayments shows **improved collection strategies or better borrower performance, leading to healthier financials.**

4. The current Average Interest Rate is 12.05%.
   Interest rates directly affect the profitability of loan products, impacting revenue margins.
   A 3.5% MoM **increase in the interest rate could attract higher revenues, but may also affect loan demand, especially among cost-sensitive borrowers.**

5. Average DTI stands at 13.3%, with an MTD average of 13.7%. Lower DTI percentage indicates higher success rate of repayment.
   **A 2.7% of MoM appreciates the loan approval system of the bank.**
   
![Screenshot 2024-09-23 010624](https://github.com/user-attachments/assets/607b8364-e215-4e70-9184-a946b17eeb9b)



LOAN APPROVAL DECISIONS:

1. Good Loans constitute 86.2% of total loan applications. These loans are funded at $370.2M and have resulted in $435.8M in total received amount.
   **Bad Loans represent 13.8% (5.3K) of applications, with $65.5M funded and $37.3M recovered.** 
   **The higher risk and potential loss is noticeable.**
   Month-over-Month (MoM) growth for funded amounts in Good Loans is 13%, while Bad Loans likely show a lower growth, though specific MoM details for bad loans are not visible.

2. **Fully Paid loans total 32.1K, funded at $351.3M, with a received amount of $413.2M.**
   **This shows a high recovery efficiency.**
   Current Loans are 1,098 in number, funded with $18.8M.
   They have brought in $24.1M, indicating strong repayment activity, with $39.4M funded this month.
   MoM Fully Paid loans received amount is $47.8M, reflecting stable repayment growth.

3. **Charged Off loans** total 5.3K, with $65.5M funded and $37.2M received, indicating **significant losses due to defaults.**
   The Month-to-Date (MTD) funded amount for charged-off loans is $87.3K, signaling either reduced new risky loans or write-offs.

4. **Average interest rates** show the highest rate for current loans at 15.10%, compared to 11.64% for fully paid loans,
   indicating charge of higher rates for ongoing loans. **This is decent but can be adjusted based on MTD and MoM amount received parameters.**

![Screenshot 2024-09-23 010746](https://github.com/user-attachments/assets/3a11a13b-d639-4839-ae10-4529034fd044)



CUSTOMER BASE SEGMENTATION:

1. Loan applications show consistent growth from 2.3K in January to 4.3K in December, with a steady upward trajectory. 
   **A notable spike occurs between August (3.4K) and December, where applications increase by 900.**
   This suggests strong quarterly performance growth, **particularly in Q4, reflecting potential seasonal trends or end-of-year demand.**

2. Applicants with over 10+ years of employment lead with 8.9K applications, indicating stability which attracts loan approvals. New hires (<1 year) still account for 4.6K applications.

3. Debt consolidation tops the chart at 18K applications, followed by credit card purposes (5K), showing that refinancing personal debt is a primary motivator.

4. There’s a diversified demand for loans, including home improvement (3K) and small business (2K), reflecting varied consumer financing needs.

5. A majority (73.2%) of applications are for 60-month terms (28.2K), showing a preference for longer repayment durations, while 36-month terms account for 26.8% (10.3K).

6. **Renters make up the largest share, suggesting renters are more actively seeking loans.** 
   This homeownership data implies that non-homeowners are the predominant loan applicants, likely driven by higher financing needs for various expenses.

![Screenshot 2024-09-23 012550](https://github.com/user-attachments/assets/98baa8bd-ead3-4262-a423-6eb2c85f5188)


## Recommendations:
Based on the insights and findings above, I would recommend to consider the following:

1. Reduce bad loans by tightening credit criteria for applicants with low credit scores or unstable employment. **Focus on minimizing exposure to high-risk segments by using predictive     
   analytics models.**

2. Consider **lowering interest rates for loans with lower DTI ratios to attract more borrowers with lower risk profiles.** Additionally, implement more stringent underwriting criteria for      loans with higher DTI ratios to mitigate financial risk.

3. **Promote products like debt consolidation and home improvement loans, which are high in demand and likely low-risk.** This can boost the portfolio's overall quality and repayment 
   reliability.

4. **Implement real-time monitoring for current loans with high interest rates or early delinquency signs.** Early intervention strategies can improve repayment rates and reduce defaults.

5. **Prioritize marketing loans to applicants with 10+ years of job tenure, as they show strong repayment performance.** This helps to build a stable loan portfolio with consistent returns.


## Assumptions and Caveats

1. "Issue Date" was taken as reference for the date related metrics such as MTD and MoM.
2. DTI's and interest rates data was inconsistent. Some had missing values. So, mean of interest rates was taken to fill the nulls.
