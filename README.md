### Prosper Loan
Prosper is a peer-to-peer lending marketplace based in the United States. Borrowers apply online for a fixed-rate, fixed-term loan between $2,000 and $40,000. Individuals and institutions can invest in the loans and earn attractive returns. Prosper handles all loan servicing on behalf of the matched borrowers and investors.

I am exploring the prosper loan dataset as a part of my Udacity Nanodegree in data analysis program. 
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

#### Exploratory Questions
1. What factors affect a loan’s outcome status?
2. What affects the borrower’s APR or interest rate?

The Prosper Loan Data was explored with the goal of finding insights on Loan Status outcomes. The main feature of interest is the LoanStatus. The unique entries in the LoanStatus columns are: 'Completed', 'Cancelled', 'Current', 'Defaulted', 'Past Due (1-15 days)', 'Past Due (16-30 days)', 'Past Due (31-60 days)', 'Past Due (61-90 days)', 'Past Due (91-120 days)', 'Past Due (>120 days)', 'FinalPaymentInProgress', and 'Chargedoff'. My interest is to find out the variables that are important to predicting LoanStatus.

In finding this relationship, I dropped some features to concentrate on some features of interest. Some features of interest are LoanTerm, BorrowerAPR, CreditScoreRange, DebtToIncomeRatio, AvailableBankcardCredit, etc.

### Summary of findings
Summarily, the following observations are drawn from this exploration

Factor that affects a Loan Outcome Status are:

> **DebtToIncomeRatio** 
> DebtToIncomeRatio is notably high in Borrowers that fall in the Not Employed category in Employment status column. Consequently, and from previous exploration, high average DebtToIncomeRatio is noticed in LoanStatus outcome categories as Defaulted, PastDue and Chargedoff. 
> Borrowers with lower Debt to income ratio have high available bank card credit, while borrowers with high debt to income ratio have lower available bank card credit.

> **BorrowerAPR** - 
> Borrowers in the Defalted, Past Due and Chargedoff Loan status categories have higher Borrower APR.

> The Not Employed category of the Employment Status column have the highest BorrowerAPR. 

> The higher the EstimatedReturn, BorrowerRate, and BankCardUtilization, the more the BorrowerAPR, and the lower the ProsperScore, AvailableBankcardCredit, and CreditRangeScoreUpper the more the BorrowerAPR

> BorrowerAPR is highest in borrowers with defaulted loan status that had 12 month loan term. BorrowerAPR is lowest in borrowers with FinalPaymentinProgress Loan Status and 12 month payment term.

> Borrowers whose BorrowerAPR are greater than 25% are more likely to not pay complete their Loan repayment.
 and BorrowerAPR. 
 > **Employment Status**
 The Not employed category of borrowers are more likely to default on the repayment of their Loan.
 
<<<<<<< HEAD
From the exploration , we discovered that there is a relationship between Employment Status, BorrowerAPR and the Loan Status. This relationship is explained in Part_II_Explanation files.

### **Key Insights for Presentation**

In the explanatory analysis, visualizations that show the relationship between Employment Status, BorrowerAPR and Loan Status will be displayed.
This will give clearer visuals on the following:

 - Loan repayment status in comparison with BorrowerAPR
 - The employment status of borrowers that are more likely to default on the repayment of their Loan
=======
From the exploration , we discovered that there is a relationship between DebtToIncomeRatio, BorrowerAPR and the Loan Status. This relationship is explained in Part_II_Explanation files.

### **Key Insights for Presentation**

In the explanatory analysis, visualizations that show the relationship between Employment Status, BorrowerAPR and Loan Status will be displayed.
This will give clearer visuals on the following:

 - Loan repayment status in comparison with BorrowerAPR
 - The employment status of borrowers that are more likely to default on the repayment of their Loan