# Identity and Access Management (IAM)

## Working in Billing Unit

The image below shows two employee in the finance unit. They are to be granted workspace on AWS. 

![ass1_1](/images/ass1_1.png)

I created two user name;
FinanceManager
FinanceUser

I created two User group;
BillingFullAccessGroup
BillingViewAccessGroup

I then attached the FinanceManager to the BillingFullAccessGroup and FinanceUser to BillingViewAccessGroup

Perform the following task as described on the attached image


![ass1_2](/images/ass1_2.png)

I followed four steps to perform the task in the attached image, they include:

I activated the access to billing data on my AWS account
I created IAM policies that grant permissions to the billing data
I attached billing policies to your user groups
I then finally tested access to the billing console


Below is a detailed explanation of the processed followed

Activation of the access to billing data on my AWS account

I signed into my AWS Management Console with my root account credentials
On the navigation bar, I choose account name, and then choose My Account.
Next to IAM User and Role Access to Billing Information, I then choose Edit.
I selected the Activate IAM Access check box to activate access to the Billing and Cost Management console pages.
I then choose Update.



To create IAM policies that grant permissions to the billing data

I signed into the AWS Management Console as a user with administrator credentials.
In the navigation pane, I choose Policies, and then choose Create policy.
On the Visual editor tab, I choose a service to get started. Then choose Billing.
I then followed these steps to create two policies:

For Full access Policy

I choose select actions and then select the check box next to All Billing actions (aws-portal:*). 
I choose Review policy.
On the Review page, next to Name, I typed BillingFullAccess, and then choose Create policy to save it.

For Read-only access Policy

I choose Select actions and then select the check box next to Read.
I choose Review policy.
On the Review page, for Name, I typed BillingViewAccess. Then choose Create policy to save it.


To attach billing policies to your user groups

In the navigation pane, I choose Policies to display the full list of policies available to your AWS account. To attach each policy to its appropriate user group, I followed these steps:
For Full access Policy
In the policy search box, I typed BillingFullAccess, and then selected the check box next to the policy name.
I choose Actions, and then choose Attach.
In the identity (user, user group, and role) search box, I typed BillingFullAccessGroup, selected the check box next to the name of the user group, and then choose Attach policy.

For Read-only access Policy

In the policy search box, I typed BillingViewAccess, and then selected the check box next to the policy name.
I choose Actions, and then choose Attach.
In the identity (user, user group, and role) search box, I typed BillingViewAccessGroup, selected the check box next to the name of the user group, and then choose Attach policy.
I then Sign out of the console


To test billing access by signing in with both test user accounts

I used my AWS account ID, my IAM user name, and password to sign in to the IAM console.


For Full access

I signed in to my AWS account as the user FinanceManager.
On the navigation bar, I choose FinanceManager@<account alias or ID number> , and then choose My Billing Dashboard.
I browsed through the pages and choose the various buttons to ensure that i have full modify permissions.

For Read-only access

I signed in to my AWS account as the user FinanceUser.
On the navigation bar, I choose FinanceUser@<account alias or ID number>, and then choose My Billing Dashboard.
I browse through the pages. I then notice that i can display costs, reports, and billing data with no problems. However, when i choose an option to modify a value, i received an Access Denied message. 


Below is a scrrenshoot of the FinanceManager Account and FinanceUser Account

FinanceManager

FinanceUser


Note:
At the end of the lab, you should perform clean up operations.




Guides:

https://docs.aws.amazon.com/IAM/latest/UserGuide/tutorial_billing.html
