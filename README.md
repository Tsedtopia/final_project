
# Scratching the surface of social cohesion
 
## Purpose: This data serves Economists, Government agencies and Non-governmental agencies both within the country and outside as a baseline for level of risk.  Without this kind of data governments may have a delayed response to the urgent needs of their nation. This is also a useful resource to organizations that provide intervention services both within their country and internationally. It’s especially important to predict potential volatility.
What makes a cohesive nation? 
How is social cohesion measured?  In my dataset there are 12 indicators identified in the Fragile State Index, and each of them have an assigned value for each of the 178 countries. The nations are ranked with #1 being the least cohesive least stable country, and 178 as the most stable most cohesive country. 
## 12 Indicators:
●	C1: Security Apparatus
●	C2: Factionalized Elites
●	C3: Group Grievance
●	E1: Economic Decline &Poverty
●	E2: Uneven Economic Development
●	E3: Human Flight & Brain Drain
●	P1: State Legitimacy
●	P2: Public Services
●	P3: Human Rights & Rule of Law
●	S1: Demographic Pressures
●	S2: Refugees & IDPs Internally Displaced Persons
●	X1: External Intervention

## The methodology used to construct the data was headed by Fund for Peace. Data analysts triangulated three different data streams to measure the 12 indicators using 1) primary data from the World Bank and UNHCR – United Nations High Commissions for Refugees, etc. 2) Content analysis of millions of online public documents using Boolean search strings to flag sharp changes from one country to the next, and 3) qualitative assessment. The approach taken is to scale and normalize the individual metrics and then integrate with weighted averages. 

![Methodology](/images/logo.png)

For the qualitative component, two separate teams of analysts independently conduct a qualitative analysis to assess, based on major events, whether the country indicator scores got better, worse, or stayed the same.  The qualitative analysis is done twice, by two different sets of analysts with a firewall between them, to reduce bias and fill gaps.
Finally the three data streams are compared to see if they generate the same outcome, and triangulated to arrive at a reconciled score.
The methodology was pretty consistent for each year, beginning with 147 countries in 2006 and expanding to a total of 178 countries on their current list.

## My testing method: Supervised ML, Regression & Linear Regression. 
Keras sequential, nn-model, deep-model, and linear regression
●	Results for target metric Fractionalized Elites
○	Nn model: R² value for y_train = .76 and y_test = .66
○	Deep model: R² value for y_train = .80 and y_test .70
●	The results were slightly varied due to the nature of the algorithm but the accuracy scores are around 82% across different indicators. 
P-value – testing the null hypothesis
 
![p-value_outcome_sample](/images/logo.png) 
Libaries: Pandas, Numpy, Tensorflow, Sklearn (preprocessing, model_slection, metrics, linear model, and matplotlib.

Import Tableau Animation - 
![https://public.tableau.com/profile/tsedey.aragie#!/vizhome/DataViz_fragilestateindex/C-indicators?publish=yes
](/images/logo.png)

Challenges and Difficulties Encountered: The data was pretty clean but interpreting and finding the most influential and most correlated indicators took a little maneuvering. The Indicators that were most correlated were C3: Grievances, X1: External Intervention, C2: Factionalized Elites, S2: Refugees and IDPs, and P1: State Legitimacy. It would be interesting to compare a test and train sample for public documents in the languages of the countries being analyzed. 

