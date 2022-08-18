### Prosper Loan
Prosper is a peer-to-peer lending marketplace based in the United States. Borrowers apply online for a fixed-rate, fixed-term loan between $2,000 and $40,000. Individuals and institutions can invest in the loans and earn attractive returns. Prosper handles all loan servicing on behalf of the matched borrowers and investors.

I am exploring the prosper loan dataset as a part of my Udacity Nanodegree in data analysis program. 
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.


#### Exploratory Questions
1. What factors affect a loan’s outcome status?
2. What affects the borrower’s APR or interest rate?

The Prosper Loan Data was explored with the goal of finding insights on Loan Status outcomes. The main feature of interest is the LoanStatus. The unique entries in the LoanStatus columns are: 'Completed', 'Cancelled', 'Current', 'Defaulted', 'Past Due (1-15 days)', 'Past Due (16-30 days)', 'Past Due (31-60 days)', 'Past Due (61-90 days)', 'Past Due (91-120 days)', 'Past Due (>120 days)', 'FinalPaymentInProgress', and 'Chargedoff'. My interest is to find out the variables that are important to predicting LoanStatus.

In finding this relationship, I dropped some features to concentrate on some features of interest. Some features of interest are LoanTerm, BorrowerAPR, CreditScoreRange, DebtToIncomeRatio, AvailableBankcardCredit, etc.

### Conclusions
Summarily, the following insights are drawn from this exploration

Factor that affects a Loan Outcome Status are:

> **DebtToIncomeRatio** 
> DebtToIncomeRatio is notably high in Borrowers that fall in the Not Employed category in Employment status column. Consequently, and from previous exploration, high average DebtToIncomeRatio is noticed in LoanStatus outcome categories as Defaulted, PastDue and Chargedoff. 

> **BorrowerAPR** - 
> Borrowers in the Defalted, Past Due and Chargedoff Loan status categories have higher Borrower APR.

> The Not Employed category of the Employment Status column have the highest BorrowerAPR. From previous plot of BorrowerAPR by LoanStatus, It was observed that borrowers with lower APR are more likely to complete their loan repayment when compared with the other borrowers. Thus Not employed category of borrowers are more likely to default on the repayment of their Loan.

> The higher the EstimatedReturn, BorrowerRate, and BankCardUtilization, the more the BorrowerAPR, and the lower the ProsperScore, AvailableBankcardCredit, and CreditRangeScoreUpper the more the BorrowerAPR

> BorrowerAPR is highest in borrowers with defaulted loan status that had 12 month loan term. BorrowerAPR is lowest in borrowers with FinalPaymentinProgress Loan Status and 12 month payment term.

> Borrowers whose BorrowerAPR are greater than 25% are more likely to not pay complete their Loan repayment.

> **DebtToIncomeRatio**

> DebtToIncomeRatio is notably high in Borrowers that fall in the Not Employed category in Employment status column. Consequently, and from previous exploration, high average DebtToIncomeRatio is noticed in LoanStatus outcome categories as Defaulted, PastDue and Chargedoff. 

> Borrowers with lower Debt to income ratio have high available bank card credit, while borrowers with high debt to income ratio have lower available bank card credit.
