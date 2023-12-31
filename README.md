# Analyzing Drug-Positive Crash Risk of Different Age Groups in the US

-------

## **Introduction**

Drunk and impaired driving are devastating issues in the US. This project investigates how exactly different age groups have contributed to this problem. What age group has the highest rate of drug use? The highest rate of drug-positive crashes? Comparing these values will allow me to analyze the relationship between age, drug use, and drug-positive crash risk. The results of this project will inform on which population of people in the US are most prone to impaired car accidents.

-------

## **Data Collection:**

[Substance use in the US overtime in different age groups](https://think.cs.vt.edu/corgis/csv/drugs/)

[Crash risk of drug-positive drivers](https://www.nhtsa.gov/drug-and-alcohol-crash-risk-study/drug-and-alcohol-crash-risk-study-databases)

-------

## **Visualizations**

### **Hypothesis 1:** 18-25 year olds had the highest rate of substance use in 2018.

<img width="541" alt="Screenshot 2023-12-31 at 3 01 24 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/10905fbc-e40e-4d5b-ae96-5b391dbab223">

**FIGURE 1.** The above plot compares the number of substance users in 2018 in each age group per about 1.5 million people. An example interpretation would be that for about every 1.5 million 12-17 year olds in the US in 2018, about 900 of them were drug users in 2018.

Figure 1 shows that in 2018, 18-25 year olds had the highest rate of substance use of the three age groups, as predicted in my hypothesis.


### **Hypothesis 2:** The ratio of use for 18-25 year olds in 2018 was significantly higher than the ratios of use for the other age groups.

<img width="456" alt="Screenshot 2023-12-31 at 3 04 03 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/dcf84bc8-90b5-4848-b6ae-e44c0a85fcab">

**FIGURES 2-3.** The above 2 plots are the sampling distributions created for two age groups by bootstrapping their drug use proportion data from 2018. The age group represented by each plot is specified in the plot title.

In order to determine if the substance use rate of 18-25 year olds in 2018 was significantly different from the use rates of the other two age groups, two bootstrap analyses were performed. The resulting sampling distributions are shown in Figures 2 and 3. These plots also show the 5% confidence interval cutoff values, as indicated by the red bars. The confidence interval for 12-17 year olds was 809-923 users (per 1,530,000 people) and that for 26+ year olds was 1115-1245 users (per 1,530,000 people). The rate of drug use for 18-25 year olds in 2018 was 2715 users (per 1,530,000 people). Since 2715 users is not in either of the sampling distributions’ confidence intervals, it can be concluded that the ratio of use for 18-25 year olds in 2018 was significantly higher than the ratios of use for the other age groups, thereby supporting my hypothesis.


### **Hypothesis 3:** 21-34 year olds had the highest frequency of drug-positive crash drivers.

<img width="419" alt="Screenshot 2023-12-31 at 3 06 21 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/04e23224-c33a-4606-9c22-94fdd5375b23">

**FIGURE 4.** The number of drug-positive crash drivers in 4 age groups.

Figure 4 represents the quantity of drivers in 4 age groups who were drug-positive car crash drivers. It shows that the age group with the most crash drivers under the influence was 21-34 year olds, followed closely by 35-64 year olds. The 16-20 and 65+ age groups had the lowest count of impaired crash drivers. This result supports my hypothesis.


### **Hypothesis 4:** Alcohol had the highest usage in every age group.

<img width="481" alt="Screenshot 2023-12-31 at 3 07 59 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/849dbac0-6976-4bfe-b904-e1a4498b053c">

**FIGURE 5.** The above three subplots show the number of people within an age group between 2010 and 2018 who were users of a certain drug. Each line represents a different drug, as specified in the legends.

Figure 5 shows the number of people within each age group who were users of a certain drug over time. From 2010 to 2018, marijuana was by far the most used drug among 12-17 and 18-25 year olds. However, these groups differ in marijuana use in that the number of 12-17 year old users decreased over time and the number of 18-25 year old users increased over time. Alcohol and cocaine were significantly less used in these groups. In contrast, alcohol and marijuana uses in 26+ year olds were comparable. From 2010 to 2015, alcohol was most used by this group but from 2015 to 2018, marijuana was most used by this group. 


### **Hypothesis 5:** Alcohol was the most frequently found drug in drug-positive crash drivers.

<img width="620" alt="Screenshot 2023-12-31 at 3 09 19 PM" src="https://github.com/catherinealeal/DrugRiskAnalysis/assets/100166102/b4a1b4f4-ffc8-4bab-a7e4-409f7be36aa4">

**FIGURE 6.** The above plot shows the frequency that different drugs were found in drug-positive crash drivers.

Figure 6 presents the frequencies that drugs were found in drug-positive car crash drivers. THC had by far the highest prevalence, followed by mixed doses, amphetamine, and alcohol. 

-------

## **Analysis**

Figures 2 and 3 prove that the rate of drug use for 18-25 year olds was significantly higher than the rates of use for other age groups in 2018 and Figure 4 signifies that 21-34 year olds were most likely to be drug-positive car crash drivers. These results correlate with each other to show that young adults, specifically people in their early 20s, are most at risk for substance abuse and for being in a car accident while under the influence. This conclusion makes sense as exposure to drug use and time spent driving might increase when an individual moves away from home or enters the professional world for the first time.

Figure 5 demonstrates that the most used drug by 12-25 year olds between 2010 and 2018 was marijuana and that the number of marijuana users in the 18-25 age group had increased during this 8-year period. Marijuana also competed with alcohol as the most used drug by 26+ year olds. Figure 6 shows that THC was the most commonly found drug in crash drivers. These results combine to demonstrate that marijuana is both the most used drug by people in the US and most common drug found in impaired car crash drivers. The increasing use of marijuana in the US could potentially put more people in danger as crash-risk increases for these individuals.

This analysis is limited by a couple factors. For one, the drug use data is for the US only, so those results can't necessarily be generalized to age groups and their drug usages throughout the world. In fact, drug use rates are likely to vary with location as accessibility and acceptance of certain drugs will vary with geographical and cultural differences. A second limitation is that the drug use data used here only considered alcohol, cocaine, and marijuana usage. These are likely the most commonly used substances so they should allow for an accurate comparison, but it is important to note that these rates don't encompass all drugs.


### View full project notebook here: 
https://github.com/catherinealeal/DrugRiskAnalysis/blob/6a5c23e8d89df88506f7e98104a42efa6bf03c71/DataScienceProject.ipynb
