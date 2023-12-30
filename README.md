# Drug Risk Analysis


## **Introduction**

Drunk and impaired driving are devastating issues in the US, so I want to investigate how exactly different age groups have contributed to this problem. What age group has the highest rate of drug use? The highest rate of drug-positive crashes? Comparing these values will allow me to analyze the relationship between age, drug use, and drug-positive crash risk. The results of this project will inform on which population of people in the US are most prone to impaired car accidents.


## **Dataset Sources:**

Substance use in the US overtime in different age groups: https://think.cs.vt.edu/corgis/csv/drugs/ 

Crash risk of drug-positive drivers: https://www.nhtsa.gov/drug-and-alcohol-crash-risk-study/drug-and-alcohol-crash-risk-study-databases 


## **Visualizations**

<img width="918" alt="Screenshot 2023-12-30 at 5 33 39 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/4b8fd8f4-c2c2-422b-af70-24123ee93ca6">

<img width="695" alt="Screenshot 2023-12-30 at 5 34 12 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/6d4de972-f183-4648-8ccd-4cbea4bd8a3f">


Figure 1 shows that in 2018, 18-25 year olds had the highest rate of substance use of the three age groups, as predicted in my hypothesis. In order to determine if the substance use rate of 18-25 year olds in 2018 was significantly different from the use rates of the other two age groups, two bootstrap analyses were performed. The resulting sampling distributions are shown in Figures 2 and 3. These plots also show the 5% confidence interval cutoff values, as indicated by the red bars. The confidence interval for 12-17 year olds was 809-923 users (per 1,530,000 people) and that for 26+ year olds was 1115-1245 users (per 1,530,000 people). The rate of drug use for 18-25 year olds in 2018 was 2715 users (per 1,530,000 people). Since 2715 users is not in either of the sampling distributions’ confidence intervals, it can be concluded that the ratio of use for 18-25 year olds in 2018 was significantly higher than the ratios of use for the other age groups, thereby supporting my hypothesis.


<img width="485" alt="Screenshot 2023-12-30 at 5 34 27 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/a3c8f2cd-f4f0-404f-89a5-e1868c0b1820">


Figure 4 represents the quantity of drivers in 4 age groups who were drug-positive car crash drivers. It shows that the age group with the most crash drivers under the influence was 21-34 year olds, followed closely by 35-64 year olds. The 16-20 and 65+ age groups had the lowest count of impaired crash drivers. This result supports my hypothesis.


<img width="689" alt="Screenshot 2023-12-30 at 5 34 49 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/b93b453c-e5af-4bf3-87a8-31091a368821">


Figure 5 shows the number of people within each age group who were users of a certain drug over time. From 2010 to 2018, marijuana was by far the most used drug among 12-17 and 18-25 year olds. However, these groups differ in marijuana use in that the number of 12-17 year old users decreased over time and the number of 18-25 year old users increased over time. Alcohol and cocaine were significantly less used in these groups. In contrast, alcohol and marijuana uses in 26+ year olds were comparable. From 2010 to 2015, alcohol was most used by this group but from 2015 to 2018, marijuana was most used by this group. 


<img width="699" alt="Screenshot 2023-12-30 at 5 35 05 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/b3fcc9f6-0115-45f3-a7b8-cae106810b4c">


Figure 6 presents the frequencies that drugs were found in drug-positive car crash drivers. THC had by far the highest prevalence, followed by mixed doses, amphetamine, and alcohol. 


## **Analysis**

Figures 2 and 3 prove that the rate of drug use for 18-25 year olds was significantly higher than the rates of use for other age groups in 2018 and Figure 4 signifies that 21-34 year olds were most likely to be drug-positive car crash drivers. These results correlate with each other to show that young adults, specifically people in their early 20s, are most at risk for substance abuse and for being in a car accident while under the influence. This conclusion makes sense as exposure to drug use and time spent driving might increase when an individual moves away from home or enters the professional world for the first time.

Figure 5 demonstrates that the most used drug by 12-25 year olds between 2010 and 2018 was marijuana and that the number of marijuana users in the 18-25 age group had increased during this 8-year period. Marijuana also competed with alcohol as the most used drug by 26+ year olds. Figure 6 shows that THC was the most commonly found drug in crash drivers. These results combine to demonstrate that marijuana is both the most used drug by people in the US and most common drug found in impaired car crash drivers. The increasing use of marijuana in the US could potentially put more people in danger as crash-risk increases for these individuals.

This analysis is limited by a couple factors. For one, the drug use data is for the US only, so those results can't necessarily be generalized to age groups and their drug usages throughout the world. In fact, drug use rates are likely to vary with location as accessibility and acceptance of certain drugs will vary with geographical and cultural differences. A second limitation is that the drug use data used here only considered alcohol, cocaine, and marijuana usage. These are likely the most commonly used substances so they should allow for an accurate comparison, but it is important to note that these rates don't encompass all drugs.


### **View full project here:** https://github.com/catherinealeal/DrugRiskAnalysis/blob/6a5c23e8d89df88506f7e98104a42efa6bf03c71/DataScienceProject.ipynb
