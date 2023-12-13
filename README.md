# Predictive Modeling of Bike Demand for BoomBikes
##### Unveiling Market Dynamics, Identifying Key Variables, and Crafting a Strategic Roadmap for BoomBikes' Post-Quarantine Success

<div>
    <img src="https://jorg3gf.github.io/images/transport.jpg" />
</div>

# Table of Contents
1. [Introduction](#introduction)
    - 1.1 [Background](#background)
    - 1.2 [Problem Statement](#problem-statement)
    - 1.3 [Business Goal](#business-goal)
2. [Tech Used](#tech)
3. [Conclusion](#conclusion)

<a name="introduction"></a>
# 1. Introduction
<a name="background"></a>
## 1.1 Background
The bicycle-sharing industry has undergone unprecedented challenges, particularly in the wake of the COVID-19 pandemic. BoomBikes, a leading provider of shared bikes in the United States, has experienced substantial revenue declines during this period. As the nation gradually emerges from the pandemic-induced lockdown, BoomBikes recognizes the need to strategically position itself to capitalize on the anticipated surge in demand for shared bikes.

<a name="problem-statement"></a>
## 1.2 Problem Statement
To address this critical challenge, BoomBikes has enlisted the expertise of a consulting company to conduct a thorough analysis. The focus is on leveraging a comprehensive dataset that captures daily bike demand across various factors in the American market. The primary goal is to identify and understand the key factors that significantly influence the demand for shared bikes post-quarantine. The company is particularly interested in unraveling the intricate dynamics that determine how different features impact bike demand.

<a name="business-goal"></a>
## 1.3 Business Goal
The overarching business goal is to develop a predictive model for shared bike demand, utilizing available independent variables. This model will serve as a strategic tool for BoomBikes' management, enabling them to make informed decisions about adjusting business strategies to meet varying demand levels and exceed customer expectations. Moreover, the model will provide valuable insights into the dynamics of demand in a recovering market, positioning BoomBikes as a leader in the evolving landscape of shared mobility.

The journey begins with a meticulous exploration of the dataset and a thoughtful consideration of factors that may influence the demand for shared bikes. Through rigorous data preparation, model building, and evaluation, this case study aims to deliver actionable insights that will empower BoomBikes to navigate the post-COVID landscape successfully.

<a name="tech"></a>
# 2. Tech Used
- pandas
- numpy
- matplotlib
- seaborn
- sklearn
- statsmodels

<a name="conclusion"></a>
# 3. Conclusion
- Most important factor affecting demand is temperature. With a coefficient of 0.73126, for every change in temperature of 1 degrees, demand increases by a factor of 0.73126 (temperature x 0.73126). Based on this, company will have to consider:
    - Necessary capacity building during hotter months to fulfill the demand:
        - Recall from our EDA section that hottest months lie in Fall season, June, July and Aug being the hottest.
    - If the company is able to scale up its resources to meet the increasing demand in these 3 months, it will also be wise to invest in increased marketing and promotional activities if more competitors operate in the same market with similar offering.
- Second most important factor is Light Rain or Snow with a coefficient of -0.27750. Hence, if a particular day has light rains, it is expected to reduce the demand by 27.7%.
    - Recall from our EDA section that frequency of light rains has been lowest and heavy rains have largely been non existant. October month shows the maximum number of instances of light rains.
        - Based on this, it is recommended to develop a sentiment based advertisement plan that heavily promotes "fun element" of "riding bikes in the rain with family".
- Third most important factor is year with a coefficient value of 0.24236. Based on the historical data, given all internal and external factors remain unchanged, the company is expected to see annual growth over last year at around 24%.
    - This helps us in factoring teh revenue and cost projections over a period of time.
- Fourth most important factor is winter with a coefficient of 0.12793. Tihs signifies that every winter, the demand is expecteed to incerase by a factor of 0.12793 basd on other months.
    - Recall from our EDA section, we recollect that Winter season constitutes of Sep. Oct, Nov and December months.
        - Company needs to work on capacity planing of these months and additionally plan for promotional campaigns in case a competitors exist with similar value propositions.
- Fifth most important variable is the month of July with a coefficient weightage of -0.10141 which signifies that every July the demand is expected to drop by a factor of 0.10141 (Around 10%)
    - Since month of July is also one of the hottest months, its relative weightage will simply decrease as compared to June and August. Hence, by logic, we can exclude month of July from our past recommendation.