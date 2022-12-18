# Survival-Analysis-Project

## I. Introduction

For burn patients, infection control remains an essential component of their treatment as the burn wound can be highly susceptible to colonization by
micro-organisms, which could lead to extended hospital stays or deaths in severe cases. In attempting to better control burn wound infection, a new 
antimicrobial detergent with 4 percent chlorhexidine gluconate was proposed as a substitute for the conventional method, a combination use of a 10 
percent povidone-iodine (Betadine*) and total body bathing with bar soap. In this report, a statistical analysis based on Cox Proportional Hazard Model
is conducted to investigate the effectiveness of the new method in terms of reducing the risk of wound infection. The data being used in the analysis 
is based on two previous cohort studies: in one study, patients were treated with the use of the new antimicrobial detergent; in another study, which was
conducted earlier, patients were treated with the conventional method. A comparison based on the two sets of data will then be conducted. More detailed 
information can be found in the publication “Evaluation of Protocol Change in Burn-Care Management Using the Cox-Proportional Hazards Model With Time-
Dependent Covariates” (Ichida, J. M et al., 1993). In our context, we will use the outcome of straphylocous aureaus infection as our response metric to
determine if infection took place. A group of variables that provide information about race, gender, burn site, burn type, percentage of burned area, as
well as time dependent variables for prophylactic antibiotic treatment and surgical excision of burned tissue, will be used as explanatory measures.


## II. Dataset

The dataset consists of 154 observations and 18 columns, including 1 index variable, 4 numerical variables and 13 categorical variables. The index
variable simply denotes the patient ID. Among the 4 numerical columns, 3 are time-to-event variables corresponding to the events of prophylactic 
antibiotic treatment, straphylocous aureaus infection and surgical excision; the other measures the percent of burned area. The 13 categorical variables
provide relevant information about burn sites, burn types (chemical, scald, flame or electric), race (white or non-white), gender (male or female), 
treatment (routine or cleansing with detergent) and also whether or not prophylactic antibiotic treatment, straphylocous aureaus infection and surgical 
excision took place.

## ..

## V. Conclusion

After examining the relationship between the straphylocous infection and various other variables, the conclusions are as follows:

+ At significance level 0.05, the infection survival for treatment group is significantly different from control group; total body cleansing with the 
detergent tended to have better survival than those who received routine care (50% to 60% less likely to be infected on average).

+ There is some weak quadratic relationship between percent of burned area and infection time: with low percent of burned area, higher percentage is 
associated with longer time to infection; with high percent of burned area, higher percentage tend to coincide with less time to infection. Such 
relationship remains dubious.

+ Percent of burned area, the only indicator of burn severity in our dataset, is not significant in Cox hazard model. It may be useful to consider other
possible metrics that describe burn severity (e.g. burn degree) in further investigation.

+ Based on five number summary (min, 25th, median, 75th, max), patients who were infected tend to have higher percent of burned area. Nevertheless, percent
of burned area is not a significant factor in the hazard model.

+ Patients with different gender do not diff significantly in infection survival.

+ Patients who are non-white have significantly different survival function from white patients; non-white patients tend to have higher survival rate overall,
based on our data. Some further clinical investigation may be needed to confirm if non-white patients are less likely to be infected than white patients.








