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
 
  Before splitting the control and treatment groups which by the way use random sampling to ensure that we eliminate bias in which the results of A/B testing will be representative of the entire  
  population. It's important when we designing our experiment to consider a few things :

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
 
  Before we run any A/B test, we need to have a clear and specific hypothesis about what we want to test and why. In A/B testing, the null hypothesis (H0) states that there is no difference 
  between the control and treatment groups, and observed results are purely by chance. The alternative hypothesis (Ha) states that there is a significant difference between the control and test 
  treatment groups.

- **Run the experiment**

  We should run your experiment long enough until we reach the desired sample size and duration, and avoid making any changes or interruptions during the experiment.
    
- **Analyzing the results**.

  After run the experiment and collect the data , it is important to analyze the results of the A/B testing carefully and to use statistical techniques to determine whether the results are 
  statistically significant. We should also look for any patterns, trends, or anomalies in the data that may explain the results.

- **Draw valid conclusions.**

  To draw valid conclusions from the  results and decide what actions to take. We should compare the results with our hypothesis and see if they support or reject it. And we ensure that our 
  final result doesn't skew by the impact of **Novelty Effect and Change Aversion** in which it hurts the validity of the test result. We should also consider the practical implications and 
  limitations of the test, such as :  the cost, time , and impact of implementing the winning version.

## Business Insights

- For **The Sign Up Banner** adjustments , we faced some problems in concluding the final result of the test that led us to raise the level of significance 
  and re-do the test again in order to gain accurate results. Even though a 2% increment in the conversion rate of the sign up has a positive impact , in this particular case it might have 
  happened due to the random chance. Moreover , it is not the desired effect size the business was looking for which is 5% , and definitely not when the first test result itself is doutable.

- For **The Homepage** adjustments , 6% uplift in the click-through-rate is a good difference to consider , especially when the experiment ran for 2 weeks. Therefore , we can say that the new 
  homepage design helped in improving the CTR more than the old , in which it's very unlikely that the difference happened due to pure chance alone. Also ,  we observed that these changes to the 
  homepage helped in slightly making the visitors more engaging for 50 seconds on the average and that's a sign of positive reaction toward the new design.


- For **Introducing More Payment Options** , most of the treatment users used the postpaid methods and ignored the other payment options , and that maybe what called the novelty effect in which 
  the users interact with the feature just because it’s new rather than the legitimate user interaction during an A/B test.and this of course would skew test results , in this cases it's better 
  for run the experiment for longer time in order to allow for more time for these users to cool down from any initial positive reaction or spike of interest due to a change that was introduced 
  as part of a treatment.

- For **Product Description Pages** adjustments , the CTR and engagement time in the treatment have declined. And to ensure the validity of this result we should check the segments of the 
  new/existing users because in some cases what lead this is what called change aversion when an affectionate users engage less with the experiment as they were used to the previous way of doing 
  things and they don’t like that their workflows got disrupted. 
  Overtime, they will likely get used to the new design and re-engage with the brand again as usual.

  ##  References

  - [A/B Testing Experimental Design Project File](https://github.com/hayasalman/e-commerce-website-ab-test/blob/main/_AB%20Testing%20Experimental%20Design.ipynb)

