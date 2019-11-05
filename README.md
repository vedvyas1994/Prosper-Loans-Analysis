# Communicate Findings About Loan Data from prosper
#### by Vedavyas Kamath <br><br>


## Dataset
Used the file `prosperLoanData.csv` which is available for download [here](https://drive.google.com/file/d/1J6fXj2c1emtJKukZaQAdRUyX4tQqYmUn/view?usp=sharing) <br>
The dataset contains details for 113,917 loans that were sanctioned between November 2005 to March 2014. The dataset contains a total 81 different attributes pertaining to each loan, some of the key variables being the loan amount, duration, borrower rate (interest rate), APR, status of the loan, completion date (if applicable), borrower's income, the listing category (reason for taking the loan), the credit score of the applicant, prosperRating (which is a unique rating given by prosper at the time of sanctioning the loan), along with personal details of the applicant such as (occupational details, employment status).
The main purpose of this project is to first explore and then summarize the nature of different variables present in the dataset that seem to affect the status of the loan and also about the relationship among multiple variables using data visualizations.


## Summary of Findings

1. Could see that ProsperScore did infact have a relation in deciding whether or not a loan was going to be defaulted. It was observed that borrowers with a higher ProsperScore tended to pay back the loans back in time without defaulting. Simillarly, as expected by logically thinking, could see that borrowers with a higher available bank credit were seen to be getting loans at a compartively lesser interest rate.

2. Observed a relationship between employment status and home ownership from the multivariate analysis to see the effect on interest rate and available bank credit. It can be seen that employed borrowers who also own homes are considered to be financially sound (just as we would think logically) and are given loans more easily that too at lesser interest rates since they seem to also have higher amount of available bank credit than the unemployed borrowers who dont own homes! The reason for this could be that home owners can keep their house on mortgage (as a security), so that the loan amount can be recovered in case the borrower defaults to pay the loan in time!


## Key Insights

1. We saw that borrowers who completed the loans in time, tended to have high Prosper Score values.

2. We saw that interest rates were very low initially and shot up exponentially with the highest value in 2011. A steady fall was then seen in the interest rates after year 2011 onwards.

3. We also saw positive co-relation between Prosper Score Credit Score and the Available Bank credit and a negative co-relation of these variables with Expected Losses. This maybe because borrowers with financially sound background (with high bank credit available) are likely to pay of the loan in time  wand NOT tend to default while making payments and end up having a higher Credit Score. And as they would be expected to pay of the loan in time, they would not be charged-off and thereby not be expected to cause losses.

4. We saw a strong positive co-relation between Interest Rate, APR and the Estimated Loss variables which shows that for Higher Interest rates, the APR is also high but is expected to make more losses. This could be the reason why we are seeing a fall in the interest rates from 2012 onwards.

5. We saw that borrowers who are employed were charged compartively lower interest rates than people who are unemployed. The same true for borrowers who owned homes and were charged lesser rates than people who did not own homes.

6. Simillarly we saw that borrowers who were employed and had their own homes also had more amount of available bank credit than those who were unemployed and didnt have homes.



## References

1. For Pointplot, Boxplot and Regplot functions:
	https://seaborn.pydata.org/tutorial.html

2. For setting ticks and axis limits:
	https://matplotlib.org/tutorials/introductory/pyplot.html#sphx-glr-tutorials-introductory-pyplot-py

3. For heatmaps:
	https://seaborn.pydata.org/generated/seaborn.heatmap.html

4. For Pairplots:
	https://seaborn.pydata.org/generated/seaborn.pairplot.html
