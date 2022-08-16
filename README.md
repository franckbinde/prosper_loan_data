# Prosper Loan Data
## by Franck Alain Binde Koube


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. All the descriptions about the columns could be find [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0). It is strongly recommended to have a look at the variables description to better understand the data. 


## Summary of Findings

- The majority of loans are in the Debt Consolidation category. Also, it looks like many borrower don't feel comfortable displaying the reasons behind a loan.
- Loans with 36 months of Term period are by far the most represented.
- August is the month with most of the originated loans (around 5200 loans). With around 3800 loans generated, February ranks last in this category.
- I have found a relatively strong and negative correlation (r = -0.717) between `ProsperScore` and `BorrowerRate`. In general, people with lower interest rate for their loan tend to complete the payment. Besides, 
- Long term loans are in general more expensive (since there is more time to complete the payment). We see that the median of the loan amount for a 60-months loan is much higher that the ones for 12 and 36 months.
- Regardless of the loan status, **home owners tend to acquire more expensive loans**. Indeed, the median and 3rd quartile of loan amounts are higher for home owners. On the other hand, owning a home doesn't seem to have a significant impact on the loan status. 
- Self-employed people with completed loans have a much lower median loan amount than self-employed with defaulted loans.

## Key Insights for Presentation

For the presentation, I focus on features that may impact `LoanStatus`, `BorrowerRate` and `LoanOriginalAmount`. I used a heatmap to see the correlation between numeric variables. Violin plots and boxplots were also used in order to better understand the distribution of these variables on both 2d and 3rd dimensionnal level. To achieve this, extra variables like `IsBorrowerHomeOwner` and `EmploymentStatus` were helpful and enabled me to reveal interesting insights.

