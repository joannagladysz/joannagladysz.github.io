---
title: Exploring the Airbnb 2024 market in Hawaii
date: 2025-03-13 12:40:00
categories: [Descriptive_Analysis, Projects]
tags: [powerbi, power query, airbnb, data cleaning]    # TAG names should always be lowercase
image:
  path: /assets/img/hawaiipost1.jpg
  alt: Kauaʻi - Photo by Braden Jarvis on Unsplash[^1]
---
*In this report, I will explore an Airbnb listings dataset to understand the short-term homestays market in Hawaii. To achieve this, I will apply a set of descriptive statistics and communicate my findings with data visualisations.*\
Recently, Hawaii has caught my attention and become my number one place to visit for a lifetime adventure, which I am yet to fulfil.  As a 90s kid, I learned about Hawaii from the animated Disney movie Lilo & Stitch, released in 2002. However, back then, it only seemed like a fictional place because it looked too good to be true.\
Well, yes, Hawaii is a tropical state island consisting of 137 smaller volcanic islands in the middle of the Pacific Ocean. It has a beautiful coastline and enormous volcanic mountains, and one of them, Mauna Kea, is taller than Mount Everest (if measured from the base). I may have already sparked your interest in Hawaii a little bit, but just before I move on, here are some extra number facts:

•	As of 2024, Hawaii’s **population** is estimated at around **1,446,146**[^2]\
•	As of 2023, their median household **income** is **$98,317**[^2]\
•	They have the 4th longest ocean **coastline** in the U.S., measuring around **1,210** kilometres (750 miles)[^3]

**Objectives**\
Now, let’s dive into my dataset exploration, where I will be looking at different areas of Hawaii, property types, reviews and prices. The purpose of this is to understand the short-term lettings accommodation market and draw some conclusions which will help to plan my trip. Here are some points I am going to cover:\
•	Neighbourhoods per island diagram\
•	Number of listings per island part\
•	Property type popularity\
•	Price range (min and max) per island part\
•	Map of listings\
•	Which property type is more likely to have 2 bathrooms per 2 bedrooms (when two couples want to share an apartment but want to have two separate bathrooms)\
•	Does a higher price correlate with a higher rating\

**The Dataset**
The dataset contains listing details obtained from web scraping on the Airbnb website dated 12th December 2024. 

| columns    | 75       |
| rows | 35,493       |

Key information in the dataset includes:
•	host details, e.g. name, host since date
•	host performance/stats, e.g. total listings, response rate
•	property details, e.g. bedrooms, bathrooms, price
•	location data, e.g. latitude, longitude, area
•	review scores, e.g. number of reviews, review scores

**Data Transformation**
Using the Power Query Editor in Power BI, I prepared my dataset by applying the following steps:
1.	Remove unnecessary columns
a.	Remove all URL columns
b.	Description (long strings)
2.	Handle missing values
3.	Convert the data type of the price column to numeric
4.	Split the bathrooms_text column into two to separate the numeric values from a string
5.	Add an index column


**Reference**

[Dataset source: https://insideairbnb.com/get-the-data](https://insideairbnb.com/get-the-data/)\

[^1] [Kauaʻi - Photo by Braden Jarvis on Unsplash https://unsplash.com/@jarvisphoto](https://unsplash.com/@jarvisphoto)

[^2] [U.S. Census Bureau: https://www.census.gov/quickfacts/fact/table/HI/PST045224](https://www.census.gov/quickfacts/fact/table/HI/PST045224)\

[^3] [Table – Method 1 (CRS) https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_coastline](https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_coastline)
