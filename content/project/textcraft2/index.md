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


## Dashboard Design and Implementation


### Home Tab

<div style="text-align:justify"><span>
The front end interface is also laid out in the three-stage fashion of the app's architecture for ease of interpretation. The first tab is the home page which comprises of the introduction to the tool and the instructions to use it.
</span></div>

<p align="center" style="font-family:Georgia;font-size:75%;">
  <img width="900" height="850" src="/project/textcraft2/pic1.png">
  <em>Home: Landing page of the app</em>
</p>

### Load Data Tab

<div style="text-align:justify"><span>
Under this tab, the user can upload a CSV file with the data or enter an API link which provides access to a json scipt of data. The json from API is automatically converted into a dataframe in R. The fetched data is previewed on the lower part of the screen. The user then chooses with field becomes the text corpus and which field would categorize the text as the response variable. Though, the user can select a single response field at a time, this field can be changed to redo the analysis. 

For reference, let's load a dataset containing the WebMD reviews for a set of selective serotonin reuptake inhibitors (SSRIs) antidepressants. The drug names are selected as the response and the reviews ("comment") are selected as the text corpus.

</span></div>

<p align="center" style="font-family:Georgia;font-size:75%;">
  <img width="900" height="850" src="/project/textcraft2/pic22.png">
  <em>Load Data: The user uploads a CSV file or enters API link</em>
</p>


### Process Data Tab

<div style="text-align:justify"><span>
This is the tab where text is analyzed and models are initiated. At the top of the screen, the user sees the top 10 words with their word counts, TF-IDF scores and the suggested words to remove. Suggested words to remove are defined by a collection of conditional statements, depending on the word frequency, their TF-IDF score and their correlation with the title of the responses. The annotation option allows the user to select the words to remove or enter a specific word. The user can revert the changes to the original form. 
</span></div>

<p align="center" style="font-family:Georgia;font-size:75%;">
  <img width="900" height="850" src="/project/textcraft2/pic33.png">
  <em>Process Data: Words selected and entered for annotation</em>
</p>

<p align="center" style="font-family:Georgia;font-size:75%;">
  <img width="900" height="850" src="/project/textcraft2/pic44.png">
  <em>Process Data: Selected words are removed from corpus</em>
</p>

<div style="text-align:justify"><span>
Once the redundant words are removed from the corpus, the app runs two main models - topic and sentiment analysis. For the topic analysis part, Latent Dirichlect Allocation (LDA) model is used in an unsupervised fashion to identify the most matching words for a particular topic. The top TF-IDF scores with respect to each response category is also obtained in the backend. The user is allowed to change the model configuration parameters like the seed value, number of topics, number of words per topic etc. The user also can perform the text tokenization in a unigram or bigram method, which basically refers to the number of words per token. For the chosen example, let's choose bigram modeling showing top 10 words and running LDA for 2 unsupervised topics. Clicking on 'Analyze Document Corpus' initiates the process.
</span></div>

<p align="center" style="font-family:Georgia;font-size:75%;">
  <img width="900" height="850" src="/project/textcraft2/pic88.png">
  <em>Process Data: LDA model configuration options</em>
</p>



{{%alert%}}
Click [TEXTCRAFT](https://neonflux56.shinyapps.io/TextCraft/) to access.
{{%/alert%}}


## References

- [http://www.tfidf.com/](http://www.tfidf.com/)

- [https://cran.r-project.org/web/packages/sentimentr/sentimentr.pdf](https://cran.r-project.org/web/packages/sentimentr/sentimentr.pdf) 

- [http://sentiment.nrc.ca/lexicons-for-research/](http://sentiment.nrc.ca/lexicons-for-research/) 

- [https://docs.rstudio.com/shinyapps.io/](https://docs.rstudio.com/shinyapps.io/) 

