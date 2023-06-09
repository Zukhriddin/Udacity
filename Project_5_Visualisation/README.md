# Prosper Load Data Exploration
## by Zukhriddin Juliev


## Dataset

I use Prosper dataset, which is a peer-to-peer loan service. The dataset contains 113,937 observations with 81 variables. The dataset can be downloaded from this [link](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554484977406000) and description of variables from this [link](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit). 
Within exploration I am interested in factors impacting investor number per loan. I restrict the data to year 2013 and variables which could be related with investor numbers. Final sample contains 33912 unique loans with 15 variables. 
Before starting investigation I conducted following wrangling procedures: converted income range variable into ordered categorical data, created text version of loan categories, converted boolean home ownership data into string type data.
For actual investigation first I looked to distribution of each variable and then its relationship with the variable of interest (investor number). Finally, I selected varriables which showed high correlation with investor number and plotted them together as a multivariate plot.

## Summary of Findings

I found that investor number of the loan is highly correlated (negatively) with expecter returns and borrower rate. This correlation is mostly driven by loan sizes. Greater loans have lower interest rate but they also have more investors. Moreover, larger loan borrowers are more often homeowner, which explains why investors are more likely to crowd into such loans even thought interest rates are low. Additionally, loans categorized to debt consolidation and business also correlated with more investors since large size loans are more frequent among these categories.
Variables such as borrower background (employment or credit history) does not much impacts the investor numbers. 


## Key Insights for Presentation

First, investor numbers is highly skewed to lower numbers. However, there are also many loans with investors more than 20. 
Second, loan size is the key factor in defining investor numbers. Larger loans are correlated with greater investor numbers.
Third, there is highly negative correlation between interest rates (borrower rate or exected returns) and investor number. these might be explained via size of the loans. Larger loans have lower rates.
Fourth, homeowners are more likely to secure large loans with more investors.
Fifth, loans category of debt consolidation or business are more likely to be funded by multiple investors. This fact can also be explained by loans size for such category and also type of security.