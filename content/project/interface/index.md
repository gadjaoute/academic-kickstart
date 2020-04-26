---
date: "2017-04-01T00:00:00Z"
external_link: ""
image:
  caption:
  focal_point: Smart
links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/gadjaoute
#slides: Healthcare Insight and Inclusion Interface     
summary: Pilot project of a relational database and build an informative interface that incorporates historical prescription of Medicare transaction, psychotropic drug, corresponding diagnoses and patient’s reviews of psychotropic drugs.
tags:
- R
- Python
- Data Visualization
title: Healthcare Insight and Inclusion Interface

url_code: ""
url_pdf: https://github.com/gadjaoute/-Healthcare-Insight-and-Inclusion-Interface-
#url_slides: https://github.com/gadjaoute/-Healthcare-Insight-and-Inclusion-Interface-
url_video: ""
---

We constructed a relational database and build an informative interface that incorporates historical prescription of Medicare transaction, psychotropic drug, corresponding diagnoses and patient’s reviews of psychotropic drugs. 

We combined FDA drug label information, patient drug reviews, Medicare FFS parts b and d provider utilization and payment data sets, as well as hospital information and review. 

We gathered data using API and scraping methods (R, Python) to extract WebMD drug reviews from psychotropic drugs.

Then we applied sentiment analysis on drug reviews to gather insights. In this example below we chose to focus on three stimulants Adderall, Strattera and Vyvanse.

![](/project/interface/drug.PNG)


We used the interface to evaluate hypotheses (i.e., understand prescribing and practice trends both at the physician level and understand geographic trends). 

![](/project/interface/dashboard.PNG)

Potential use: Summarize from the connection between related information including geographic location, NPI (provider identifier), drug, diagnosis, cost, review for professionals to extrapolate business, epidemiology and medical insights ranging from nationwide to individual level.






{{%alert%}}
Click [DASHBOARD](https://github.com/gadjaoute/-Healthcare-Insight-and-Inclusion-Interface-) to view more details on this project.
{{%/alert%}}
