---
date: "2019-12-01T00:00:00Z"
external_link:
image:
  caption:
  focal_point: Smart
links:
- icon: twitter
  #icon_pack: fab
  #name: Follow
  #url: https://twitter.com/gadjaoute
#slides: MSSEDA
summary: User-Defined Real Time Text Mining Automation Tool 
tags:
- R
- Data Visualization
- Deep Learning
title: Textcraft

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---
## Executive Summary

TextCraft delivers a framework with user-friendly interface to analyze and visualise any text corpus making it a versatile asset for unstructured text analysis. TextCraft is unique in the way that it is scalable, robust and its ease-of-interpretation, thus making it seamless even for user having minimal background in dealing with text. It uses various natural language processing algorithms in the backend, which are easily configurable, producing accurately tailored results.The content is very visual and dynamic for any user to understand the effective topics and sentiments in a text corpus. One of the many possible use cases for this tool could be for business owners to potentially make business strategies and decisions based on customer review sentiment captured by this web application. Another applicable use for this tool is to innovate methodologies in healthcare research, such as to extract key insights from unstructured deidentified clinical notes or patient drug reviews.

## Introduction

This web application was envisioned as an asset for users with little or no background understanding of dealing with text data. This user friendly interface allows for a user to perform text analytics, mainly topic modeling and sentiment analysis, on any text data.

The app works in three stages:

![](/project/textcraft2/stages.PNG)

### 1. Load Stage

<div style="text-align:justify"><span>
The user uploads data in a csv file or hits Application Programming Interfaces(APIs) to pull data into the tool. The user views a preview of the collected data and decides the field that becomes the response and the field on which text models are applied.
</span></div>


### 2. Process Stage

<div style="text-align:justify"><span>
This is the stage where data cleaning and modelling occurs. The user views a glimpse of general summaries of the dataset such as the TF-IDF scores, frequency counts etc. The user can annotate the word collection accordingly. The tool also allows the user to adjust configuration parameters for running various models. 
</span></div>


### 3. Insights Stage

<div style="text-align:justify"><span>
This stage displays a set of tailored charts and visuals corresponding to the configured outputs for the user to make sense of the data. The plots are grouped by each response field categories making the analysis more granular and comprehensive.
</span></div>


![](/project/textcraft2/workflow.PNG)

{{%alert%}}
Click [TEXTCRAFT](https://neonflux56.shinyapps.io/TextCraft/) to access.
{{%/alert%}}


## References

- [http://www.tfidf.com/](http://www.tfidf.com/)

- [https://cran.r-project.org/web/packages/sentimentr/sentimentr.pdf](https://cran.r-project.org/web/packages/sentimentr/sentimentr.pdf) 

- [http://sentiment.nrc.ca/lexicons-for-research/](http://sentiment.nrc.ca/lexicons-for-research/) 

- [https://docs.rstudio.com/shinyapps.io/](https://docs.rstudio.com/shinyapps.io/) 

