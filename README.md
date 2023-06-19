# PowerBI Capstone Project

### Data Science Salaries 2023 (Predictive Data Analytics)

![Screenshot of Main Report][([Imgur](https://i.imgur.com/a0lg6K1.png)

[Screenshot of Country report](https://i.imgur.com/qPAgxy5.png)

**Contents/Agenda**

* Introduction

  * Role

  * Business Problem Overview

  * Solution Approach

* Data Overview

* Data Analytics Results

* Executive Summary 

  * Actionable Insights

  * Recommendations

**Role**

* Data Analyst for a higher education learning institute

* Reporting to Head of Sales and Marketing

**Business Challenge Overview**

With globalisation and technological advancement, market competition for higher education is intense. The Sales and Marketing department needs to gain insights on salaries of different Data Science fields in the Data Science domain, as shown in the dataset, to better strategise their marketing plan.

Data Science Salaries 2023 💸 | Kaggle

https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023

**Solution Approach**

* Extract, Transform, Load 

* Share insights and recommendations

**Data Overview**

1.  work_year         : The year the salary was paid.
                        (2023, 2022, 2021, 2020)

2.  experience_level  : The experience level in the job during the year
                        (EN: Entry, MI: Middle, SE: Senior, Ex)

3.  employment_type   : The type of employment for the role
                        (FT: Full time, PT: Part time, CT: Contract, FL: Flexi)

4.  job_title         : The role worked in during the year.

5.  salary            : The total gross salary amount paid.

6.  salary_currency   : The currency of the salary paid as an ISO 4217 currency code.

7.  salaryinusd       : The salary in USD

8.  employee_residence: Employee's primary country of residence in during the work year as an ISO 3166 country code.

9.  remote_ratio      : The overall amount of work done remotely

10. company_location  : The country of the employer's main office or contracting branch

11. company_size      : The median number of people that worked for the company during the year
                        (S: Small, M: Medium, L: Large)

**Data Reprocessing**

There is no blank value.

Removal of 

* “salary”, as it bears no significant in analysis, since total gross salary in various currency would not be good for comparison against each other. “salaryinusd” would be more comparable. 

* “salary_currency”, since “salaryinusd” is used directly for comparison, and “salary” is disregarded. 

* “employee_residence”, since most of the records of “employee_residence” is the same as “company_location” and for the efficiency of analysing. 

Addition of

* Serial_number for unique identification

**Executive Summary**

Actionable Insights 

* Salary => Minimum: US$5132   Average: US$137570   Max: US$450000
* For Experience_level, Ex has the highest average salary, which may be the reason for them no longer in service, eg retrench due to being high cost. Followed by Senior, Middle then Entry, which is very logical. 
    Ex: US$194930.93   Senior: US$153051.07   Middle: US$104525.94   Entry: US$78546.28
    
* For Company_size, surprisingly, Medium-sized company has highest average salary, followed by Large-sized company, then Small-sized company. It may be due to Large-sized company generally tend to attract wider pool of talents and may have better welfare, thus Medium-sized company needs to provide better salary to gain competitive edge.
    Medium-sized: US$143130.55 (42.14%)   Large-sized: US$118300.98 (34.83%)   Small-sized: US$78226.68 (23.03%)
  
* There is an upward trend in salary from year 2020 to 2023, especially super steep upward trend for 2021-2022, which matches the duration of COVID pandemic. During COVID pandemic, employees are required to work from home, and this brings about the mark demand in advance technology.
  
* For Employment_type, as expected, Full Time has the highest pay, followed by Contract, Flexi then Part Time. This is very logical, as Flexi and Part Time naturally has shorter working hours than Full Time or Contract, thus salaries are also lower. 
     FT: 138314.20 (40.31%)   CT: 113446.90 (33.07%)   FL: 51807.80 (15.1%)   PT: 39533.71 (11.52%)
  
* US has the highest number of people working in Data Science by this dataset, followed by Spain, France, India. Out of 3755, 3040 company_location are US. It may be due to US being one of the largest country and having a very big population as compared to many other countries.
  
* Israel has the highest average salary for working in Data Science by this dataset, but there are only two records of salaries. The high salary may be due to the country being war prone. 

Recommendations

* Sales and marketing can focus mainly on US market, since there is a high percentage of Data Science work there. But further data needs to be collected to understand if this market is saturated and which countries have high demand for people to work in Data Science, so that more precise details can be shared to attract potential students.
  
* Maximum and Average salaries (especially for average salaries for Medium-sized companies) can be shared during Sales and Marketing to gain interest from potential students.
  
* Further data can be collected over next few years eg 3 – 5 years, to facilitate deeper understanding of salaries, post COVID pandemic, which World Health Organisation has just announced on 4 May 2023 that COVID-19 is no longer global health emergency. This will help better analysis for future long term planning.
  
* Further analysis can be conducted by studying the salaries of Data Science by remote work, non-remote work and hybrid, for even more detailed analysis.
  
* Further analysis can be conducted to gain insights into whether Employee_residence different from Company_location can have effect on salaries eg higher salary to compensate for the moving from a country to another. 
