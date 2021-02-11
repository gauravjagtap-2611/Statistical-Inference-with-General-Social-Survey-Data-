# Statistical-Inference-with-General-Social-Survey-Data-
# 1. Introduction
The General Social Survey (GSS) is an observational study conducted by the National Opinion Research Center, at the University of Chicago.Our analysis will focus on the GSS 2012 report; hence, this data is generalizable to adults, aged 18 years and above, living in households in the United States, who are able to do the survey in English or Spanish.

# 2. Research question 1 :
## Is there any relation between political party affiliation and race to which people belong?
 
Visualizing different race affiliation to political parties in US.
![image](https://user-images.githubusercontent.com/78009164/107667228-62f47380-6cb5-11eb-80c9-b65adb693897.png)

## Interpretation:
If we consider different races and their political affiliation, *white* race has somewhat equal proportion of political affiliation ,but at the same time it has maximum and of all races greatest no of *Strong Republican* affiliation.\
Similarly, Black population seem to  have *Strong Democrat* affiliation and least *Strong Republican* affiliation.This is exactly opposite to *White* population.
Others have roughly equal political party affiliation.

## 2.3 Inference:

## 2.3.1 Stating Hypothesis:
<div class="alert alert-block alert-info">
**Null hypothesis:** Race and Partyid are independent of each other. \

**Alternative hypothesis:** Race and Partyid are dependent.
</div>
## Chi-sq Results:

>Pearson's Chi-squared test

>> data:  new_df$partyid and new_df$race
>>X-squared = 5670.8, df = 14, p-value < 2.2e-16

## Conclusion 2.3.4:

We have enough evidence to say that there is association between race of population and party affiliation.


#  Research question 2:
## Is there income disparity among different races in US society?

## 3.1 Motivation

The reason why this question is interesting is that this research surveys across a broad range of US demographics, including all races. Studying the differences between average family income across races may reveal helpful insights about the income gap in the US.

Now we will try to visualise this income distribution among different races using violine plot.

![image](https://user-images.githubusercontent.com/78009164/107667287-73a4e980-6cb5-11eb-91c2-9e0e47fc84dc.png)

## Interpretation:
Here we can see that, White & Other races have similar kind of income distributions. And greater proportion of the people belonging to Black race have fairly low income. As interpretation of graphs/plots is subjective, we try to confirm this hypothesis using Statistical tests.


## 3.3 Inference:

## 3.3.1 Stating Hypothesis:

<div class="alert alert-block alert-info">
μ = average family income (in US dollars)

**Null hypothesis:** The average family income is the same across all races(i.e μ1 = μ2 = μ3).

**Alternative hypothesis:** The average family income differs between at least one pair of races.

</div>


## Conclusion:
 WE carry out One Way ANOVA to come this conclusion, for detailed analysis resfer to attached R pdf file.\
 \
The data provide convincing evidence that at least one pair of population means are different from each other. There is a difference between the average family income (is US dollars) between at least one pair of race.
