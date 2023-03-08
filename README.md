# Bikesharing with Tableau
Use tableau to visualize NYC City-Bike data to help make the case for starting a City-Bike inspired company in Des Moines, Iowa.

[link to my City-Bike Story](https://public.tableau.com/views/20230306_City_Bike_Story/City_Bike_Story?:language=en-US&:display_count=n&:origin=viz_share_link)


## Overview

Data from City-Bike, a bike sharing transportation company similar to Bird or Lime scooters, was analyzed to highlight what makes the platform practical in NYC. The practicality of these aspects were then tested against the idea of operating a similar bike sharing business in Des Moines, Iowa.

To observe what made the platform practical in NYC, we asked the following questions:

- What specific features (weather, topography) of NYC allow for the city-bike to be appealing to customers?

- Are there specific areas in NYC that are more likely to attract customers to paying for the city-bike services?

- What types of customers are consuming the city-bike platform? (Subscribers vs. One-time purchasers, Male vs. Female, age demographics, etc.)


With these questions in mind, I went about analyzing bikesharing data to find out what made City-Bike so successful in New York City.

### Analysis

I then made visualizations to address these questions. For example, to address what specific features of the city contributed to more successful starting city-bike locations, I plotted the City-Bike station location latitudes versus longitudes. Tableau automatically generated a map of Manhattan with each City-Bike station as a blue marker. Furthermore, different data could be interpreted from each marker by coordinating these markers to have their size and color change by the number of times customers would ride each city bike. This would help give insights into the popularity of certain locations of the city for building City-Bike locations.

To address the question of what types of customers participated in the City-Bike platform, I plotted the average ride trip duration by the number of bikes. From this information, I could determine what was the most common duration of a City-Bike ride (in minutes).

One other important additional question to answer was what were the most common times of the day and week that City-Bike rides occurred. And also, what was the gender demographic of these customers and how it might influence which times of the week these customers took City-Bike rides. This data was specifically plotted as a series of heatmaps. By plotting two time parameters such as Hours of Starttime on the y-axis and Days of Stoptime on the x-axis, and set the count of records value as in influence on the colors mark in Tableau, I could see a heatmap of data and could interpret which times of the week were the busiest for City-Bike rides based on the darkness or lightness of specific colors.

Its important to obtain as much data as we can, regarding the parameters previously discussed, to convince venture capitalists to fund the next bike sharing campaign in Des Moines, Iowa.

Let's look at this data in action in the next section.


## Results

![Top Starting Locations](https://github.com/willmino/bikesharing/blob/main/png%20of%20viz/Top%20Starting%20Locations.png)

One of the key parameters to determining the success of a bike-sharing company is the location in which the City-Bike is first presented to its customers. The location should be either of utmost practical use (ex: for daily commutes) or for pleasant recreational purposes.

Above is a plot of the location of each City-Bike station in Manhattan. In order to obtain more information from simple x,y coordinate pairs, each dot presenting a City-Bike station was modified by size and color parameters in Tableau to reflect the number of city bike rides. For example, the city bikes with the most individual rides were designated to be larger and darker blue in color. The city-bikes with fewer rides were then set to be smaller in size and lighter blue in color.

We can see that there are generally larger and darker circles, meaning more popular City-Bike stations in Lower and Midtown Manhattan. This is a good indicator that a majority of the popularity of City-Bikes can be due to the residents of NYC. Other areas of Manhattan Island, such as Harlem and Upper Manhattan, are separated from the corporate lifestyle and congestion of downtown Manhattan. For this reason, City-Bike stations in these areas are smaller and lighter in color, indicating less frequency of ride sharing. Thus, the areas of the city with generally the most activity, undeniably the downtown areas of Manhattan, serve as the most attractive locations for City-Bike stations. We will keep this in mind when we decide to make the case for a City-Bike station in Des Moines Iowa, carefully interpreting what areas of the new city may be ideal locations for City-Bike station.

![Checkout Times per User](https://github.com/willmino/bikesharing/blob/main/png%20of%20viz/Checkout%20Times%20for%20Users.png)

Further supporting the claim that the City-Bikes are primarily used by commuting residents of Manhattan, we can see in the above figure that the average trip duration per City-Bike ride is generally less than one hour. In fact, most of the data is actually less than 30 minutes in trip duration. This trip time is short and realistic for an every-day bike-ride. Short and realistic bike rides are ideal for NYC residents to commute to work. Longer bike-rides are too strenuous for recreational activity and also not practical for most people's commutes in NYC, since there are other methods of longer distance transportation such as subways.
However, we'll see later on that further evidence will suggest Manhattan residents are using the City-Bike to commute to work.


![Checkout Times by Gender](https://github.com/willmino/bikesharing/blob/main/png%20of%20viz/Checkout%20Times%20by%20Gender.png)

Further delving into the trip duration aspect of a City-Bike ride, we can see there is a male and female demographic to be interpreted. The male demographic in orange represents the majority of City-Bike rides in Manhattan. The female demographic represents a fraction of the number of bike rides compared to the number of bike rides in the male demographic. The unknown gender demographic represents the smallest portion of bike-rides. These three demographics are all reaching out for City-Bike services in Manhattan.


![Average Trip Duration](https://github.com/willmino/bikesharing/blob/main/png%20of%20viz/Average%20Trip%20Duration.png)

Examining the profile of City-Bike customers, we can draw conclusions from different age demographics in the plot above. While plotting age on the x-axis versus average trip duration on the y-axis, we can see that younger riders born between 1993 and 2003 are taking longer rides on average than riders born between 1945 and 1992. There is a cleaner resolution of the younger demographic because there are likely more data points. The resolution of the age group born between 1885 and 1940 is poor. This is likely due to a lower sample size of riders in this age range. Thus, in certain examples, if only one person is born in 1892 and 1969, as seen in the highest peaks in the dataset, its indicative of likely one data point. The length of these specific rides is far greater than any of the other rides and further suggests a small sample size.


![User Trips by Gender by Weekday](https://github.com/willmino/bikesharing/blob/main/png%20of%20viz/User%20Trips%20by%20Gender%20by%20Weekday.png)

The heatmap above, where the darkest colors are in the subscribers section, indicates that most City-Bike customers are subscribers. Its unlikely that mostly tourists of NYC would become subscribers to the local City-Bike services. Thus, the heatmap suggests most subscribers of City-Bike services are residents of NYC and furthermore they are daily commuters. It makes sense that daily commuters would take advantage of a bike that they don't have to store in their Manhattan apartment, and that they can have access to whenever it is convenient for them. The data further confirms there is a larger male demographic of City-Bike riders.


![Trips by Weekday for Each Hour](https://github.com/willmino/bikesharing/blob/main/png%20of%20viz/Trips%20by%20Weekday%20for%20Each%20Hour%20.png)

In the orange heatmap above, the busiest times for weekday City-Bike rides occur between the hours of 6 am to 9 am in the morning and 5 pm to 7 pm in the evening. This clearly indicates that City-Bike rides are most likely during weekday work commuting times. The higher activity during these times coincides perfectly with the average corporate American 9 to 5 work schedule. Due to the high concentration of corporate American building workplaces in Manhattan, all the data so far strongly indicates the City-Bike rides are a popular choice for commuting to work for Manhattan residents.


![Trips by Gender (Weekday per Hour)](https://github.com/willmino/bikesharing/blob/main/png%20of%20viz/Trips%20by%20Gender%20(Weekday%20per%20Hour)%20.png)

Finally, the last snapshot of our gender demographics reveal again that City-Bike riders are mostly male. This is indicated by the darker colors around the busiest weekday commute times in the MALE section of the figure. The lighter colors of the heatmap in the FEMALE section suggests that overall less riders are female. This could pose as a problem for future bike-sharing companies if the gender demographic of a city is not similar to that of Manhattan, New York. This could indicate that future advertising funding should be geared towards appealing to more women in Des Moines, Iowa for the future bikesharing company.

## Summary

Overall, its safe to draw the conclusion from this dataset that most of the NYC City-Bike customers are daily commuters. This was highlighted by several of the visualizations. For example, the blue heatmap revealed that most customers are subscribers. The Starting Station Locations visualization revealed that the most active City-Bike stations are in Lower and Midtown Manhattan. And finally, the orange heatmap visualizations revealed the most active times of City-Bike use are during morning and evening rush hours. All of these conclusions overwhelmingly suggest that daily commuter subscribers comprise the bulk of the customer base for the City-Bike bikesharing business. This is important to note because we need to determine if its not only possible to commute to work via bicycle in Des Moines, but also if there is enough 9 to 5 type workers who live in the city. These factors alone suggest a strong business model for the success of the City-Bike bikesharing services in Manhattan, New York. If Des Moines, Iowa does not turn out to accommodate these features, then another approach to applying the bikesharing services platform in this city may be required.

With this in mind, if we wanted to be sure about our decision to start the bikesharing platform in Des Moines, Iowa, we better dig deeper into some of the factors that impacted the popularity of ridesharing in certain circumstances.

### Additional Visualizations

1. From 5pm to 7 pm on Wednesdays in Manhattan, there are 30% less rides compared to other weekdays at that time. Without context, this data might not make sense. I would suggest the Des Moines, Iowa bikesharing company create a future data parameter called "Status" for each bike. The values for status would be 'ACTIVE', 'INACTIVE', or 'IN REPAIR'. If a figure like this could provide an easily interpretable readout, we could drill down further into datasets to find out why bike traffic is less on Wednesdays. Before performing this additional analysis, the first step would be to carry out the same analysis on an additional summer month's dataset in Manhattan. If the July 2019 or September 2019 heatmap City-Bike number of rides was still lower on Wednesday from 5 pm to 7 pm compared to the other days of the week, then we could tell there may be some unique aspect of either Manhattan, or the City-Bike program that is decreasing the amount of City-Bike rides taking place on Wednesday evenings. 

Thus, this additional analysis can be carried out by taking the COUNT of the rows of data of City-Bikes where the Status value is 'IN REPAIR'. If we see there are more bikes with an 'IN REPAIR' status during this time compared to other days of the week, it would be a direct indicator that City-Bikes in New York were in need of repair for some reason during this time. It is a good process to uncover unforeseen circumstances such as this to make sure there are no unknown factors that could be leading to a decrease in business and profitability of bike sharing services in a city.

2. Create a map plot which shows the starting station latitude and longitude along with the ending station latitude and longitude. Then, you can drag the "start station ID" and "end station ID" values to the details mark and colors marks. Select a different color for each starting station ID and ending station ID and create a line that stretches from the starting station location to the ending station location. In this way, we can view the trip path for each City-Bike and calculate the distance traveled during a given trip. This would help with metrics that would improve feasibility and practicality of City-Bike station locations. For example, it would be unwise to put a bike sharing station locations at the beginning and end of a route that requires the customer to go uphill both ways. This is a practicality issue that one might not be able to interpret readily from this dataset. Adding this extra layer to the data will help greatly improve the practicality for picking locations for ridesharing bikes.
