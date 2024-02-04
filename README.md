# Sebastian's portfolio
Data Analytics Portfolio

# [Project 1: FoodHub Data Analysis](https://github.com/sebtor100/Exploratory-Data-Analysis-) 
![Exploratory-Data-Analysis-EDA-steps-source-7](https://github.com/sebtor100/SEB_portfolio/assets/122765165/090d49c7-1b44-4d27-87ac-2fbebee2e30b)

## Overview

The project focuses on analyzing the data from FoodHub, a food aggregator company, to enhance customer experience and improve business strategies. The data contains information about different food orders, including order details, customer ratings, and various time-related metrics.

## Conclusion and Recommendations
## Conclusions:
- The top 4 restaurants (Blue Ribbon Fried Chicken, Blue Ribbon Sushi, Shake Shack, The Meatball Shop) should be prioritized for promotions and marketing efforts.
- Popular cuisine types (American, Japanese, Italian) can be highlighted in advertisements to attract more customers.
- Mean delivery time on weekends is slightly higher, optimization strategies can improve customer satisfaction.
## Recommendations:
- Collaborate with top restaurants for exclusive promotional deals.
- Create cuisine-specific promotions based on popular cuisine types.
- Optimize delivery processes during weekends to reduce mean delivery times.
- Introduce special offers for high-cost orders to incentivize customers.
- Encourage customers to provide feedback and ratings for better service quality.

#  [Project 2 : Machine-Learning-Potential-Customers-Prediction](https://github.com/sebtor100/Machine-Learning-Potential-Customers-Prediction)
![Illustration-of-random-forest-trees](https://github.com/sebtor100/SEB_portfolio/assets/122765165/73c9b1af-6d9a-4218-abbc-c02d3eccf72e)

## Context
The EdTech industry has experienced significant growth in the past decade, with the Online Education market projected to be worth $286.62 billion by 2023, exhibiting a compound annual growth rate (CAGR) of 10.26% from 2018 to 2023. The surge in online education, driven by features such as ease of information sharing, personalized learning experiences, and transparent assessment, has made it a preferred choice over traditional education. The Covid-19 pandemic has further accelerated the growth of the online education sector, attracting new customers and giving rise to numerous companies in the industry.

Amidst this growth, ExtraaLearn, an early-stage startup, focuses on providing programs on cutting-edge technologies to students and professionals, aiding them in upskilling/reskilling. As the company generates a substantial number of leads regularly, one of its challenges is identifying which leads are more likely to convert into paid customers. As a data scientist at ExtraaLearn, your task is to analyze the leads data and build a machine learning model to identify potential conversions, understand the factors influencing the lead conversion process, and create a profile of leads likely to convert.

## Objective
The primary objectives of the ExtraaLearn project are as follows:

1. Analyze and build an ML model to identify leads more likely to convert to paid customers.
2. Identify the key factors influencing the lead conversion process.
3. Create a profile of leads that are likely to convert.

## **Conclusion**

- The best model we have got so far is the Gradient Boost Classifier model with modified weights which is giving nearly ~ 87% recall for class 1 on the test data.
- The company should use this model to know beforehand which lead is going to be converted and act accordingly.
-  `firstinteraction_website`, `time_spend_website`, `Profile_completed_Medium` and `age`seem to be the most important features.
- The overall lead conversion rate is 29.9%, which provides a baseline to compare against.
- Leads who first interact via the website have significantly higher conversion rates (45.6%) compared to mobile app (10.5%). Focusing marketing and resources on driving more website traffic could improve overall conversion.
- Time spent on the website is highly correlated with conversion, with converted leads spending a median of 789 mins vs 317 mins for non-converts. Keeping leads engaged onsite longer should increase conversion likelihood.

## **Recommendations**

- Since time spent on the website emerged as the most important factor in predicting lead conversion, ExtraLearn should prioritize marketing strategies
that engage visitors and extend their website session lengths:

    1. Optimize site architecture and navigation to make it easy for visitors to find relevant content and navigate to related topics/pages. This encourages further exploration.
    2. Implement advanced tracking analytics to identify popular site content as well as pages with high exit rates. Refine or enhance high-interest areas; modify or remove content that fails to engage.
    3. Integrate interactive elements like assessments, quizzes, calculators, etc. that lead visitors to spend more time providing information relevant to course matching.
    4. Retarget visitors via ads/email campaigns who leave the site before hitting key engagement thresholds personalized to vertical/offering. Remind them of content still to explore.
    5. Test modular course content samples accessible to visitors without requiring lead forms upfront. This demonstrates value from courses before asking for visitor info.

  The core focus should be providing sticky website experiences tailored to visitor vertical/persona that drive session times upward and subsequently increase the likelihood of lead conversion. An integrated analytics and testing framework will enable iterating on the most effective engagement strategies over time.

- Given the goal is to maximize conversion of potential customers, continue using the Gradient Boosting model in production to score incoming leads. Use the lead scores to focus sales efforts on those most likely to convert.
- Put additional resources into the website experience, features, content etc to drive longer session times. This has a direct impact on conversion.
- Analyze what web pages and content converts spend more time on and identify opportunities to better engage them during the session.
- Establish feedback loops to continually collect data on new leads, retrain models periodically, and improve conversion performance over time.
- Set up A/B testing frameworks to test changes to web pages, outreach campaigns, pricing models etc. and their impact on conversion rates.


#  [Project 3 :Applied-Data-Science-Loan-Prediction-](https://github.com/sebtor100/Applied-Data-Science-Loan-Prediction-)
Loan Prediction Techniques
![hyperparam_intro_rf_only2](https://github.com/sebtor100/SEB_portfolio/assets/122765165/b31a6af2-6307-41c7-baa6-f95f85cda708)

# Loan Default Prediction
## Problem Definition
## The Context:
In the contemporary landscape of retail banking, a significant proportion of profits stems from interest accrued through home loans, primarily extended to customers with regular or high income. However, the specter of loan defaulters poses a considerable threat to banks, as non-performing assets (NPAs) can substantially erode profits. Therefore, the approval process for these loans is a multifaceted challenge, traditionally relying on manual assessments of applicants' creditworthiness. Yet, this approach is not only labor-intensive but also susceptible to human errors and biases.

Recognizing the limitations of heuristic-based automation attempts, many banks are turning to the power of data science and machine learning to revolutionize the loan approval process. The goal is to develop machine learning models capable of learning the intricacies of the approval process, eliminating biases, and enhancing efficiency. However, a crucial consideration in this endeavor is to ensure that the machine does not inherit biases ingrained in the historical human approval process.

## The objective:
The primary objective is to build a classification model capable of predicting clients likely to default on their loans. Additionally, the model should provide actionable recommendations to the bank regarding crucial features to consider during the loan approval process.

## Conclusions:
Multiple machine learning models were built and evaluated, with the tuned Random Forest model achieving the best performance on key metrics like F1 score. It had scores of 0.95 for the non-default class and 0.78 for the default class.
The models were able to predict loan defaults with decent accuracy, outperforming a manual lending process. Key drivers of default risk were identified such as number of delinquencies, debt-to-income ratio and credit history length.
There is still room for improvement in model performance, especially for the minority default class. Additional applicant data could further boost accuracy.
## Recomendations:
The tuned Random Forest model should be deployed as the final solution due to its robust performance, interpretability and ability to balance precision and recall.
A two-step loan approval process is recommended. First, applicants should be classified as likely defaulters or not using the Random Forest model. Then a second regression model can predict uitable loan amounts for non-defaulters.
The key drivers of default risk should inform lending policy and credit worthiness evaluation during the manual underwriting process as well. Applicants with long credit history and low debt ratios should be preferred.
Additional data like income stability, payment behavior with other lenders, personal obligations etc. should be collected in loan applications wherever possible. This can feed into incremental model improvements over time.
Appropriate thresholds need to be set for default probability beyond which loans get rejected. These cut-offs require business input based on risk appetite.

# [Project 4: Boston House Price Prediction]([https://github.com/sebtor100/Exploratory-Data-Analysis-](https://github.com/sebtor100/Boston-House-Price-Prediction) 

#  [Project 5 :Shinkansen-Bullet-Train-in-Japan](https://github.com/sebtor100/Shinkansen-Bullet-Train-in-Japan)
Customer Satisfaction Prediction Techniques 
![Japanese-shinkansen-train-e1572594353517-825x550](https://github.com/sebtor100/SEB_portfolio/assets/122765165/f56ab095-b7a6-4ed2-8115-02d0710d911d)

## About

This problem statement is based on the Shinkansen Bullet Train in Japan, and passengers’ experience with that mode of travel. This machine learning exercise aims to determine the relative importance of each parameter about their contribution to the passengers’ overall travel experience. The dataset contains a random sample of individuals who traveled on this train. The on-time performance of the trains along with passenger information is published in a file named ‘Traveldata_train.csv’.  These passengers were later asked to provide their feedback on various parameters related to the travel along with their overall experience. These collected details are made available in the survey report labeled ‘Surveydata_train.csv’.

In the survey, each passenger was explicitly asked whether they were satisfied with their overall travel experience or not, and that is captured in the data of the survey report under the variable labeled ‘Overall_Experience’. 

The objective of this problem is to understand which parameters play an important role in swaying passenger feedback towards a positive scale. You are provided test data containing the travel data and the survey data of passengers. Both the test data and the train data are collected at the same time and belong to the same population.


## Goal:
The goal of the problem is to predict whether a passenger was satisfied or not considering his/her overall experience of traveling on the Shinkansen Bullet Train.

## Dataset: 

The problem consists of 2 separate datasets: Travel data & Survey data. Travel data has information related to passengers and attributes related to the Shinkansen train, in which they traveled. The survey data is aggregated data of surveys indicating the post-service experience. You are expected to treat both these datasets as raw data and perform any necessary data cleaning/validation steps as required.

The data has been split into two groups and provided in the Dataset folder. The folder contains both train and test data separately.

•	Train_Data
•	Test_Data

Target Variable: Overall_Experience (1 represents ‘satisfied’, and 0 represents ‘not satisfied’)

The training set can be used to build your machine-learning model. The training set has labels for the target column - Overall_Experience.

The testing set should be used to see how well your model performs on unseen data. For the test set, it is expected to predict the ‘Overall_Experience’ level for each participant.

## Data Dictionary:

All the data is self-explanatory. The survey levels are explained in the Data Dictionary file.

Submission File Format: You will need to submit a CSV file with exactly 35,602 entries plus a header row. The file should have exactly two columns

•	ID
•	Overall_Experience (contains 0 & 1 values, 1 represents ‘Satisfied’, and 0 represents ‘Not Satisfied’)

## Evaluation Criteria:

Accuracy Score: The evaluation metric is simply the percentage of predictions made by the model that turned out to be correct. This is also called the accuracy of the model. It will be calculated as the total number of correct predictions (True Positives + True Negatives) divided by the total number of observations in the dataset.
 
In other words, the best possible accuracy is 100% (or 1), and the worst possible accuracy 0%. 

## Validation Accuracy Final Model: 0.9528501801229073

#  [Project 6: Amazon Product Recommendation System](https://github.com/sebtor100/Amazon-Product-Recommendation-System)
Recommendation System Techniques 
![0_lRi888vssyKrR2Ks](https://github.com/sebtor100/Sebastian_portfolio/assets/122765165/288e192f-c68e-4cc5-9838-ac3b243a5e29)

# Amazon-Product-Recommendation-System
Amazon Product Recommendation System

Welcome to the project on Recommendation Systems. We will work with the Amazon product reviews dataset for this project. The dataset contains ratings of different electronic products. It does not include information about the products or reviews to avoid bias while building the model. 

--------------
## **Context:**
--------------

Today, information is growing exponentially with volume, velocity and variety throughout the globe. This has lead to information overload, and too many choices for the consumer of any business. It represents a real dilemma for these consumers and they often turn to denial. Recommender Systems are one of the best tools that help recommending products to consumers while they are browsing online. Providing personalized recommendations which is most relevant for the user is what's most likely to keep them engaged and help business. 

E-commerce websites like Amazon, Walmart, Target and Etsy use different recommendation models to provide personalized suggestions to different users. These companies spend millions of dollars to come up with algorithmic techniques that can provide personalized recommendations to their users.

Amazon, for example, is well-known for its accurate selection of recommendations in its online site. Amazon's recommendation system is capable of intelligently analyzing and predicting customers' shopping preferences in order to offer them a list of recommended products. Amazon's recommendation algorithm is therefore a key element in using AI to improve the personalization of its website. For example, one of the baseline recommendation models that Amazon uses is item-to-item collaborative filtering, which scales to massive data sets and produces high-quality recommendations in real-time.

----------------
## **Objective:**
----------------

You are a Data Science Manager at Amazon, and have been given the task of building a recommendation system to recommend products to customers based on their previous ratings for other products. You have a collection of labeled data of Amazon reviews of products. The goal is to extract meaningful insights from the data and build a recommendation system that helps in recommending products to online consumers.

-----------------------------
## **Dataset:** 
-----------------------------

The Amazon dataset contains the following attributes:

- **userId:** Every user identified with a unique id
- **productId:** Every product identified with a unique id
- **Rating:** The rating of the corresponding product by the corresponding user
- **timestamp:** Time of the rating. We **will not use this column** to solve the current problem

![cs](https://github.com/sebtor100/Sebastian_portfolio/assets/122765165/9050234c-71e1-402e-a465-19a5b184aa1c)

### **Conclusion and Recommendations**

-----------------------------
**Conclusions:**
-----------------------------

***Baseline Model:***

*Pros:*
Simplicity: The baseline model offers a simple and quick-to-implement solution.
Benchmarking: It provides a baseline for comparison with more complex models.

*Cons:*
Accuracy: The baseline model has a higher RMSE (Root Mean Squared Error) of 1.0256, indicating lower predictive accuracy.
Limited Personalization: Lacks the ability to provide personalized recommendations.
Recommendation:
While suitable for quick comparisons, the baseline model may not deliver highly accurate or personalized recommendations.


***User-User Collaborative Filtering:***

*Pros:*
Personalization: User-User CF achieved a Precision@10 of 0.853, Recall@10 of 0.889, and F1-Score@10 of 0.871, indicating good personalization.
User Preferences: Effectively considers user preferences for recommendations.

*Cons:*
Scalability: Faces scalability issues for large datasets and is sensitive to sparsity.
Complexity: Despite good personalization, the model is sensitive to the complexity of user interactions.
Recommendation:
User-User CF is effective for smaller platforms with engaged user communities that value personalized recommendations.


***Item-Item Collaborative Filtering:***

*Pros:*
Item Similarities: Item-Item CF considers item similarities, achieving a Precision of 0.839, Recall of 0.88, and F1-Score of 0.859.
Diverse Catalogs: Effective for platforms with diverse item catalogs.

*Cons:*
Sparsity Sensitivity: Similar to User-User CF, it is sensitive to sparse data.
Cold Start: May not handle the cold start problem well, especially for new items.

Recommendation:
Suitable for platforms with a wide range of diverse items, but attention is needed for the cold start problem.

***SVD-based Collaborative Filtering:***

*Pros:*
Latent Factors: SVD-based CF incorporates latent factors, achieving a Precision@10 of 0.846 and Recall@10 of 0.798.
Personalization: Offers personalized recommendations based on latent factors.

*Cons:*
Cold Start Challenge: Faces challenges in scenarios with insufficient data, especially for new items.
Data Dependency: Requires a significant amount of data for effective training.
Recommendation:
Ideal for platforms with a substantial user-item interaction history, aiming for a high level of personalization. Mitigation strategies needed for the cold start problem.

In summary, the choice of a collaborative filtering model depends on the specific needs of the platform, considering factors such as user base size, item catalog diversity, and the availability of historical interaction data. Business stakeholders should weigh the trade-offs in terms of model complexity, scalability, and personalization to make informed decisions. Regular model evaluation and monitoring are essential for maintaining recommendation system performance over time.

**Business Recommendations:**

**Combine Collaborative Filtering Models:**

1. Consider combining user-user, item-item, and SVD-based models for a hybrid approach, leveraging the strengths of each. This can enhance recommendation accuracy and robustness.
Cold Start Strategy:

2. Implement content-based methods to address the cold start problem. Use metadata and user features to make initial recommendations before sufficient interaction data is available.
Dynamic Personalization:

3. Implement real-time personalization to adapt to changing user preferences. Continuously update models based on user interactions and feedback.
A/B Testing:

4. Conduct A/B testing to evaluate the performance of different recommendation models. Gather user feedback and iterate on models for continuous improvement.
User Engagement Strategies:

5. Implement strategies to encourage user engagement, such as personalized notifications, discounts on recommended items, or gamification elements. This can enhance user satisfaction and interaction.

***Scalability Considerations:***

1. Monitor system performance as the user base grows. Explore distributed computing solutions for handling scalability issues associated with collaborative filtering models.

In conclusion, a well-balanced approach that considers the strengths and limitations of different recommendation models, combined with thoughtful business strategies, can lead to an effective and engaging recommendation system. Continuous monitoring, user feedback, and adaptation are key elements in maintaining the relevance and performance of the recommendation system over time.

