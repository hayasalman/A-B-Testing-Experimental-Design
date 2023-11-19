## A/B Testing Experimental Design

![AB_test](https://github.com/hayasalman/e-commerce-website-ab-test/assets/71796909/1db2a706-f3df-419f-b25d-d73cc7db2283)

## Overview

Through the birth of the internet, A/B testing went digital. Today, it’s used to compare two versions of an app, a website, or even things like newsletters and email subject lines 
to determine which is more effective (depending on a specific metric).

## About the dataset

*All the datasets stored as CSV file and can be accessed through this links :*

- [Homepage Actions](https://github.com/hayasalman/e-commerce-website-ab-test/blob/main/Datasets/ecommerce_homepage_actions.csv)
- [Homepage Session Time](https://github.com/hayasalman/e-commerce-website-ab-test/blob/main/Datasets/homepage_sessions.csv)
- [Payment Options](https://github.com/hayasalman/e-commerce-website-ab-test/blob/main/Datasets/payment_opt.csv)
- [Product Description Page Actions](https://github.com/hayasalman/e-commerce-website-ab-test/blob/main/Datasets/pdp_actions.csv)
- [Product Description Page Engagement Time](https://github.com/hayasalman/e-commerce-website-ab-test/blob/main/Datasets/pdp_engagement_time.csv)
- [Sign Up Conversions](https://github.com/hayasalman/e-commerce-website-ab-test/blob/main/Datasets/signup_conversions.csv)

  ## Coding

  -  Python Integrated Development Environment (IDE) : Jupyter Notebooks.

   **Packeges used** 
  * **pandas - numby** : used for data manipulation.
  * **matplotlib - seaborn** : used for data visualtion.

  ## Approaches & Methodologies

  - **Define the objective of the test.**

  This could be increasing conversion rates, increasing click rates, improving the user experience, etc.
    
  - **Design the experiment.**
 
  Before split the control and treatment groups which by the way done use random sampling to ensure that eliminate bias as we want the results of A/B testing to be representative of the entire population, we should take in consideration a few things:

  **The units of diversion.**
      
    It is an iterative process to try out some decisions for unit of diversion , it could be :
         
    - **user_id based**: user consistency if they log in.
            
    - **cookie-based**: user consistency if they use the same browsers and devices.
            
    - **event-based**: least user consistency because the users may be mixed into the two groups.
         
  **The population.**

  It's could be one of these :

  - **Intra-user experiment**: exposing the same user to the feature being on and off over time, analyzing how they behave in different time windows.

  - **Interleaved experiment**: for ranking type of applications, e.g. ranking or preferences, exposing the same user to the A and B side at the same time.

  - **Inter-user experiment**: A/B testing, two groups of users on the A and B side. A refinement is two cohorts of users, which match up the parameters in the two groups.
 
  **The size.**
 
  The effect size is a measure of how large or significant the difference or relationship between two groups or variables is .
  The larger the effect size, the smaller the sample size needed to detect it. 
    
  **The duration and exposure.**
    
  Determining the duration is how long to run the experiment, and exposure is what percentage of the traffic will be included for the experiments based on the averaged traffic per day.
  We also need to consider how long the experiment will be run. We must consider longer duration in order to reduce the effect of specific days or seasonality effect , and if the change
  is highly risky, then we may expose it to only a subset of the traffic, which means running the experiment for a longer time.

  - **Define the hypothesis.**
 
  Before we run any A/B test, we need to have a clear and specific hypothesis about what we want to test and why. In A/B testing, the null hypothesis (H0) states that there is no difference between the control and treatment groups,
  and observed results are purely by chance. The alternative hypothesis (Ha) states that there is a significant difference between the control and test treatment groups.
  

  - **Analyzing the results**.

  After conduct A/B test and collect the data , it is important to analyze the results of the A/B testing carefully and to use statistical techniques to determine whether the results are statistically significant.

  - **Draw valid conclusions.**

    
