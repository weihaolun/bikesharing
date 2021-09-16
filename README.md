# CitiBike Analysis with Tableau

## I. Project Overview

### Background

Kate traveled to NYC last summer and enjoyed riding CitiBike everywhere, which allowed her to really get to know the city and interact with the people who live there and who are using bikes for their communities. 

A gem of an idea starts to form in her mind. What if she could start a similar Bike Share business for her hometown of Des Moines, Iowa. I have been helping Kate to brainstorm, and with support from a potential investor who might be interested in providing seed funding to explore a bike share program in Des Moines.

For the first step, we have decided to figure out how the Bikeshare business actually works in New York City. From there, we will have a proposal on how it might work in Des Moines. Since I have data analysis experience, I will conduct a thorough analysis on CitiBike data from August 2019 and visualize the result using Tableau. 

### Purposes

The purpose of this analysis is to get a deep understanding of NYC CitiBike data and created a solid business proposal to convince investors that a Bikesharing program in Des Moines.

For this analysis, I have used Pandas to clean the data, then created set of visualizations story using Tableau.

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

The is page shows an overview of August 2019 CitiBike data. Within one month, there are 2,344,224 rides, 69,037,166,989 bikes available in the city, and 2,344,135 stations in operation. Among all the rides, there are 81.07% taken by loyalty program subscriber, 18.93% by regular customers; 65.28% taken by males, 25.10% by females and 9.62% with undefined gender. From the overview we can conclude that there are 78,140 rides taken per day in average, and male subscribers are the main customers.

<img width="1440" alt="1  Overview" src="https://user-images.githubusercontent.com/84211948/133383868-2ae4188e-9276-4709-bd12-01b2966c20c5.png">

**2. Checkout Times for Users**

The graph shows the distribution of checkout times, which are the trip durations between checkin and checkout of bike ridings. The peak is at 5-6 minutes, which indicates that more than 140K trip durations are as short as 5-6 minutes. Most rides are checked out within 50-40 minutes and remaining small number of rides exceed one hour. We can make two conclusions according to this graph:
1.	A large number of stations are very close to each other, within distances of minutes of bike ridings.
2.	Many users prefer to ride bikes when the distances are short, very likely that too short to take public transportations but good to ride bikes to avoid walking in hot summer.

<img width="1440" alt="2  Checkout Times for Users" src="https://user-images.githubusercontent.com/84211948/133383887-97aca310-6464-4601-91d1-9167be4d39ad.png">

**3. Checkout Times by Gender**

Similar to the previous graph, this page also shows the checkout times, while also divided by genders. The gender breakdown is included on this board as a reference. The trip duration trend for each gender has similar pattern to the overall users’: peak at 5-6 minutes and mostly within 50 minutes. At the same time, we can conclude that the distribution of number of rides among genders also follows the gender breakdown.

<img width="1440" alt="3  Checkout Times by Gender" src="https://user-images.githubusercontent.com/84211948/133383904-ef5057d4-2f1d-444d-9263-ae6883f06f02.png">

**4. Trips by Weekday for Each Hour**
<img width="1440" alt="4  Trips by Weekday for Each Hour" src="https://user-images.githubusercontent.com/84211948/133383928-d1266f38-4223-4765-a798-b897fffe2d29.png">

**5. Trips by Gender (Weekday/Hour)**
<img width="1440" alt="5  Trips by Gender (Weekday:Hour)" src="https://user-images.githubusercontent.com/84211948/133383953-1f59e977-344b-4184-8f23-4b25bc0836fd.png">

**6. User Trips by Gender (Usertype/Weekday)**
<img width="1440" alt="6  User Trips by Gender (Usertype:Weekday)" src="https://user-images.githubusercontent.com/84211948/133383979-ddc48782-8fb7-4af6-9785-0d5204dba9b8.png">

**7. Top Starting and Ending Locations Map**
<img width="1440" alt="7  Top Starting and Ending Locations" src="https://user-images.githubusercontent.com/84211948/133383991-017f5068-f1be-4908-9596-601eb0689f56.png">

**8. Average Trip Duration**
<img width="1440" alt="8  Average Trip Duration" src="https://user-images.githubusercontent.com/84211948/133384688-78bac614-f601-48cb-99ac-01cea5a19a62.png">

## III. Summary

**1. Top 20 Stations IDs**
<img width="1440" alt="9  Extra 1 Top 20 Stations" src="https://user-images.githubusercontent.com/84211948/133384057-986392f0-688f-407f-a3ef-2844e05e5516.png">

**2. Stations by Usertype**
<img width="1440" alt="10  Extra 2 Stations by Usertype" src="https://user-images.githubusercontent.com/84211948/133384074-ab309328-a305-4888-85b7-a616503a542a.png">
