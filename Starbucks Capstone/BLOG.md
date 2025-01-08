<img width="1001" alt="image" src="https://github.com/user-attachments/assets/9c87c0d7-df7b-449a-9f3e-4f20a4392f90" />

# Optimizing Marketing Strategies with Data: The Starbucks Capstone Challenge

## Introduction

In today's data-driven world, businesses thrive on understanding their customers. Starbucks, a global leader in coffee retail, offers rewards through its mobile app to engage users and enhance customer loyalty. The Starbucks Capstone Challenge presents a simulated dataset replicating customer interactions within the rewards ecosystem. By analyzing this dataset, the goal is to uncover which demographic groups respond best to specific types of offers. This analysis can help Starbucks design more personalized marketing campaigns and optimize their promotional strategies.

This blog delves into the step-by-step methodology, findings, and insights derived from the dataset, providing a comprehensive overview of how data science can refine marketing decisions.

---

## Project Definition

### Project Overview

The Starbucks Capstone Challenge provides transaction, demographic, and offer data. This dataset mimics user interactions on the Starbucks rewards mobile app, where users receive different types of offers such as:
- **BOGO** (Buy One Get One Free)
- **Discounts**
- **Informational Ads**

Each offer has a defined validity period, and users may or may not interact with these offers. The dataset simplifies real-world customer behaviors by focusing on a single product. The challenge lies in combining various data sources to determine which customer segments respond most effectively to each offer type.

### Problem Statement

The project's primary objective is to identify patterns in user behavior and evaluate which demographic groups are most likely to respond to specific types of offers. This knowledge can empower Starbucks to:
1. Personalize their offers.
2. Maximize customer engagement.
3. Drive revenue growth.

### Metrics

To measure success, the following metrics are used:
1. **Offer Completion Rate:** The percentage of users who complete an offer after receiving it.
2. **Offer View Rate:** The percentage of users who view an offer.


These metrics provide a robust framework to evaluate user interactions and assess offer effectiveness.

---

## Exploratary Data Analysis

### Data Exploration

The dataset is divided into three files:
1. **Portfolio Dataset:** Contains metadata about offers, such as type, reward, and duration.
2. **Profile Dataset:** Includes demographic information like age, gender, income, and membership date.
3. **Transcript Dataset:** Logs events such as transactions, offers received, offers viewed, and offers completed.

Initial exploration revealed key insights:
- **Age Distribution:** The age distribution is bell-shaped, with most users in middle age.
- **Gender Distribution:** There are significantly more males than females in the dataset.
- **Income Distribution:** Users are predominantly in the middle-income bracket, with peaks around $60,000 to $80,000.
- **Membership Trends:** The majority of users joined the rewards program in 2016–2017.
- <img width="1001" alt="image" src="https://github.com/user-attachments/assets/83bb8f77-e6c6-4c87-80d7-510ad2eaca55" />


### Data Visualization

The visualizations provided clarity on:
- **Offer Popularity:** Which offer types (BOGO, Discount, or Informational) are most frequently completed.
- <img width="673" alt="image" src="https://github.com/user-attachments/assets/8ec081be-ee7c-4b62-a531-d4555e2e6075" />
- 
- **Time Series Analysis:** Patterns in user activity and offer completions over time.
- <img width="934" alt="image" src="https://github.com/user-attachments/assets/7ac92c3c-bb17-4855-8ca5-32c868eea28f" />
- <img width="898" alt="image" src="https://github.com/user-attachments/assets/ac6c3d11-d2b5-41ca-9e39-d3c5d646794e" />


---

## Deep Analysis and Startegy Summary

### Insights and Evaluation

**Offer Type Effectiveness:**
- **BOGO Offers:** Most popular and effective among young adults (ages 18–30) with higher incomes ($70,000–$120,000).
- <img width="885" alt="image" src="https://github.com/user-attachments/assets/d22bc6b0-7c20-4ea9-9cb1-f48b33f11e99" />
- <img width="883" alt="image" src="https://github.com/user-attachments/assets/7a53ee43-9c19-408c-acd2-7539da201c4b" />

- **Discount Offers:** Appealing to middle-aged adults (ages 31–60) across all income levels, particularly those managing household budgets.
- <img width="893" alt="image" src="https://github.com/user-attachments/assets/ef9c023c-b2d0-4853-8839-c9357cbdf487" />
- <img width="886" alt="image" src="https://github.com/user-attachments/assets/47e26ccb-9098-43b6-8b8b-4e6e03d2a3bf" />

- **Informational Offers:** Engages older adults (ages 61–100), providing value without the immediate pressure of purchase completion.

**Demographic Trends:**
- **Age:** Completion rates improve after age 35, making this group a priority for targeted campaigns.
- <img width="650" alt="image" src="https://github.com/user-attachments/assets/e2ebfa16-37e0-4919-b588-75dab728b998" />

