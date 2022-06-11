# Prosper Loans Data Exploration

## Dataset

The dataset involves 113,937 loans made using the Prosper service. There are 81 
variables in total, for various loan attributes such as *Term* and *BorrowerRate*, and various borrower attributes such as *Occupation* and *ListingCategory*. You can find the dataset [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), with feature documentation [here](https://docs.google.com/spreadsheets/u/0/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit?usp=sharing).

The main 4 variables I focused on were *LoanStatus*, *LoanOriginalAmount*, *BorrowerRate* and *ProsperScore*. Mostly *LoanStatus* though, I've also looked at the effect of various borrower-related factors on the status of a Loan, and whether it contributes to more loans being completed or not. 

## Summary of Findings

So, I've started with about 12 variables, and analyzed all of them univariately, interesting findings include that 70% of all finished loans have been successfully completed, BorowerRate turned out to have some specific common rates, most commonly at 31%, although that doesn't lead to te best chance of a successful loan. The most common amount of money loaned was $4000. Most borrowers had a yearly income of at least $25,000. Over 50% of loans were made for Debt conslidations, and they were mostly made by professionals, programmers and teachers. While a very small amount were made by Dentists and Judges.

For my Bivariate analysis, I studied the effect of other variables on the loan status, and the chance of a successful completed loans. It turns out that loans with a rate between 0.2 and 0.35 have a 40% chance of being successfully completed. On the other hand, Prosper scores of 8+ had a relatively higher chance of completed loans. People who list *Other* as their occupation tend to do relatively worse in terms of completed loans, while *Professionals* have a higher chance, same goes for *Judges* and *Dentists* although their number was small. Also it seems that Debt Consolidation leads to many default loans, and self-employed borrowers have a relatively high chance of not successfully completing a loan.

Other findings include a very clear negative correlation between a borrower's rate and Prosper score, and a clear negative correlation between a borrwer's rate and the amount of money borrowed. Later, In my multivariate analysis I've analyzed these 4 variables and ended up confirming my Bivariate analysis findings.

## Key Insights for Presentation

I start by showing the distribution of the 5 most common Occupations and Listing categories, also the percentage of finished loans, using relative bar plots. Then I move on to show the effect on Borrower's rate on finished loans and that the chance of successful loans is lower between 0.2 and 0.35, this is shown using a violinplot followed by a pie chart.

I also show some of the bivariate interesting insights, regarding Occupation and Listing Categories and which lead to a higher chance of a successful loan. This is shown by a Faceted bar plot.

## Files in this project

- Notebooks: Shows the analysis process.
- Output: Shows the findings.

