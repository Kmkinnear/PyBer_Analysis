# PyBer_Challenge

## Project Overview
The purpose of this project was to come up with a summarized DataFrame of our ride-sharing data that was broken out by "city type"(rural, urban, and suburban). Our DataFrame specifically looked at the date range of 1/1/19 - 4/28/19. After completing that, we created a multiple-line chart that showed the total weekly fares for each city type over our date range.

## Results
The first step in our analysis was to merge our two data files into one set of data by the "city" column. From there we were able to use code to determine our total ride count, total driver count, total fare amount, average fare per ride, and average fare per driver. We collected all this data which we broke out by our three city types. Then we were able to create a DataFrame using all our data which made it easier to read.

<img width="326" alt="image" src="https://user-images.githubusercontent.com/110848660/195378099-f33a4fb3-c029-400c-beee-2aa7dcc0ba57.png">

<img width="542" alt="image" src="https://user-images.githubusercontent.com/110848660/195378272-3ae78ea5-4465-49d9-a865-e5f30a71e03e.png">

There are a few takeaways that we can see by looking at this DataFrame:
  * Total Rides - There were significantly more rides in the urban city type compared to the suburban and rural ride counts. 
  * Total Drivers - The total driver number was significantly higher for the urban market compared to the other two city types. It was also interesting to see that the number of total drivers in the rural and suburban markets was less than the number of total rides. That means that riders likely always had plenty of drivers    available when they needed to schedule a ride. In the other two markets, you had better utilization with drivers doing multiple rides. 
  * Total Fares - This column wasn't too surprising when you factor in the number of total rides between the three different city types. There was a much higher ride count number for the urban city type and that's reflected again in the total fare column.
  * Average Fare per Ride - There isn't as big of a swing in this column compared to the other ones we looked at so far. It's likely that the average fare per ride is higher due to the rural rides going a further distance. It's hard to know where the rides went to in our data, but I suspect that the rural rides started in a rural area and ended up at an urban area. That meant more miles compared to an "urban area to urban area" ride that would be less mileage causing a lower fare amount.
  * Average Fare per Driver - This number had a big swing mostly due us dividing our "total fare column" by the low number of total drivers in the rural city type and the high number of total drivers in the urban city type. This caused the average fare for rural drivers to be much higher than the average fare of urban drivers.

After completing our analysis over the whole data set, we took a look at a smaller data range (January-April). We filtered our data and created a pivot table that showed the fare total for each week among the different city types. This photo shows a sample of our data that covered the first 10 weeks using the .head() function.

<img width="129" alt="image" src="https://user-images.githubusercontent.com/110848660/195389629-6c43d742-5217-496d-9b05-bf1136649dbb.png">

We were then able to complete the last step of our analysis which was to create a multiple-line chart displaying our "Total Fare by City Type" data using our smaller date range of data. This chart confirms what we looked at earlier with the urban rides accounting for the highest fares, the suburban fares being the second highest, and the rural rides having the lowest total fare amount. 

<img width="541" alt="image" src="https://user-images.githubusercontent.com/110848660/195392779-eafd81d7-c21b-4128-9486-f46424146714.png">

## Summary
We were able to come up with some recommendations based off our PyBer Analysis:
  * We should try and find a way to incentivize urban drivers to do some suburban or rural rides. There are more urban drivers than the number of rides so there are some drivers that aren't being utilized. Meanwhile, there are more rides than drivers in the rural and suburban areas. We can't see the number of cancelled rides in this exercise, but it's possible that some passengers are going to a competitor to find a ride or cancelling it altogether if the wait time is too much waiting on a driver.
  * We may need to increase our rates on the urban rides because the average fare is the lowest of the three. Part of that is due to the number or total drivrs in the urban area. It's also probably due to those being lower mileage rides than the other two city types. When we factor in that we have more drivers there than rides, we may have drivers that are struggling to find multiple rides. This means that they are stuck with low paying rides which means they aren't making as much money and may quit. Maybe we can come up with a "Short Ride" pay supplement to help drivers be more willing to accept shorter rides that would not hvae paid as much. 
  * We should also do some additional analysis and take a look at other factors like trip mileage and the time stamps of the rides. Looking at trip mileage would help us see what our fare amount per mile is and see if there are any big swings in the data. It would also shows us the average trip length among the different city types. If we see that the rural areas are having a lot of higher mileage trips, we may need to find a way to get drivers out there to help due to drivers being tied up on longer rides. Especially with the urban area already having more drivers than trips. One benefit of seeing the time stamps is that we can see if there are fluctuations throughout the day in certain areas. That would allow us to better place our drivers to maximize the number of rides we can take and not risk riders going with a competitor due to us not having enough drivers in the area. 
