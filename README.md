# Automated-Recommender-System-From-Dashboard-Insights-to-Actionable-Recommendations

The objective here is to create an automated system that generates personalized recommendations based on specific insights derived from a dashboard (in Power BI, Tableau, Google Colab, etc.). The focus is on leveraging pre-existing insights and triggering actions based on these insights.

# Steps to Build an Automated Recommender System

1. Data Extraction from the Dashboard
Retrieve the latest insights and data from your existing dashboard.

2. Recommendation Logic
Based on the extracted insights, develop logic to generate automated recommendations.

3. Triggering Actions
Automatically send alerts or messages to specific stakeholders based on the recommendations.

# Detailed Implementation

1. Data Extraction from the Dashboard
   
**Google Colab Example:**

Assuming the insights are stored in a  **CSV or a similar format**:

![image](https://github.com/user-attachments/assets/9dff42b1-c5e3-4b1b-aa63-46511bbb2277)

This code snippet loads the insights data from a CSV file into a pandas DataFrame.

**Power BI Example:**

![image](https://github.com/user-attachments/assets/f566b05c-e1dc-4ce7-8e1d-637ad2858ed1)

This code snippet retrieves report data from Power BI using its REST API and converts it into a pandas DataFrame.


**Tableau Example:**

![image](https://github.com/user-attachments/assets/3662eb54-f579-445c-b598-8d44adefae68)

This code snippet uses the Tableau Server Client library to download data extracts and load them into a pandas DataFrame.

2. Recommendation Logic
   
Once the data is extracted, the next step is to develop the logic for generating recommendations based on the insights.


![image](https://github.com/user-attachments/assets/d946ccc2-8611-4769-bc34-29acf71b02ee)

This function iterates through the DataFrame, evaluates various conditions, and generates personalized recommendations for each user.


3. Triggering Actions

After generating recommendations, the next step is to automatically send alerts or messages to stakeholders.
   
Example using Email Alerts:

![image](https://github.com/user-attachments/assets/b59c04c7-4652-4e1e-b464-250c89992f19)

This code snippet defines a function to send email notifications to stakeholders based on the generated recommendations.

Automating the Process using Airflow:

To ensure the entire process runs automatically, we can use a tool like Apache Airflow.


![image](https://github.com/user-attachments/assets/9d235801-2bfa-437b-b227-668797fcd12f)

This DAG (Directed Acyclic Graph) in Airflow automates the extraction of data, generation of recommendations, and sending of notifications.

**Conclusion**

By following these steps, you can build an automated recommender system that generates personalized recommendations based on insights from your dashboard and automatically triggers actions to support users. This system ensures timely and relevant actions are taken, improving user experience and financial management.
