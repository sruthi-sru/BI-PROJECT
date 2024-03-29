# BI-PROJECT Call Center Analysis for PWC

# Problem Statement

To create a Dashboard that reflects all relevant Key Performance Indicators (KPIs) and metrics in the call center dataset.

Possible KPIs to include:

* Overall customer satisfaction
* overall calls answered/abandoned
* Calls by time
* Average speed of answer
* Agents performance quadrant -> average handle time(talk duration) vs calls answered

# Data Visualization

Here Power BI tool is used for Data visualization and below figure depicts all the

kpi required for the basic analysis:






<img width="1210" alt="Screenshot 2023-07-27 at 5 22 54 PM" src="https://github.com/sruthi-sru/BI-PROJECT/assets/71058362/64ce335f-cc14-4f2f-b8e8-a6a1b84487d2">


# Calculations used

Average satisfaction rating = Average('Call Center'[Satisfaction rating])

Best performer 

<img width="558" alt="Screenshot 2021-08-21 at 2 00 23 PM" src="https://github.com/sruthi-sru/BI-PROJECT/assets/71058362/6c36ad1a-e2b4-41f7-894e-80452eca33b3">


Average speed of calls

<img width="361" alt="Screenshot 2021-08-21 at 1 59 37 PM" src="https://github.com/sruthi-sru/BI-PROJECT/assets/71058362/7bef68a7-4a26-4235-b179-9465b3de24c8">


Answered calls = Calculate(distinctcount('Call Center'[Call Id]),Filter('Call Center','Call Center'[Answered (Y/N)]="Y")) 

Problem resolved = Calculate(distinctcount('Call Center'[Call Id]),Filter('Call Center','Call Center'[Resolved]="Y"))
