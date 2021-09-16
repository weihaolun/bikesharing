# CitiBike Analysis with Tableau

## I. Project Overview

### Background

Kate traveled to NYC last summer and enjoyed riding CitiBike everywhere, which allowed her to really get to know the city and interact with the people who live there and who are using bikes for their communities. 

A gem of an idea starts to form in her mind. What if she could start a similar bikesharing business for her hometown of Des Moines, Iowa. I have been helping Kate to brainstorm, and with support from a potential investor who might be interested in providing seed funding to explore a bikesharing program in Des Moines.

For the first step, we have decided to figure out how the bikesharing business actually works in New York City. From there, we will have a proposal on how it might work in Des Moines. Since I have data analysis experience, I will conduct a thorough analysis on CitiBike data from August 2019 and visualize the result using Tableau. 

### Purposes

The purpose of this analysis is to get a deep understanding of NYC CitiBike data so that Kate can create a solid business proposal to convince investors that the bikesharing program in Des Moines will success.

In this analysis, I first used Pandas to clean the data, then created a set of visualizations story using Tableau.

**The analysis includes:**
  1.	The length of time that bikes are checked out for all riders and genders.
  2.	The length of time that bikes are checked out for each gender.
  3.	The number of bike trips for all riders and genders for each hour of each day of the week.
  4.	The number of bike trips for each type of gender for each day of the week.
  5.	The number of bike trips for each type of user and gender for each day of the week.
  6.	Top starting and ending stations for all users on maps.
  7.	Average trip duration by ages.

**In Summary section, I will also provide two further analysis recommendations.**
1.	Top 20 stations’ ID and names.
2.	Starting and ending stations by user type.

## II. Results

**1. Data Overview**

This page shows an overview of August 2019 CitiBike data. Within one month, there are 2,344,224 rides, 69,037,166,989 bikes available in the city, and 2,344,135 stations in operation. Among all the rides, there are 81.07% taken by loyalty program subscribers and 18.93% by regular customers; 65.28% taken by male users, 25.10% by female users and 9.62% users with undefined gender. From the overview we can conclude that there are 78,140 rides taken per day in average, and male subscribers are the main customers.

<img width="1440" alt="1  Overview" src="https://user-images.githubusercontent.com/84211948/133383868-2ae4188e-9276-4709-bd12-01b2966c20c5.png">

**2. Checkout Times for Users**

The graph shows the distribution of checkout times which are the durations between checkin and checkout of bike ridings. The peak is at 5-6 minutes, which indicates that more than 140K trip durations are as short as 5-6 minutes. Most rides are checked out within 50-40 minutes and remaining small number of rides exceed one hour. We can make two conclusions based to this graph:
1.	A large number of stations are very close to each other, within distances of minutes of bike ridings.
2.	Many users prefer to ride bikes when the distances are short, very likely that too short to take public transportations but good to ride bikes to avoid walking in hot summer.

<img width="1440" alt="2  Checkout Times for Users" src="https://user-images.githubusercontent.com/84211948/133383887-97aca310-6464-4601-91d1-9167be4d39ad.png">

**3. Checkout Times by Gender**

This dashboard shows the trip durations by genders. The gender breakdown is included on this board as a reference. The duration trend of each gender has similar pattern as the overall users’: peak at 5-6 minutes and mostly within 50 minutes. Moreover, we can conclude that the distribution of ride counts among genders also follows the gender breakdown.

<img width="1440" alt="3  Checkout Times by Gender" src="https://user-images.githubusercontent.com/84211948/133383904-ef5057d4-2f1d-444d-9263-ae6883f06f02.png">

**4. Trips by Weekday for Each Hour**

The dashboard below includes two graphs. The top graph is a heatmap shows the number of rides by weekday for each hour of the day. The bottom graph is a bar chart to reference the average peak hours during a day.

Conclusions from this dashboard:
1.	Weekday morning rush hours are peak times for CitiBike ridings. A variety of reasons can explain this trend, such as that many users ride bikes to get to work to avoid possible delays by public transportation, or just for keeping a healthy habit.
2.	Weekday afternoon rush hours are also peak times for CitiBike usage. Bike riding is a great way for city residents to surpass rush hour traffics.
3.	It is very interesting to see that Wednesday afternoon rush hour is an exception and is worth to research the cause behind. 
4.	In addition, Friday’s afternoon usage of CitiBike starts as much earlier, as many workplaces allow employees to get off work earlier on Fridays. Friday’s morning / afternoon rush hours are still busy but not as much as the other days. 
5.	For weekends, more bike rides are taken between 10am and 5pm. People tend to get up later on weekends and ride CitiBikes to enjoy the city on weekends. 

<img width="1440" alt="4  Trips by Weekday for Each Hour" src="https://user-images.githubusercontent.com/84211948/133383928-d1266f38-4223-4765-a798-b897fffe2d29.png">

**5. Trips by Gender (Weekday/Hour)**

This heatmap shows the number of bike rides by genders for each hour of each day of the week. The usage trends of male and female users are the same as the previous analysis, and male and female users share the same pattern. Except that the male count of rides is much larger than female count along with the gender breakdown. The pie char of gender breakdown is included on the right side on the dashboard again for reference.  

For undefined gender section, we see a pattern that more users take bike rides on weekends. This fact will be analyzed in the following page.

<img width="1440" alt="5  Trips by Gender (Weekday:Hour)" src="https://user-images.githubusercontent.com/84211948/133383953-1f59e977-344b-4184-8f23-4b25bc0836fd.png">

**6. User Trips by Gender (Usertype/Weekday)**

