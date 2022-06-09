# D2C-Propensity-Model
:pinched_fingers: Can you identify the potential leads for a D2C startup?

## :question: What is propensity modeling?
Propensity modeling attempts to predict the likelihood that visitors, leads, and customers will perform certain actions. It’s a statistical approach that accounts for all the independent and confounding variables that affect said behavior.

So, for example, propensity modeling can help a marketing team predict the likelihood that a lead will convert to a customer. Or that a customer will churn. Or even that an email recipient will unsubscribe.

The propensity score, then, is the probability that the visitor, lead, or customer will perform a certain action.

## :dart: Problem Statement
A D2C startup develops products using cutting edge technologies like Web 3.0. Over the past few months, the company has started multiple marketing campaigns offline and digital both. As a result, the users have started showing interest in the product on the website. These users with intent to buy product(s) are generally known as leads (Potential Customers).

- Leads are captured in 2 ways - _Directly_ an _Indirectly_.

- Direct leads are captured via forms embedded in the website while indirect leads are captured based on certain activity of a user on the platform such as time spent on the website, number of user sessions, etc.

- Now, the marketing & sales team wants to identify the leads who are more likely to buy the product so that the sales team can manage their bandwidth efficiently by targeting these potential leads and increase the sales in a shorter span of time.

- Now, as a data scientist, your task at hand is to predict the propensity to buy a product based on the user's past activities and user level information.

## About Dataset
You are provided with the leads data of last year containing both direct and indirect leads. Each lead provides information about their activity on the platform, signup information and campaign information. Based on his past activity on the platform, you need to build the predictive model to classify if the user would buy the product in the **_next 3 months or not_**.


Data Dictionary
You are provided with 3 files - train.csv, test.csv and sample_submission.csv


Training set
train.csv contains the leads information of last 1 year from Jan 2021 to Dec 2021. And also the target variable indicating if the user will buy the product in next 3 months or not


| Variables        | Description           |
| ------------- |:-------------|
| id     | Unique identifier of a lead |
| created_at     | Date of lead dropped      |
| signup_date | Sign up date of the user on the website      |
| campaign_var (1 and 2)      | campaign information of the lead      |
| products_purchased | No. of past products purchased at the time of dropping the lead      |
| user_activity_var (1 to 12)      | Derived activities of the user on the website    |
| buy | 0 or 1 indicating if the user will buy the product in next 3 months or not    |
