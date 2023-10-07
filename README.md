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
![image](https://github.com/sreya134/crime-prediction/assets/125150816/ca4e4679-275b-4876-a48a-58b7840ba3c2)

Data Preparation:
Many of the columns in the crime dataset contained null values. For example, 3% of observations had ethnicity completed, which is very low quality. However, for this business problem, most features in the crime dataset did not add value. Furthermore, I opted to focus on dates between January 1, 2010 and December 31, 2019. Therefore, most data quality issues were resolved simply by the removal of the columns and/or observations not necessary for this project. The weather dataset, however, did have missing values that needed to be filled in; accomplished this by using a backfill function.

Modeling
Used eight regression models on our dataset, and all yielded approximately the same results – an R2 between 0.42 and 0.49.  The Random Forest Regression model yielded the lowest R2 and the LightGBM regressor yielded highest R2 of 0.49. LightGBM is an open-source gradient boosting framework that is based on tree learning algorithm.

Evaluation
For evaluation purposes, focused on evaluating the Random Forest Regression model and attempted to improve its R2. For this regressor, the validation curve showed a large distance between R2 of the training set and validation set. Additionally, the validation curve displays a low R-squared value. The options for addressing this is to add new features, replace the model, or adjust hyperparameters.