- **Gender:** Females are more likely to complete offers than males, despite similar view rates.
- <img width="637" alt="image" src="https://github.com/user-attachments/assets/65131052-a668-4a63-9a9e-6275907bc4d7" />

- **Income:** Engagement peaks in the middle-income range ($50,000–$90,000), while higher-income users demonstrate better completion rates.
- <img width="646" alt="image" src="https://github.com/user-attachments/assets/b5d7bb6e-9f82-45d0-a89c-4f8fb753948b" />

### Correlation Analysis

- **Transactions:** Positively correlated with offer completions, suggesting active app users are more engaged.
- **Membership Tenure:** Slightly correlated with offer engagement, as long-term members show more consistent interaction.
- **Income:** Shows a minor correlation with completion rates, aligning with higher affordability.
- <img width="716" alt="image" src="https://github.com/user-attachments/assets/f658b8ca-c0f3-4961-9117-d27a7d32451a" />


## Summary of Findings

- **BOGO Offers for Higher-Income Young Adults:**
- Target Group: Individuals in the age group of 18-30, particularly those with incomes in the higher brackets (70k-120k).
- Rationale: This demographic shows a rising trend in both BOGO offer view and completion rates as income increases. Young adults with higher disposable incomes may be more incentivized to take advantage of BOGO offers.arget individuals aged 18–30 with incomes between $70,000–$120,000.
- 
- **Discount Offers for Middle-Aged Adults:** 
- Target Group: Individuals within the age groups of 31-60, across all income brackets.
- Rationale: Consistently high completion rates for discount offers in these age groups suggest that middle-aged adults, who might be managing household budgets, find direct discounts more appealing and actionable.
- 
- **Informational Offers for Older Adults:** 
- Target Group: Individuals in the age group of 61-100.
- Rationale: Older adults show a gradual increase in engagement with informational offers, particularly as they move into higher age brackets. Informational content may be valuable for this demographic, providing insights or awareness about products which can lead to informed purchasing decisions without the immediate pressure of completing a sale.

---

## Machine Learning Modeling

### Data Preprocessing

Steps taken include:
1. Cleaning missing demographic data.
2. Encoding categorical variables (e.g., gender, offer type).
3. Normalizing numerical features such as income and transaction amounts.
4. Gnerate Labels based on people's response to different offers
- <img width="809" alt="image" src="https://github.com/user-attachments/assets/f337098a-468f-469d-b13a-7cca95564242" />


### Implementation

Data integration was performed to merge the datasets, creating a unified dataset for analysis. The methodology included:
- Filtering irrelevant events.
- Linking offers to user demographics.
- Aggregating user activity to analyze behavior trends.

### Refinement

To ensure reliable results:
- Cross-validation was used for robustness.
- Hyperparameters were optimized for machine learning models.

### Model Evaluation and Expected Outcomes

-The models used for predicting offer interactions and completions include decision trees and random forests, chosen for their interpretability and robustness. Here’s how the results were evaluated:
-- 1.	Precision and Recall: High precision indicates the model correctly identifies users likely to engage with offers, while recall ensures a wide coverage of potential responders.
-- 2.	F1 Score: A balance between precision and recall, providing a holistic view of model performance.
-- 3.	Accuracy: Measures the overall correctness of the model but can be biased due to imbalanced data.

### Evaluation
- The result is showing incredibly high accuracy to both training and test dataset, with membership years to be the most important features
- <img width="508" alt="image" src="https://github.com/user-attachments/assets/e08a4082-9e7d-47fd-9ccf-2898f4c8d84b" />

- The goal of the model is to output probabilities for each of the offer category, and users can set up threshold as their need so that person is not limited to receive only one offer, if the probability score pass the threshold for a certain offer type, they can receive multiple of them.
- <img width="878" alt="image" src="https://github.com/user-attachments/assets/4e8db2d6-5fc2-4489-b11c-de2b8500edc5" />

---

## Conclusion

### Reflection

This project demonstrates how data-driven decisions can optimize marketing strategies. By understanding customer behavior, Starbucks can better tailor their offers to different demographics, improving engagement and revenue.

Challenges included handling missing data and balancing model complexity with interpretability. Nevertheless, the findings highlight the potential of targeted promotions.

### Improvement

Future enhancements could include:
- Focus on the goal of revenue maxmizing and also take cost into consideration.
- Testing advanced machine learning models like Tensorflow and Pytorch.
- Incorporating more granular data, like time-of-day activity trends and also geography data.

---

This analysis underscores the power of data science in shaping marketing decisions and driving customer satisfaction. By tailoring campaigns to specific groups, Starbucks can achieve both loyalty and growth.
