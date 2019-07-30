# Lyft - Baywheels Data Exploration
### Data from January 2019 to June 2019
## by Gautam Gadiyar

## Introduction

> The Lyft - Baywheels is a Bike sharing company that rents out bikes to customers who may hire a bike from any nearest point. It was a partnership program with Metropolitan Transportation Commission in order to motiate people to use envireonnment friendly means of transport. Beginning operation in August 2013 as Bay Area Bike Share, the Bay Wheels system currently has over 2,600 bicycles in 262 stations across San Francisco, East Bay and San Jose. On June 28, 2017, the system was re-launched as Ford GoBike in a partnership with Ford Motor Company.<br>
After Motivate's acquisition by Lyft, the system was subsequently renamed to Bay Wheels in June 2019.The system provides bikes 24/7 to customers at nominal costs. The customers have access to all the bikes once they are a member or have a pass for themselves.


## Dataset

The dataset was a combination of 6 datasets, one for each month starting from Jan 2019 to june 2019. There were a total of 1.2 million records after the datasets were combined.The dataset mainly deals with the different stations, start and ends times, duration of trips, gender of users etc. This data was quite clean and there was minimal cleaning required.<br>

The following is the dataset link:<br>
https://s3.amazonaws.com/baywheels-data/index.html
<br>
The dataset had the following features:
<ul>
<li> Duration in seconds</li>
<li> Start time</li>              
<li>End_time</li>                   
<li>Start_station_id</li>           
<li>Start_station_name</li>         
<li>Start_station_latitude</li>     
<li>Start_station_longitude</li>    
<li>End_station_id</li>             
<li>End_station_name</li>           
<li>End_station_latitude</li>       
<li>End_station_longitude</li>      
<li>Bike_id</li>                    
<li>User_type</li>                  
<li>Member_birth_year</li>          
<li>Member_gender</li>              
<li>Bike_share_for_all_trip</li>    
<li>Member_age</li>                 
<li>Distance_travelled</li>
</ul>
As we can see the data is mostly numeric and good to take out useful stats.


## Summary of Findings

The dataset was very insightful and gave good understanding of the trends towards the service. Lets go step by step.
<br>
#### Assess and Cleaning:
<ol>
<li> There were minor datatype changes required, like start and end time was converted to datetime.</li>
<li> The distance was in the form of coordinates which was not useful. The distance was calculated in kilometers.</li>
<li> The speed was calculated to gain some good insights.</li>

#### Exploration:
>The Initiative is a success story according to me as the service is being actively used by the people of the cities. The system is nice and easy to use which can be known from the number of subscribers that the system had. During the exploration it was found that more than 80% of the rides was by subscribers. This shows that customers are happy and are subscribing to the service.<br>
>For the exploration I had to find the speed, distance in km and also do some groupby to get the required data. The bike_id, station_id were some of the unique values that helped in finding the right exploration. It can be noticed that the 'Bike Share for All' initiative was started by Lyft but hasn't reached the masses yet. Hence we saw less than 10% being the initiative users.<br>
>The distance also was very short which shows that professional woring in the bearby localities used the service to get to work or to the University to study. Long trips were mostly carried by guest customers during the weekends. The distance travelled by Customers was more than the Subscribers.


## Key Insights

The gender gap was the main concern in the finding. A whopping 74% male user compare to females. This could mean that the females travelled less or did not prefer the service. This need more awareness among the ladies about the company and the service.<br>
The service was mostly used by people in the age group 20 to 40. This shows that it is mostly the working professional or students using the service. This was also confirmed from the fact that the peak usage of the service is during the working hours in the morning or in the evening.
<br>
An interesting thing is that the speeds of travel of ladies is quite better the the men. This was noticed for the subscribers where most of them travelled short distances. The customers trend was different though where men were faster.
<br>
The Market Street and San Francisco Caltrain station are teh favorites. There is a very good footfall in the region and the company can focus to put in a few more bikes if required. The commercial aspect of the are could be the reason for the heavy demand. Any any given time there will be a lot of people in the Markets or a staion. The Bike Share for all initiative can be marketed in these areas.<br>