This dashboard includes a heatmap on the number of bike rides by both gender and user type for each day of the week. And both gender breakdown and user type breakdown pie charts are included as references.

As mentioned above, unsubscribed customers tend to ride more on weekends and subscribers ride more on weekdays. This is because most users who take bike rides on weekdays would prefer subscription programs for regular usage and potential promotions. People who don’t take bike rides on weekdays may just prefer to ride bikes on weekends for exercises or city exploration occasionally. Another possible reason is that part of unsubscribed users are just temporary tourists from other cities and areas. These customers are very unlike to be attracted by subscription.

Another interesting point is that all subscribers have their gender defined in the database. The company does a great job on collection information from subscribe users, and may be necessary to enhance data collection for unsubscribed users.

<img width="1440" alt="6  User Trips by Gender (Usertype:Weekday)" src="https://user-images.githubusercontent.com/84211948/133383979-ddc48782-8fb7-4af6-9785-0d5204dba9b8.png">

**7. Top Starting and Ending Locations Map**

The maps below indicate the most popular starting and ending stations in the city. The markers are colored and sized based on ride counts. We can easily see from the visualization that the distributions of markers have the same pattern on the two maps. 

Several popular areas are: Midtown area in both West and East along Broadway, Midtown West along Hudson River, Greenwich Village in Lower West, Lower Manhattan along Hudson River, Lower Manhattan, and around Central Park.These areas are full of businesses, tourist attractions, schools, residential buildings and public transportation hubs, so there are more CitiBike stations available in these areas. 

Upper Manhattan and Queens are less popular. Population distributions in these areas are less dense than in other areas as well. Especially in Queens, more people would choose public transportation due to the longer distance.

<img width="1440" alt="7  Top Starting and Ending Locations" src="https://user-images.githubusercontent.com/84211948/133383991-017f5068-f1be-4908-9596-601eb0689f56.png">

**8. Average Trip Duration**

This dashboard includes two area graphs of the average duration of bike rides by age. The top chart is generated from the raw data, where we can see the birth year starts as early as 1885. By common sense, we can conclude that this set of data must contain some invalid data. Besides unrealistic data, the birth year of 1969 also stands out as an outlier. It could be possible that 50-year-old users in average rides for the longest duration as 50 is the age when people start to pay more attention to health. However, it would be a very extreme case and is hard to determine the validity. The cause to the  invalidity might be that users, especially unsubscribed users input a random birth year during registration as many people consider age as an important privacy.

To keep the sufficiency of the analysis, we should filter out invalid data and outlier for a more accurate analysis. I chose birth year range from 1945 to 2002 and removed 1969. We can see a more consistent data from the adjusted area graph below. In this chart, we see a significant increase in trip duration after 1994. Therefore, users at 25-year-old and younger have longer trip durations. 

<img width="1440" alt="8  Average Trip Duration" src="https://user-images.githubusercontent.com/84211948/133384688-78bac614-f601-48cb-99ac-01cea5a19a62.png">

## III. Summary

Main points to summarize the visualized analysis above:
1.	Male users and subscribers are the main userbase.
2.	Majority rides take less than one hour, and young aged people tend to ride longer in time.
3.  There are more rides during rush hours on weekdays, then followed by weekends daytime.  
4.	Most rides are taken in city centers.

In conclusion, for Kate to start a bikesharing business in Des Moines, she should first build stations in the busiest areas of the city, especially business districts where locate more office buildings to get a good start. Then, she can spread the business by building more stations around those areas. The busier the area is, the denser and larger the stations should be. Maintenance should be scheduled outside of busy hours, such as after 12am. For marketing, Kate can focus on male young age population first and create effective marketing strategies to attract subscribers. Overall, the potential of bike sharing business in Des Moines is very strong.

### Recommendations for further analysis

**1. Top 20 Stations IDs**

The first recommendation for further analysis is to conclude the top 20 starting stations and top 20 ending stations as shown in the dashboard below. The x-axis shows the station ID, and the tooltip includes the station name. The purpose of this analysis is to provide support to potential expansion plans. For top starting stations, CitiBike may consider adding more bikes, and for top ending stations, CitiBike can consider expanding the station to hold more bikes.

<img width="1440" alt="9  Extra 1 Top 20 Stations" src="https://user-images.githubusercontent.com/84211948/133384057-986392f0-688f-407f-a3ef-2844e05e5516.png">

**2. Stations by Usertype**

The second recommendation is to generate starting and ending station maps with markers colored by user type. As shown below, the legend on top right indicates that blue markers represents customers and red markers represents subscribers. However, on the maps, blue marks actually indicate stations used by both subscribers and customers because two colors overlaps on each other, while red markers indicate stations used by subscribers only. Bronx area has a number of starting and endings stations used by subscribers only; Jersey City area has several ending stations used by subscribers only. 

The purpose of this analysis is to explore potential marketing strategies based on user type. There are two popular attractions around the Bronx area: New York Botanical Garden and Bronx Zoo. It’s a convenient option to ride a bike from public transportation hub to the attractions The marketing team can market the advantage of CitiBike to tourists to increase unsubscribed userbase. For Jersey City, many people work in Manhattan and ride bikes to return home in Jersey City. It only takes 25 minutes to bike home from Lower Manhattan and approximately 45 minutes from Upper West Manhattan. The marketing team can utilize this type of usage to attract more subscribers in Jersey City area. 

<img width="1440" alt="10  Extra 2 Stations by Usertype" src="https://user-images.githubusercontent.com/84211948/133384074-ab309328-a305-4888-85b7-a616503a542a.png">
