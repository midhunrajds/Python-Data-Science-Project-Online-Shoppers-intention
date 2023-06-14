[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/NumPy-1.x-blue.svg)](https://numpy.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.x-blue.svg)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-blue.svg)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.x-blue.svg)](https://seaborn.pydata.org/)

# Python-Data-Science-Project-Online-Shoppers-intention

To determine if visiting sessions close to special days have an impact on finalized transactions, and also to identify patterns related to browsing period activity and pages visited.

## Basic Structure of the Project

## Project description 
- [Hypothesis](#hypothesis)
- [Methods](#methods)
- [Analysis](#analysis)
- [Results](#results)

## Outline of the Project
+ How pages visited by the visitor in a session and total time spent in each of these page categories affect purchase behaviours. I intend to use Clustering technique to identify patterns.
+ Determine whether the closeness of the site visiting time to a specific special day (e.g. Mother’s Day, Valentine's Day) result to be finalized with transaction using Classification technique.

## Justification of the Project
The project will help to gain knowledge on applying various techniques and tools learnt, to solve data science problems.
The outcome of the project will help to gain more insights into customer behaviour/ patterns.
On an organizational level, better placement of strategies to increase sales and optimize online experience for customers.

## Datasets
[Dataset Link](https://archive.ics.uci.edu/ml/machine-learning-databases/00468/)
This dataset is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.
This allows for the sharing and adaptation of the datasets for any purpose, provided that the appropriate credit is given.

## Desired Outcomes
To gain insights into customer behaviour patterns, and determine the affects of special days and weekends etc. on sales.

## Abstract
                  
## Introduction
### Column Descriptions:
+ Administrative: This is the number of pages of this type (administrative) that the user visited.
+ Administrative_Duration: This is the amount of time spent in this category of pages.
+ Informational: This is the number of pages of this type (informational) that the user visited.
+ Informational_Duration: This is the amount of time spent in this category of pages.
+ ProductRelated: This is the number of pages of this type (product related) that the user visited.
+ ProductRelated_Duration: This is the amount of time spent in this category of pages.
+ BounceRates: The percentage of visitors who enter the website through that page and exit without triggering any additional tasks.
+ ExitRates: The percentage of pageviews on the website that end at that specific page.
+ PageValues: The average value of the page averaged over the value of the target page and/or the completion of an eCommerce transaction.
+ SpecialDay: This value represents the closeness of the browsing date to special days or holidays (eg Mother's Day or Valentine's day) in which the transaction is more likely to be finalized. More information about how this value is calculated below.
+ Month: Contains the month the pageview occurred, in string form.
+ OperatingSystems: An integer value representing the operating system that the user was on when viewing the page.
+ Browser: An integer value representing the browser that the user was using to view the page.
+ Region: An integer value representing which region the user is located in.
+ TrafficType: An integer value representing what type of traffic the user is categorized into.
+ VisitorType: A string representing whether a visitor is New Visitor, Returning Visitor, or Other.
+ Weekend: A boolean representing whether the session is on a weekend.
+ Revenue: A boolean representing whether or not the user completed the purchase.
 
## The Problem (Context)
Only 15.5% of the visitors end up purchasing as per dataset collected over a period of one year.
What drives the purchase behavior and how can we increase the sales ?

## Purpose of the Study
Identify interesting correlations and patterns to understand customer intentions in a better way.
To gain insights into customer behavior patterns, and determine if there are any affects of special days and weekends etc. on sales.

## Project Description
Various data analytics techniques learnt during the course is applied to explore the data.
Followed the CRISP-DM process to ensure proper methodology.
Data Preparation: The data used in this analysis is an Online Shoppers Purchasing Intention data set provided on the UC Irvine’s Machine Learning Repository. This dataset has no missing values and all attributes are relevant to the analysis.

## Project Description: Hypothesis
Exploratory Data Analysis is done as there were no apriori notions before starting the project to be more familiar with the data.
Explored possibilities of certain category attributes such as region, visitor type, and special days, weekends affecting purchase behavior if any.
Some strong correlations were found between certain attributes.

## Project Description: Methods
- Exploratory Data Analysis.
- Clustering customers to segments using the data analytic techniques.
- [Full Code](Midhun_PRaj_Project_Python_Analysis.ipynb)

### Project Description: Analysis

<img width="782" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/2bd08e38-e4c6-42cf-8495-d53d0d4edae4">

+ Checked for null values.

![image](https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/1d674733-7771-4c58-929e-6c336da27db8)

+ Basic description to look at the mean, std, etc.

<img width="635" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/fc127406-ec12-477c-9955-da84fa1d9e1d">

+ Checked for total sessions ending up in purchase, represented as a pie chart here.

<img width="631" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/98cde7f3-066a-4f36-b7d2-146e345929c6">

+ Checked for correlations with ’Revenue’ attribute. There is an interesting correlation with ‘PageValues’ and attributes related to duration spent on website.(BounceRates, ExitRates, ProductRelated etc.)
 
+ Data Transformation/ Data Preparation.

<img width="604" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/40f70bcf-1b9a-4f4d-ac69-ddd1e2a75973">
 

## Observations:
### PageValues vs Revenue:

<img width="552" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/e13c8978-ba33-4603-bb9b-990779420ff8">

+ There are many outliers in positive outcome(True Revenue).
+ Pagevalue influenced purchases.
### Bounce Rates vs Revenue:

<img width="657" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/9f7cd0f9-c3df-43d0-a4ba-cda3057b0bb0">

+ So many outliers for False Revenue.
+ Bounce Rates also influenced whether to buy or not.

<img width="744" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/692792a6-690b-413b-a523-e43cae3b3fbb">

+ Trying to see how amount of time spent on the website relates to the bounce rates.

### Elbow method used to find out the optimal clusters in admin duration v bounce rates.

<img width="522" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/c7880269-2621-4c55-ae2c-f50dea6945b6">

+ According to the plot, number of clusters = 3.

<img width="557" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/dc8903ac-38a4-4514-82ac-85929cfc8125">

+ From the clustering plot, we can infer that more time customers spend in administrative duration in a website are less likely to bounce out from the website.
+ There are 3 groups:
  - Blue ones are a group of customers who stay for shortest administrative duration and have highest chance for navigating away.
  - Green ones are general group, they do not navigate away from the first visited page, but not necessarily ending up purchasing.
  - Orange ones are the target group who spends most time on the website and purchases.

<img width="820" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/56b81177-1f28-4425-acd8-b36c15b0171f">

There are more returning visitor visits than new visitors and also there is a very insignificantly low category “Other”. To compare website activity of the visitor types, total duration spent is calculated as Administrative +Informational + Product related.

<img width="504" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/79d55a7e-fab2-46c7-8a07-c67e190822bb">

+ As per boxenplot, returning visitors spend longer on the site.

<img width="651" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/ec8e6ff7-4d38-4ecb-a9b4-dc912df0ff84">


<img width="401" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/081be402-2396-4424-b97f-a0129f3b8c95">
<img width="477" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/bb5e11c6-cf20-47d2-bda4-62b4d787c5c6">

+ Majority of the visitors use operating systems and browsers with codes 1. and 2.

 <img width="605" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/14f52cac-8fa0-4f01-bd4c-0ca151ad6470">
 
 Major chunk of the visitors are from regions 1. and 3.

<img width="683" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/a8de8ec9-acb0-47d2-be31-14ddd88a0fb6">
 
 As ‘Special Day’ approaches, the values must increase in range (0 to 1). As per dataset, only months February and May have days "close to special days" which is certainly wrong. Hence this attribute is not useful as is. May be ‘SpecialDay’ is coded by the business owner as per some other criteria which we do not know as of now.

<img width="531" alt="image" src="https://github.com/midhunrajds/Python-Data-Science-Project-Online-Shoppers-intention/assets/126799337/11cf63be-4768-494a-9eee-e3cc8570e4fc">

 No important correlations observed for weekend attribute. No significant impact on customer intention.

## Project Description: Results
No significant activity was observed near special days. Suggest to provide offers close to the special day to increase revenue.
Region – Visitors are concentrated only on two regions, we can try to reach other bases.
There is no significant impact of weekend on customer intentions. So there is a need to push for more activity and sales during weekends.
Need to concentrate on target audience and also look for new visitors as the majority of sessions were returning visitors.

## Conclusion
Clustering shows that with more time spent on the website, there is more chance of purchase.
However, there are more returning visitors, meaning not many new visitors. As per all the analysis done, we can conclude that the revenue conversion is low (15.5%) with the current strategy, and we need to find ways to penetrate new customer bases, concentrating on aggressive sales and marketing aimed at special days and weekends.

### Bibliography
+ https://archive.ics.uci.edu/ml/machine-learning- databases/00468/
+ https://seaborn.pydata.org/tutorial.html https://matplotlib.org/stable/tutorials/index 
    
