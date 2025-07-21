# Business-Statistics-Report-ad-Hypothesis-testing-

## Objectives 

This project delivers a statistically‑grounded profile of the global Top 200 YouTubers, using data sourced from SocialBook’s real time influencer analytics platform. 

It has three linked objectives:

 - Describe the landscape: visualising how followers, likes, views, engagement rate and “boost index” are distributed across video categories and creator countries through bar charts, treemaps, packed‑bubble plots and histograms. 

- Test for significant differences in audience behaviour: applying a one‑way ANOVA to determine whether average 1‑day, 3‑day and 7‑day view counts differ across countries. 
- Model what drives popularity—running multiple linear regression to discover which engagement metrics most strongly predict subscriber counts, providing actionable insight for marketers and creators. 

By integrating descriptive and inferential statistics, the study aims to identify where influence is concentrated, how engagement patterns vary, and which factors best explain a channel’s follower base—insights that inform data‑driven influencer selection and content strategy.

## 📁 Contents

| Folder | Description | File |
|--------|-------------|------|
| `data/` | Raw survey data (.xlsx) | [Top 200 Youtubers.xlsx](https://github.com/folakeobalakun/Business-Statistics-Report-ad-Hypothesis-testing-/blob/main/Top_200_youtubers%20(1)%20-%20another%20cleaned%20copy.xls) |

<img width="452" height="199" alt="image" src="https://github.com/user-attachments/assets/4b4a97f3-d204-4cbe-b904-0a22227684da" />

The Standard deviation and variance are a measure of how far the data are from the mean. 
A small standard deviation indicates that the values in the data set are clustered around the mean, whereas a large standard deviation indicates that the values in the data set are far from the mean. In Table 1 above followers and likes have higher variance which means the values are more are not uniform i.e.; they are varied values.

<img width="452" height="250" alt="image" src="https://github.com/user-attachments/assets/129e5eca-7da6-4b00-889b-e7bfc5177248" />

The Main video category with the highest number of followers, The category with the highest number of followers is music with 2.12Billion followers and it is followed by Entertainment with 1.648Billion followers, the third main video category is Education with 0.48Billion (479Million). This shows that people would rather follow music and entertainment channels compared to Education channels.


<img width="452" height="226" alt="image" src="https://github.com/user-attachments/assets/5b8c1492-e537-4020-92ae-39222bba2d4f" />

Category Gaming and Apps has the highest boost index, the highest followers, high views and also highest class, so this is the same across the other categories whichever category is high in one would also be high in the other, and the category with low values is also low in the others. This could mean that there is a correlation between these variables

<img width="452" height="255" alt="image" src="https://github.com/user-attachments/assets/2dcf55bf-ae5e-4dde-9b4f-601e60b90b4b" />

The United States is leading with 52 categories consisting majorly of Gaming and Apps channels, India is second category with a total of 36 channel categories also consisting majorly of Gaming and Apps category. The third country is Brazil with a total of 8 categories

## Hypothesis Testing
One Way Anova


The Hypothesis is usually written as:
Null Hypothesis: H0: µ1 = µ2 = µ3 = ... µn (all n population means are equal)
Alternate Hypothesis, H1: At least one µ is different (at least one of the population means is different)
Using F value 
If F > F critical, then there isn’t enough evidence to support Null Hypothesis (Reject Null)
If F < F critical, then there is enough evidence to support the Null Hypothesis (Accept Null)
 Using P value 
If P - Value < 0.05 (alpha) then we reject the Null Hypothesis(H0)
If P – Value > 0.05 (alpha) then we accept the Null Hypothesis (H0)

For the Top 200 YouTube Influencer data, the proposed hypothesis for one-way Anova is 
H0 : µAvg. 1 Day  = µAvg. 3 Day = µAvg. 7 Day (Avg. 1 Day, Avg. 3 Day and Avg.3 Day have equal population mean in the Country variable)
H1 : At least one of the means is different 

 <img width="431" height="194" alt="image" src="https://github.com/user-attachments/assets/303366c1-1b52-4b10-aecf-992dd3c8bd0b" />
 

F value is 6.8668, F Critical is 3.0210
F Stat > F Critical, therefore we reject the H0 and accept H1
Using P value 
P – Value =0.0011
P value < 0.05 therefore we reject the H0 and accept H1

 with 95% confidence it can be said that the population mean is difference between Avg 1 day, Avg 2 day and Avg 3 day

## Linear Regression Analysis

For the Test based on the data, the dependent variable used is followers and the independent variable used are likes, views, boost index, comment avg and engagement rate 

Proposed Hypothesis 
H0 : There is no relationship between followers and other independent variables
H1 : There is a relationship between followers and at least one of the independent variables.

<img width="443" height="82" alt="image" src="https://github.com/user-attachments/assets/4016b99c-4841-4352-bab3-6bdce2d1da1d" />

R represents the correlation coefficient between dependent and independent variables, value is shown as 0.892. 
R2 indicates the proportion of variance in the dependent variable that the independent variables can collectively explain. The value shows 0.795
Adjusted R2 a modified and more accurate form of R2 shows the proportion of variation accounted for by only the independent variable, from our model summary It can be said that comments Avg, Boost Index, Engagement rate, views and likes account for 79% of variation in followers. 

<img width="453" height="152" alt="image" src="https://github.com/user-attachments/assets/520147df-d624-4e7c-9de1-06e4a7917288" />

Using the Anova table to test our hypothesis 
 P value is  <0.01 (sig), 0.01<0.05

Therefore, we reject the null hypothesis(H0) and accept the alternative hypothesis (H1) 

To conclude it can be said with 95% confidence that there is a relationship between followers and at least one of the independent variables.






