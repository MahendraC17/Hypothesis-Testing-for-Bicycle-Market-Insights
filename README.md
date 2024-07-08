# Hypothesis Testing for Market Insights

Hypothesis Testing on the Bicycle Sales to gain information on factuals and counterfactuals deriving the Bicycle Sales.
Kaggle's dataset was used for this project. Original dataset's link from Kaggle cannot be found as it was not save but the dataset can be found in the repo.

Hypothesis Testing helps in finding relationships, dependency on various groups and correlation.
HO - _Null Hypothesis_ which is a ground truth and we try to reject it.
H1/HA - _Alternate Hypothesis_ is opposite of the Null Hypothesis, when we reject HO, we accept H1 or otherwise.
DIfferent features encode variety of groups which can help in insightful knowledge which can help in targeted marketing to gain profit in the market. In context to the _Bicycle Sales_ Dataset, I try to gain which features group is more responsible of buying or not buying.


## 1. Categorising Features

Following features were categorised based on their respective nature.

Categorical Features: 
`Marital_Status`: 'Married', 'Single'

`Gender`: 'Female', 'Male'

`Education`: 'Bachelors', 'Partial College', 'High School', 'Partial High School', 'Graduate Degree'

`Occupation`: 'Skilled Manual', 'Clerical', 'Professional', 'Manual', 'Management'

`Home_Owner`: 'Yes', 'No'

`Commute_Distance`:  0.5,  2.5,  7.5, 10.0

`Region`: 'Europe', 'Pacific', 'North America'

Numerical Features:
`Income`

`Children`
`Age`


Target feature:
`Purchased_Bike`: 1, 0

## 2. Graphical Distribution:

-- A Histogram was plotted for categorical features to see the categories distribution.
-- A QQ plot was plotted for the numerical features to verify the normality of the features.
-- Further confirming the QQ plot with a density plot of the numerical features.
-- Having `Normal` with `Continuous` and `Discrete` features changes the Hypothesis Test which needs to applied on them.

## 3. Hypothesis Test findings:

-- alpha = 0.05 (Significance Level)

1. Income and Bike Purchase
Null Hypothesis (H0): There is no significant difference in mean income between those who purchased a bike and those who didn't.
Alternative Hypothesis (HA): There is a significant difference in mean income between those who purchased a bike and those who didn't.

Mean Income (Purchased Bike): 57505.20
Mean Income (Did Not Purchase Bike): 54874.76
Standard Deviation of Income: 31066.07
The Z-test was applied for hypothesis testing, and the results showed:

Z-statistic: 1.34
P-value: 0.1810
Conclusion: Failed to reject the Null Hypothesis: There is no significant difference in mean income between those who purchased a bike and those who didn't.

2. Age and Bike Purchase
Null Hypothesis (H0): There is no significant difference in mean age between those who purchased a bike and those who didn't.
Alternative Hypothesis (HA): There is a significant difference in mean age between those who purchased a bike and those who didn't.

Mean Age (Purchased Bike): 42.94
Mean Age (Did Not Purchase Bike): 45.35
Standard Deviation of Age: 11.35
The Z-test was applied for hypothesis testing, and the results showed:

Z-statistic: -3.35
P-value: 0.0008
Conclusion: Reject the Null Hypothesis. There is a significant difference in mean age between those who purchased a bike and those who didn't.

3. Children and Bike Purchase
Null Hypothesis (H0): There is no significant difference in the proportion of individuals with 0 children who purchased a bike compared to those with 1-5 children who purchased a bike.
Alternative Hypothesis (HA): There is a significant difference in the proportion of individuals with 0 children who purchased a bike compared to those with 1-5 children who purchased a bike.

Chi-square statistic: 32.28
P-value: 0.0000
Conclusion: Reject the Null Hypothesis. There is a significant difference in the proportion of individuals with 0 children who purchased a bike compared to those with 1-5 children who purchased a bike.

4. Gender and Bike Purchase
Chi-square statistic: 0.09
P-value: 0.7681

Conclusion: Failed to reject the Null Hypothesis. There is no significant difference in the proportion of individuals who purchased a bike based on gender.

5. Marital Status and Bike Purchase
Chi-square statistic: 11.54
P-value: 0.0007

Conclusion: Reject the Null Hypothesis. There is an association between Marital Status and bike purchase.

6. Education and Bike Purchase
Chi-square statistic: 25.33
P-value: 0.0000

Conclusion: Reject the Null Hypothesis. There is an association between Education and bike purchase.

7. Occupation and Bike Purchase
Chi-square statistic: 8.01
P-value: 0.0914

Conclusion: Failed to reject the Null Hypothesis. There is no significant difference in the proportion of individuals who purchased a bike based on Occupation.

8. Home Ownership and Bike Purchase
Chi-square statistic: 0.29
P-value: 0.5872

Conclusion: Failed to reject the Null Hypothesis. There is no significant difference in the proportion of individuals who purchased a bike based on Home Ownership.

9. Region and Bike Purchase
Chi-square statistic: 13.75
P-value: 0.0010

Conclusion: Reject the Null Hypothesis. There is an association between Region and bike purchase.

10. Cars and Bike Purchase
Chi-square statistic: 52.94
P-value: 0.0000

Conclusion: Reject the Null Hypothesis. There is an association between the number of Cars and bike purchase.

11. Commute Distance and Bike Purchase
Chi-square statistic: 28.84
P-value: 0.0000

Conclusion: Reject the Null Hypothesis. There is an association between Commute Distance and bike purchase.

12. Income and Region
Null Hypothesis (H0): There is no significant difference in mean income among different regions.
Alternative Hypothesis (HA): There is a significant difference in mean income among different regions.

F-statistic: 62.87
P-value: 0.0000
Conclusion: Reject the Null Hypothesis. There is a significant difference in mean income among different regions.
