# Customer Churn Analysis & Business Recommendations

**1.	Project Overview & Business Goals**

The objective of this project was to understand the key drivers of customer churn and identify early warning signals that the business can use to proactively retain users. Customer churn represents a direct loss of recurring revenue, and identifying leading indicators of churn enables earlier and more cost-effective interventions.

The business goals were to:

- Identify behavioral and service-related factors associated with churn
-	Develop actionable metrics that can be monitored regularly
  	Provide clear, data-driven recommendations to reduce churn and improve retention

To achieve this, account information, user activity data, and customer support data were integrated to form a comprehensive view of customer behavior.

**2. Summary of Work Undertaken**

Three datasets were used:

-	Account information: subscription plan, pricing, and churn status
-	User activity: event types, frequency of engagement, and recency
-	Customer support: support tickets, channels, and resolution time

The work involved:

- Data validation and cleaning to ensure consistency across datasets
- Feature engineering, including:
  - Total user events – engagement intensity
  - Days since last activity – how many days have customers been inactive?
  - Activity days – consistency over time
  - Average support resolution time
  - Revenue at risk per paid plan 
-	Data integration to create a unified customer-level dataset
- Exploratory analysis to assess relationships between engagement, support experience, and churn

**3. Key Findings**

**Finding 1: User Engagement Is the Strongest Predictor of Retention**
- Retained users exhibit significantly higher activity levels than churned users
- On average, retained users have approximately four times more recorded events
- Churn rates decrease sharply as engagement increases

Insight: Even modest increases in user engagement are associated with substantial improvements in retention.

**Finding 2: Inactivity Precedes Churn**
- Churned users show much longer periods of inactivity prior to leaving
-	The mean number of days since last activity among inactive users is approximately 66 days, with a median of 58 days
-	Prolonged inactivity is a strong early signal that a user is at risk of churn

Insight: Churn is rarely sudden; it is typically preceded by disengagement.

**Finding 3: Support Resolution Time Matters More Than Ticket Volume**
- The number of support tickets alone does not strongly predict churn
-	Churned users experience longer support resolution times than retained users within the same subscription plans
-	The overall average resolution time is approximately 10.2 hours, with greater variability among free-plan users

Insight: Support quality and speed, rather than frequency of contact, influence customer retention.

**Finding 4: Free and Low-Engagement Users have the Highest Risk**
- Free-plan users exhibit the highest churn rates
-	Users with very low activity levels consistently show the highest likelihood of churn across all plans

Insight: Early engagement and onboarding represent the largest opportunity for churn reduction.

**4. Key Metric to Monitor**

**Primary Metric: Days Since Last Activity**
This metric is recommended as the primary leading indicator of churn because:
- It changes before churn occurs
-	It captures disengagement directly
-	It is easy to monitor and operationalize

A threshold of 30–45 days of inactivity is suggested as an early warning trigger for intervention.

**Supporting Metrics**
- Churn rate
-	Average support resolution time by plan
-	Average total user events
-	Percentage of users active within the last 30 days

**5. Recommendations to the Business**
1.	Implement an Early-Warning Churn System
  - Flag users who have been inactive for 30–45 days
  - Trigger automated or personalized re-engagement efforts
2.	Strengthen Early User Engagement
  - Improve onboarding experiences, particularly for Free and Basic users
   - Encourage at least 2–3 meaningful actions during the initial usage period
3.	Prioritize Support Speed for At-Risk Users
  - Fast-track support tickets for inactive or high-value users
  - Introduce resolution-time SLAs aligned with churn risk
4.	Align Teams Around Engagement Metrics
  - Use shared metrics across product, support, and marketing teams
  - Focus on preventing disengagement rather than reacting to churn

**6. Conclusion**

The analysis shows that customer churn is driven primarily by disengagement rather than dissatisfaction alone. Prolonged inactivity is the strongest early warning signal, while faster support resolution contributes positively to retention. By monitoring leading engagement metrics and intervening earlier, the business can meaningfully reduce churn and protect recurring revenue.

