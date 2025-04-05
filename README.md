# Project Description

You work as an analyst for the telecommunications operator Megaline. The company offers its customers two prepaid plans: Surf and Ultimate. The sales department wants to know which plan generates the most revenue so they can adjust their advertising budget.

You will conduct a preliminary analysis of the plans based on a relatively small customer selection. You will have data on 500 Megaline customers: who the customers are, where they are from, what plan they use, and the number of calls and text messages they sent in 2018. Your task is to analyze customer behavior and determine which prepaid plan generates the most revenue. Later, you will find in the project instructions the exact aspects of customer behavior you need to analyze. Determining which plan, on average, generates the most revenue is a question that will be addressed through statistical tests. You will find more information about this later in the project instructions section.

## Rate Description
Note: Megaline rounds seconds to minutes and megabytes to gigabytes. For calls, each individual call is rounded up: even if the call lasted only one second, it will count as one minute. For web traffic, individual web sessions are not rounded up. Instead, the monthly total is rounded up. If someone uses 1025 megabytes this month, they will be charged 2 gigabytes.

Below is a description of the rates:

Surf:

Monthly payment: $20.
500 minutes per month, 50 SMS, and 15 GB of data.
If the package limits are exceeded:
1 minute: 3 cents.
1 SMS: 3 cents.
1 GB of data: $10.

Ultimate:

Monthly payment: $70.
3,000 minutes per month, 1,000 SMS, and 30 GB of data.
If the package limits are exceeded:
1 minute: 1 cent.
1 SMS: 1 cent.
1 GB of data: $7.
Data Dictionary
In this project, you will work with five different tables.

The users table (data about users):

user_id: The user's unique identifier.
first_name: The user's first name.
last_name: The user's last name.
age: The user's age (in years).
reg_date: Subscription date (dd, mm, yy).
churn_date: The date the user stopped using the service (if the value is missing, the plan was in use when this database was retrieved).
city: User's city of residence.
plan: Plan name.

The calls table (call data):

id: Unique identifier of the call.
call_date: Date of the call.
duration: Duration of the call (in minutes).
user_id: The identifier of the user making the call.
The messages table (data about SMS):

id: Unique identifier of the SMS.
message_date: Date of the SMS.
user_id: The identifier of the user sending the SMS.
The internet table (data about web sessions):

id: Unique identifier of the session.
mb_used: The amount of data used during the session (in megabytes).
session_date: Date of the web session.
user_id: The identifier of the user.
The plans table (data about tariffs):

plan_name: Name of the tariff.
usd_monthly_fee: Monthly payment in US dollars.
minutes_included: Minutes included per month.
messages_included: SMS included per month.
mb_per_month_included: Data included per month (in megabytes).
usd_per_minute: Price per minute after exceeding the package limits (for example, if the package includes 100 minutes, the operator will charge for the 101st minute).
usd_per_message: Price per SMS after exceeding the package limits.
usd_per_gb: Price per gigabyte of extra data after exceeding the package limits (1 GB = 1024 megabytes).

## Steps to complete the project

- Step 1. Open the data file and review the general information
- Step 2. Prepare the data
- Step 3. Analyze the data
- Step 4. Test the hypotheses
The average income of Ultimate and Surf rate users differs.
The average income of users in the New York-New Jersey area is different from that of users in other regions.
