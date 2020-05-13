# Prosper-Loans-Data-Analysis
Project is part of a Udacity Data Analyst Nanodegree. The task of the project was to analyze and visualize real-world data.
## Installations:
 - Python 3
 - Anaconda distribution to install Python, since the distribution includes all necessary Python libraries as well as Jupyter Notebooks.
 - Numpy
 - Pandas
 - Matplotlib
 - Seaborn
 
 ## Dataset

> This project is on a data set from Prosper, which is America’s first marketplace lending platform, with over $7 billion in funded loans. This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, borrower employment status, borrower credit history, and the latest payment information.

The main purpose of this project is to summarize the characteristics of variables that can affect the loan status and to get some ideas about the relationships among multiple variables using summary statistics and data visualizations.


## Summary of Findings

 - DTI values ranges from 0 to 10. But most of the values are between 0 an 1.
 - Though, Incomerange of (25,000 - 49,999) and (50,000 - 74,999) has almost equal number of loans but 35% of total charged off loans are in (25,000 - 49,999) where as in (50,000 - 74,999) has only around 22% of total charged off loans.
 - Most of the DTI values with more than 1 are from (1-24,999) category so if we include these we will be biasing our results. because (1-24,999) category has less than 10 percent with DTI greater than 1 but these can change the average values drastically.
 - Though Both category levels of IsBorrowerHomeowner have same number of loans. (chargedoff,defaulted,pastdue) loans are much higher when IsBorrowerHomeowner is False.
 - Though CreditScoreAverage for non home owners follows the same distribution as observed in bivariate analysis. for home owners the creditscoreAverage has different distribution is quite evident in the defaulted and chargedoff loans.
 - Percentage of charged off and defaulted loans from All existing customers are less when compared to percentage of charged off and defaulted loans from All new customers. Which suggests to predict loan status, borrower prosper history is more important than the general history of borrower.
 - Prosper score with 10(best) also have the credit scores around 600



## Key Insights for Presentation

 - In ($1-24,999) income category if we consider all the loans then if the DTI average is greater than 0.75 then most probably it is one of the (chargedoff,defaulted,pastdue) loans and less than 0.75 it's either current or completed loans this conclusion is false because these average values are affected by the extreme values. if we remove the extreme cases about more than 90 percent of loans follows the different distribution and their average DTI for defaulted and charged off loans are less.
 - Distribution of loan status for existing customers are better than the new customers.
 - Distribution of credit scores are different for home owners in each loan status it is clearly evident in Defaulted loan status.
