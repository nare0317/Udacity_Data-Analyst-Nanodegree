## Prosper Loan Data Exploration
## by Narae Im


## Dataset

> This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.


## Summary of Findings

My main interest is figuring out what features are best for predicting the Credit Grade(Rating) in the dataset.

I expected that each borrowers Monthly Income, DebtToIncomeRatio, and Employment status will have the strongest effect on CreditGrade: the higher the income and the lower the DebtToIncomeRatio and the more stable the employment status, the greater grades of credit rating.

1) Univariate exploration
I looked into Rating, DebtToIncome Ratio, Stated Monthly Income and Income range variables.
- Rating : Among 8 credit rating in total, "D", "C", "B" was the top 3 most common rating. 
- Stated Monthly Income : There were some high outliers in the data, so I limit the x axis from $500 - $2000,  and as the distribution has a long tail, I plotted on a log-scale and the final distribution looks roughly unimodal, with one peak between 3k - 7k. 
- Debt To Income Ratio : When plotted DebtToIncomeRatio variable, most of values were in between 0 and 1. So I limited x axis to 0-1. There's a long tail in the distribution of the Debt to Income Ratio. Most of values are between 0.1 - 0.3 and only few values are greater than 0.5.
- Income Range : The most common income range was $25,000 ~$75,000.

2) Bivariate exploration
- Quantitative vs Quantitative : I used correlation heat map. I found out that Rating(numeric) has a strong positive correlation with CreditScoreRangeLower, CreditScoreRangeUpper and a strong negative correlation with BorrowerRate.
- Quantitative vs. Qualitative : I looked into Credit Ratings by Debt To Income Ratio and Stated Monthly Income. 
- Qualitative vs. Qualitative : I looked into Distribution of Income Ranges and Credit Ratings. 

3) Multivariate exploration
- I used point plot for Borrower Monthly Income($) across Employment Status and Rating and Debt To Income Ratio across Employment Status and Rating. 
- Also, in final steps, I used heat maps to figure out the relationships with Rating, BorrowerRate, and StatedMonthlyIncome / Occupation, BorrowerRate, and StatedMonthlyIncome.

## Key Insights for Presentation

My main goal of this presentation is to figure out what features are affecting the Credit Grade(Rating) in the dataset.
So I included 4 visualizations in this presentation.

1) Credit Ratings by Debt To Income Ratio and Stated Monthly Income
2) Distribution of Income Ranges and Credit Ratings
3) Borrower Monthly Income across Employment Status and Credit Rating
4) Debt To Income Ratio across Employment Status and Credit Rating