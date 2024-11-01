# -Analysis-of-Property-Rental-Prices-and-Number-of-Reviews-in-the-NYC-in-2023

**To: Bruce Wayne, Managing Partner, Janzen Consulting Group**

**From: Aikokul Abdivalieva & Lincoln Chanakira, Analysts, Janzen Consulting Group** 

**Date: October 8, 2024** 

**Subject: Analysis of Property Rental Prices and Number of Reviews in the NYC in 2023** 

*The Number of Reviews is Not the Key to Pricing Insights*

This memo presents an analysis of the relationship between property prices and the number of reviews in the New York City rental market. Understanding how the volume of reviews correlates with rental prices is critical for identifying market trends and factors influencing renters’ and owners’ decisions. Using Ordinary Least Squares (OLS) regression with the significance level of 0.05, this analysis aims to uncover insights for both renters and property owners and managers. The **Null Hypothesis (H₀)** states that there is no relationship between the number of reviews and the price of rental properties. Meanwhile, the **Alternative Hypothesis (H₁)** states that there is a relationship between the number of reviews and the price. The **independent variable (IV)** is the “Number of Reviews,” representing the total number of reviews for each property listed. The **dependent variable (DV)** is the “Price,” reflecting the listing price.

<img width="994" alt="Screenshot 2024-11-01 at 14 04 20" src="https://github.com/user-attachments/assets/59373d16-c9a3-4d14-814c-0a0a587c6d91">

<br>
● No missing values; 50 outliers were kept unchanged to reflect the real rental market prices.

● The distribution of prices is almost symmetric, i.e. the data is evenly distributed.

● The variation of prices in NYC rentals in 2023 is moderate to high.

<br>
<img width="1016" alt="Screenshot 2024-11-01 at 14 06 42" src="https://github.com/user-attachments/assets/a9092c07-a83a-452f-87d2-ddff715c82c1">

<br>
● 183 missing values were removed from the dataset to work with only known values.

● 1024 outliers were kept unchanged in order to reflect the natural variability in the number of reviews, although there is a risk of incorrect conclusions.

● A right-skewed distribution indicates that while most properties receive fewer reviews with some having none, somproperties have a significantly higher number of reviews.

● The large standard deviation indicates a wide variation in the number of reviews among rentals. 

<img width="549" alt="Screenshot 2024-11-01 at 14 32 40" src="https://github.com/user-attachments/assets/ea366e49-8056-4181-a3f3-dc5c13394839">


**Assumptions:**

The analysis indicates that there is no strong evidence of violating any of the assumptions. However, there are influential outliers that are located beyond the Cook’s distance. These units may affect the result and it is recommended to compare regression analysis with another dataset after removing them.

**Regression Model:** Price = 624.4 + (0.03 * Number of Reviews)+ ε 

The F-statistic is 2.8, with a (p < 0.1), indicating that the model is statistically insignificant at the 0.05 alpha level. The IV (Number of Reviews) has a coefficient of 0.03 with a p-value < 0.1. This means that there is no evidence to suggest that the number of reviews is related to price. Hence, we failed to reject the Null Hypothesis. With the statistical insignificance and very low R²(0), generalizing these findings to the target population is risky, as the model explains none of the variance in price. 

Holding all else constant, for every additional review a property receives, its price increases by 0.03 USD. However, this is a very small increase, which may not have a very meaningful impact on the price of a rented place. F² = 0, the power of the regression analysis is very low, i.e. the model is unlikely to detect a meaningful effect, if there is one. 
<img width="494" alt="Screenshot 2024-11-01 at 14 34 24" src="https://github.com/user-attachments/assets/a92cde3f-ec8c-43f4-9bf7-d49a5c0b7fc1">

**Potential weaknesses and gaps:** The model explains almost none of the variance in price, indicating that the number of reviews is not a meaningful predictor. Using only the number of reviews and keeping the impactful outliers oversimplified the relationship. 

**Recommendations:** To improve the model, usage of additional variables such as property location, room type, and others are recommended. Also, multiple regression approaches with these predictors (e.g., location, property size) can yield more accurate and insightful results. 

**Conclusion:** The analysis reveals that the number of reviews had a statistically insignificant relationship with the rental price in NYC 2023. The model explains almost none of the variance in price, suggesting that reviews alone are not a meaningful predictor of rental pricing. This suggests that relying on the number of reviews alone as a pricing factor may lead to misguided decisions.

<img width="682" alt="Screenshot 2024-11-01 at 14 36 16" src="https://github.com/user-attachments/assets/add320f8-b3b5-4ba1-a127-c97f2c19b819">
<img width="696" alt="Screenshot 2024-11-01 at 14 36 07" src="https://github.com/user-attachments/assets/e3fa3e2f-7642-4738-be47-4c0891f3d17d">
<img width="730" alt="Screenshot 2024-11-01 at 14 35 56" src="https://github.com/user-attachments/assets/d926e9a1-bb08-4ef7-9152-8b598560164c">
<img width="796" alt="Screenshot 2024-11-01 at 14 35 42" src="https://github.com/user-attachments/assets/3357e8cc-16a8-4935-bdf0-719d05f25624">
