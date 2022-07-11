# AWS Free Tier usage alerts using AWS Budgets

## Task:

1. Create a cost budget
2. Create a usage budget

NB: Include Budget alarm at your preferred threshold.


TO CREATE A COST BUDGET

I signed in to the AWS Management Console and open the AWS Cost Management console 

In the navigation pane, I choose Budgets.

At the top of the page, I choose Create budget.

For Choose budget type, I choose Cost budget. Then, selected Next.

Under Set budget amount, for Period, I choose how often I want the budget to reset the actual. I selected Monthly for every month.

For Budget effective date, I choose Recurring budget for a budget that resets after the budget period.

![Cost Budget](Images/Images/CB1.jpg)

For Budgeting method, I selected the way that I want my budget amount to be determined each budget period:

I selected "Fixed"

![Cost Budget](Images/CB2.jpg)

Under Budget scoping - for Advanced options, I choose Use amortized costs

![Cost Budget](Images/CB3.jpg)

Then choose Next.

I choose Add an alert threshold.

Under Set alert threshold, for Threshold, I entered the amount that must be reached for me to be notified. 

Next to the amount, I choose % of budgeted amount to be notiﬁed when your costs exceed the threshold percentage.

Next to the threshold, I choose Actual to create an alert for actual spend. 

Under Notification preferences - for Email recipients, I entered the email addresses that I want the alert to notify. 

NB: I set two alert, one at 25% and the other at 80%


![Cost Budegt](Images/CB4.jpg)


![Cost Budegt](Images/CB5.jpg)


Then choose Next.

I Reviewed my budget settings, and then choose Create budget.

![Cost Budegt](Images/CB7.jpg)

![Cost Budegt](Images/CB8.jpg)




TO CREATE USAGE BUDGET

I signed in to the AWS Management Console and open the AWS Cost Management console 

In the navigation panel, I choose Budgets.

At the top of the page, I choose Create budget.

For Choose budget type, I choose Usage budget. Then, choose Next.

![Usage Budget](Images/UB1.jpg)

Under Choose what you’re budgeting against, for Budget against, I choose Usage type groups.

![Usage Budget](Images/UB2.jpg)

Under Set budget amount, for Period, I choose how often I want the budget to reset the actual,I selected Monthly for every month.

For Budget effective date, I choose Recurring budget for a budget that resets at the end of each budget period. 

For Budgeting method, I selected the way that i want my budget amount to be determined each budget period: I choose "Fixed"

![Usage Budget](Images/UB3.jpg)

I choose Add an alert threshold.

Under Set alert threshold, for Threshold, I entered the amount that must be reached for you to be notified.

Next to the amount, I choose % of budgeted amount to be notiﬁed when your usage exceeds the threshold percentage.

Next to the threshold, choose Actual to create an alert for actual usage.

Under Notification preferences - for Email recipients, I entered the email addresses that I want the alert to notify.

NB: I set budget alert at 80%

![Usage Budget](Images/UB6.jpg)



I choose Next.

I reviewed My budget settings, and then choose Create budget.

![Usage Budget](Images/UB8.jpg)

![Usage Budget](Images/UB9.jpg)


Guide:
https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-create.html
