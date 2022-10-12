
Martin Viera Schiavi, Matias Nuñez Franco

Coderhouse

DataScience Proyect


credit_card_churn.csv: file with database


Introduction: Credit cards are a good source of income for banks due to the different types of fees they charge, such as annual fees, balance transfer fees, cash advance fees, late payment fees, and foreign transaction fees, among others.

Some fees are charged to all users, regardless of usage, while others are charged under certain circumstances.

Customers abandoning credit card services would be a loss to the bank, so the bank wants to analyze customer data and identify those who abandon credit card services and the reasons for doing so, so that the bank can improve in those areas.

A churn model is a mathematical representation of how churn affects your business. Churn calculations are built from existing data (the number of customers who abandoned your service during a given time period). A predictive churn model extrapolates this data to show churn rates of potential customers in the future.

Churn (also known as customer defection) is a problem for subscription companies. When your revenue is based on recurring monthly or annual contracts, every customer that leaves puts a dent in your cash flow. High retention rates are vital to your survival. What if we told you that there is a way to predict, at least to some extent, how and when your customers will cancel?

Creating a churn prediction model will help you make proactive changes to your retention efforts that reduce churn rates. Understanding the impact of churn on your current revenue goals and making predictions about how to manage those issues in the future also helps you stem the flow of lost customers. If you don't take action against churn now, any business growth you experience will not be sustainable.

Comprehensive customer profiles help you see what types of customers are canceling their accounts. Now is the time to find out how and why they churn. Ask yourself the following questions to learn more about the pain points in your product and customer experience that cause customers to decide to churn.

What is churn? Customer churn (or customer attrition) is the tendency of customers to abandon a brand and stop being paying customers of a given company. The percentage of customers who stop using a company's products or services over a given period of time is called the customer churn rate (attrition). One way to calculate the attrition rate is to divide the number of customers lost during a given time interval by the number of customers acquired, and then multiply that figure by 100%. For example, if you have acquired 150 customers and lost three in the past month, your monthly churn rate is 2%.

The churn rate is a health indicator for companies whose customers are subscribed and pay for services on a recurring basis, so a customer remains open to more interesting or advantageous offers. In addition, each time their current engagement ends, customers have the opportunity to reconsider and choose not to continue with the company. Of course, some natural churn is inevitable, and the figure differs from industry to industry. But having a higher churn figure than that is a definite sign that a company is doing something wrong."

There are many things brands can do wrong, from complicated onboarding where customers are not given easy-to-understand information about product usage and capabilities, to poor communication, e.g., lack of feedback or delayed responses to queries. Another situation: Long-time customers may feel unappreciated because they do not receive as many bonuses as new customers.

Objective Explore and visualize the data set. Build a classification model to predict whether or not the customer will drop out. Optimize the model using appropriate techniques Generate a set of ideas and recommendations to help the bank.

Problem Does income have any effect on dropout? Does gender have any relationship with dropout? What are the signs of attrition?

Members Martin Viera Matias Franco

Problem Indication of the source of the dataset and the selection criteria (Data Acquisition)

Dataset https://www.kaggle.com/code/xavier14/predicting-churn-with-tree-based-models

Data Dictionary CLIENTNUM: Client number. Unique identifier for the customer holding the account

Attrition_Flag: Internal event (customer activity) variable - if the account is closed then "Attrited Customer" else "Existing Customer"

Customer_Age: Age in Years

Gender: Gender of the account holder

Dependent_count: Number of dependents

Education_Level: Educational Qualification of the account holder - Graduate, High School, Unknown, Uneducated, College(refers to a college student), Post-Graduate, Doctorate.

Marital_Status: Marital Status of the account holder

Income_Category: Annual Income Category of the account holder

Card_Category: Type of Card

Months_on_book: Period of relationship with the bank

Total_Relationship_Count: Total no. of products held by the customer

Months_Inactive_12_mon: No. of months inactive in the last 12 months

Contacts_Count_12_mon: No. of Contacts between the customer and bank in the last 12 months

Credit_Limit: Credit Limit on the Credit Card

Total_Revolving_Bal: The balance that carries over from one month to the next is the revolving balance

Avg_Open_To_Buy: Open to Buy refers to the amount left on the credit card to use (Average of last 12 months)

Total_Trans_Amt: Total Transaction Amount (Last 12 months)

Total_Trans_Ct: Total Transaction Count (Last 12 months)

Total_Ct_Chng_Q4_Q1: Ratio of the total transaction count in 4th quarter and the total transaction count in 1st quarter

Total_Amt_Chng_Q4_Q1: Ratio of the total transaction amount in 4th quarter and the total transaction amount in 1st quarter

Avg_Utilization_Ratio: Represents how much of the available credit the customer spent
