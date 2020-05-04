# Prosper Lending Data Analysis Project

## Dataset

The data contains 113,937 loans with 81 variables on each loan, including loan amount, 
borrower rate (or interest rate), current loan status, borrower income, and many others. 
However, because of missing data issues, only data after July 2009 is interpreted.


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
interest rate for borrowers and their credit rating.However, this relationship
is only clear if the rating or credit score is really high or really low. In 
other words, if borrowers are very high risk, they are penalized by higher 
interest rates. On the other hand, if borrowers are very low credit risk, 
they entitile low borrowing rate. For customer wtih medium risk, there is no 
clear pattern. 

I extended my investigation of interest rate against credit rating by looking 
at the impact of categorical features. The multivariate exploration showed that 
there is a negative relation ship between the credit rating and interest rate. 
The higher credit rating, the lower interest rate. However, there is no clear 
different in interest rate of borrower who have the same credit rating but 
different listing category or employment status. When borrowers own a home, 
they pay lower interest if their employment status is employed, fulltime or 
self-employed. It is completely inverse for unemployed borrowers.


## Key Insights for Presentation

For the presentation, I focus on just the influence of credit rating to the 
interest rate of borrowers. I start by introducing the interest rate variable, 
followed by the pattern in distribution of Average Credit Score, Prosper Score
and Prosper Rating.

Afterwards, I introduce the relationship between Interest Rate and Prosper Rating, 
Employment Status and Home Ownership by ploting a pairgrid boxplot. Then, I dig 
deeper to the relationship between Interest Rate and Average Credit Score as well
as Prosper Score. Two scatter plots of each two variables and a pinpoint plot of 
three variable are created to visualize the relationship between them. 

Finally, another pinpoint plot is display to visulize the relationship between
Interest Rate, Imployment Status and Home Ownership

jupyter nbconvert slide_deck.ipynb --to slides --post serve --template output_toggle
