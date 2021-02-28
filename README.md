# Cluster Analysis of Web User Sessions

You can view the output [here]( https://nehalmuthu.github.io/Cluster-Analysis-for-Web-Users-Sessions/ )!

## Overview:
- Targeted Advertisement, product/offer campaigns, providing discounts to lure in customer, etc are some of the major application areas of e-commerce.
- All the above mentioned application requires segmentation of customers so as to ease the marketing of products.
- While there are traditionally many ways to group users/customers based on their personal characteristics, this projects aims to categorize them based on their navigational patterns (i.e. pattern in webpages visited by a user) observed from their user sessions. 
- Based on the page visits of a user we categorize the users.
- We do a group wise analysis of page hits which can be used to understand the needs of each segment.
- Additionally we build a user network based on sessions and do community detection to identify similar users for targeted advertisements. 
- Also a web-page network is built in order identify important pages in a website. Based on the transition probability matrix formed we find the probability of page transitions.
- Finally, we have build a network plot for user and colored each node based on i) age category ii) location, so as to check for the characteristics of a group.

I personally spent a lot of time understanding and interpreting the dataset. So I will boil it down for you guys.

## Dataset:
- I have provided the dataset in the data folder.
- To learn more about the dataset go to (https://archive.ics.uci.edu/ml/datasets/msnbc.com+anonymous+web+data)
- Go to the above mentioned link and under data folder you will find msnbc990928.seq.gz.
- Download and extract. You will get .seq file, you can view it using notepad++.
- It is not much different from .txt, so you can read it normally using “fopen” in python(for reference check the code folder).

## Understanding the Dataset:
- Each line in the dataset represents a user session. 
- Assume each line to be a user.
- Each line is something like this :  2 12 3 4 12 12
- Meaning user has visited page 2 then 12 followed by 3, 4 and again 12.
- The website MSNBC is an American news-based pay television cable channel.
- It contains different pages like sports, medical, economy, accident, education, etc.
- Each website is denoted by a number.
- So for instance, page 2 means it’s a sports page.


## Pre-processing of data:
Each row represents a user.
So basically we are gonna cluster each row.
For that we need a feature vector that represents each user/row.
So we form a n*14 matrix, where n is the number of users, 14 is the no of pages in msnbc.com.
Each user is represented by their page visits.
Now we have the dataset ready, deploy all your algorithms using the data.


## How to check and run the code: 
Just open the codes under code folder in google colab
It has all the required tutorial links and documentations.

## Output:
You can check the final output in index.html page (wait for a couple of seconds to load)


