Payment Funnel Analysis with SQL
<img width="683" alt="image" src="https://github.com/user-attachments/assets/95009b66-639e-4828-b658-1a5f685ba9f8" />

Case Study: Payment Funnel Analysis
Your finance team comes to you one day asking about why there are so many unpaid subscriptions. Lately, customers have been choosing or opting into a paid subscription plan, but many are not completing the process by paying for their subscription. When customers sign up for a subscription, we consider them to officially be a customer, but they aren’t considered “converted” into a paid plan until they actually pay for their subscription by completing the payment process. Because of this, the company has a less-than-desired conversion rate since many companies have started a subscription but haven’t actually paid yet. This is a huge issue for the company because we have customers who are signing up for our product but aren’t paying— which has resulted in a large loss in revenue. 


As a seasoned data analyst, you know that the finance team’s concerns are valid and worth looking into, so you immediately come up with a plan to dig into this. You meet with the product manager, and she walks you through the entire payment process. First, users have to open and enter the payment portal— and you already notice that this could be a large friction point for customers. Once inside the payment portal, they have to enter their credit card information and hit submit. It’s possible for users to hit an error here if they input incorrect or incomplete information. Then the data is sent to a 3rd party payment processing company where the credit card is actually processed. It’s also possible for users to hit an error here if the vendor has an issue processing the card. If everything is successfully completed with the vendor, they send the success message back to us, and we’re able to log the transaction as complete on our side too. 


After learning more about the business side of things and what the user sees on the frontend, you have to determine if we even have data to track all of these user events. If the data doesn’t exist, you may have to measure proxies, brainstorm a workaround, and propose new user events to track in order to have better data collection for the future. Luckily, after meeting with your frontend engineer and data engineer, you learn that all of the major payment portal user events are tracked in the payment_status_log. You immediately start brainstorming ways to determine how to measure the success of each subscriptions, and more importantly, where the friction points are. Once you develop some insights, you’ll be able to go back to the product manager with product recommendations to reduce friction and increase successful payments. This will have a large impact on revenue and get you noticed by the leadership team. 


Payment Funnel Analysis Summary
Title: Improving Conversion Rates in the Payment Funnel
Executive Summary:
This analysis investigates the high number of unpaid subscriptions within our payment funnel. By identifying and addressing the friction points, we aim to improve the conversion rate and increase revenue.

Business Problem:
The company is facing a significant issue with customers opting into paid subscription plans but not completing the payment process. This has led to a lower-than-desired conversion rate and a considerable loss in revenue.

<img width="473" alt="image" src="https://github.com/user-attachments/assets/58d46839-6bb6-4f39-b19e-fc7e60345776" />

Methodology:
Data Extraction: Utilized payment_status_log to track user events throughout the payment funnel.

<img width="469" alt="image" src="https://github.com/user-attachments/assets/f3a794af-f6c1-4f5e-a744-f186d9a4252a" />

Analysis:

Calculated conversion rates at each stage of the payment funnel.

Identified common user errors and vendor processing issues.

Analyzed the frequency of errors and their impact on conversion rates.

<img width="621" alt="image" src="https://github.com/user-attachments/assets/ca595970-c008-43f8-974a-1e105eaded44" />


Visualization: Created funnel charts and bar charts to illustrate conversion rates and error occurrences.

<img width="485" alt="image" src="https://github.com/user-attachments/assets/38832dd5-1621-4a34-b2fe-33666eb560bd" />

<img width="600" alt="image" src="https://github.com/user-attachments/assets/1b0b8943-9b9a-4473-a149-08eab3e0a6c4" />

Skills:
SQL for data extraction and analysis.

Data visualization for presenting findings.

Problem-solving to identify friction points and propose solutions.

Results:
Conversion Rate Insights: Identified that a significant drop-off occurs at the payment entry stage.

Common Errors:

User Errors: Incorrect or incomplete payment information.

Vendor Errors: Issues with the payment processing vendor.

Impact Analysis: Errors have a substantial impact on conversion rates, with user errors being more frequent but vendor errors causing more significant drop-offs.

Business Recommendations:
Improve User Experience:

Simplify the payment portal interface.

Implement real-time validation and error messages to guide users in entering correct information.

Enhance Error Handling:

Work with the vendor to reduce processing errors.

Provide clear instructions and support options for users facing issues.

Monitor and Optimize:

Continuously track user events and errors to identify new friction points.

Implement A/B testing to evaluate the effectiveness of changes.

Next Steps:
Implement the recommended changes to the payment portal.

Monitor the impact of these changes on conversion rates.

Gather feedback from users to further refine the payment process.

