# crime-prediction
Business Question:
Original business question was to predict what volume of Part 1 crime activity might a police district in Baltimore City expect for the most common Part 1 crimes based on day of week, date, time of day, holidays, neighborhood, location, temperature, precipitation, and other possible features. 

Through exploration of the Part 1 crime dataset from Baltimore City, adjusted business problem. The final business problem was to attempt to predict the daily volume of Part 1 crimes in Baltimore City’s Northeast Police District based on features of the day. These features were the day of the week (e.g., Monday, Tuesday, etc.); whether the day was a holiday; the minimum, maximum, and average temperature; the average wind speed; the total precipitation; whether it was in the winter; and whether there was a thunderstorm, mist, or fog on the day.

Methodology to Answering the Business Problem:
Approach to this project was to follow the CRISP-DM methodology and to use supervised learning with regression models.

Data Understanding:
After drafting the business question, collected the Part 1 crime dataset from Open Baltimore City and the weather dataset from the National Center for Environmental Information (NCEI). The crime dataset was in a usable format. However, the weather dataset needed processing to a usable format. 
Collected Part 1 crime data from Baltimore City and weather data from National Center for Environmental Information with NOAA.
https://data.baltimorecity.gov/datasets/baltimore::part-1-crime-data/explore 
https://www.ncei.noaa.gov/access/search/dataset-search 

The following shows the volume of crime in each district and the volume of each crime description. 

![image](https://github.com/sreya134/crime-prediction/assets/125150816/68fbb16e-e669-4437-80ba-1c0b40eefe67)




