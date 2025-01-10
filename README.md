
#Impact of Subscription Periods on Purchase Behavior#

This README outlines the steps for the A/B test insights, and the test was conducted to compare the performance of annual (control) and monthly (test) subscription plans. The goal was to determine the optimal default subscription period.

#Download the datasets
In order to reproduce the analysis, download the following datasets:
experiment_enrollment: determines whether Wistia accounts should be considered as well as the default plan shown
account_info: includes characteristics about the account including information about first trials, first purchases, and plans
page_views: details which path the Wistia app occurred for the account

#Analyze in Python
I created the analysis in Python (Jupyter Hub) and used SQLite within Python to merge data and create metrics. I pulled new customers that are analyzable, filtered for accounts enrolled on the /account/plans page and determined whether they were converted or not. I saved the results as an output to call in the subsequent SQL queries.

A/B Test on Subscription Period Options
Next, I separated the conversion rates by the groups and noted that the A/B test was not statistically significant. 

Subscription Period Options by Company Size
I developed a query that checked the conversion rates by company size and analyzed the percentages of total accounts by company size. I showed the conversion rates by default subscription period shown and company size in a data visualization. 

Trial Usage Conversions
I created a SQL query that pulls conversion rates by trial usage, shown in a data visualization. 

Trial Usage by Company Size
Finally, I wrote a query that shows the percentages of total accounts using trials for each company size.

Slide Deck
I synthesized the results and recommendations into a Google Slide Deck.

![image](https://github.com/user-attachments/assets/297586da-8e6f-44d5-bfaf-42388425abb5)
