# Sebastian's portfolio
Data Analytics Portfolio

# Project 1 : FoodHub Data Analysis (https://github.com/sebtor100/Exploratory-Data-Analysis-)

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

# Project 2 : Machine-Learning-Potential-Customers-Prediction (https://github.com/sebtor100/Machine-Learning-Potential-Customers-Prediction)

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
