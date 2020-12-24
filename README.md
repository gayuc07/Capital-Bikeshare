# Capital Bikeshare

![Bikeshare](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/bike.JPG)

Capital Bikeshare (also called CapBi) is a bicycle sharing system that serves Washington DC, Arlington County, Alexandria, Falls Church, Montgomery County, Prince George’s County, and Fairfax County. The Capital Bikeshare system is owned by the local governments and is operated by Motivate International, Inc.(Motivate International, Inc). As of August 2019, Capital Bike has 500 stations and 4300 bicycles.

The distribution of the docks is shown below:

![Map](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/map.JPG)

As we can see from the above image, the majority of the docks for the bicycle are in Washington DC.

Bike tours in Washington DC are not only a popular family activity but renting a bike is a great way to get around without breaking the bank or sitting in traffic. There are dedicated bike lanes in Washington DC hence there is safety and convenience for the rider.

Capital BikeShare is undoubtedly cheaper than its competitors and the docks are conveniently placed around monumental locations. Capital Bikeshare is often faster than other modes of transportation and its annual membership offers unlimited trips under 30 minutes which helps save money. CapBi can be used to commute to work or ride to meet friends and is a great alternative for exercise since it is human-powered instead of electric powered. CapBi services save fuel, prevents carbon emissions, it is not only healthy for the rider but also for the environment.

As CapBi services are very popular and always in demand, we want to predict the number of bikes riders will use per hour and have contingencies to fulfill the demand. To estimate the number of bikes required we will consider various factors such as weather, temperature, working or non-working hour, the hour of the day, etc.

## Exploratory Data Analysis

### Bike Demand by Season and Temperature

From the plots below we can see that winter is the least favorite season for hiring bikes while spring, summer, and fall have pretty similar patterns.

![season](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/bike_per_Season.JPG)

In this plot we also include the temperature, and observe that higher numbers of bikes are rented in each season when temperatures are between 80-90 degree Fahrenheit.

![Temperature](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/bike_temp.JPG)

### Bike Demand by Weather Conditions

The plot shows that people like to bike most in cloudy weather, followed by fair. Rain, snow, windy etc. are not preferred.

![Weather condition](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/bike_weather_condition.JPG)

### Bike Demand by Year, Weekday & Hour of the Day

There is a steady increase in the number of bikes rented up to the year 2017 and then it decreased in 2018. Also, more bikes are hired during the weekday as compared to weekends.

![weekend](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/bike_weekend.JPG)

The bikes hired peak during morning and evening 8 AM and 6 PM rush hours when people are heading or returning back from work.

![Hour](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/bike_hour.JPG)

### Bike Demand by Holiday

We notice that riders rent bike more often on days when there is no holiday, but the number of bikes rented during holidays is still significant.

![Holiday](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/bike_holiday.JPG)

### Correlation Between Bikes Hired and Weather

There is a positive 44% correlation between temperature and bikes hired, additionally, Humidity has a negative correlation of 30%.

![Correlation](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/correlation.JPG)

## Model Assessment

Thus random forest performs the best with the R-square value being highest at 0.93.

![Results](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/Model_results.JPG)

![Feature_imp](https://github.com/gayuc07/Capital-Bikeshare/blob/main/Images/feature_imp.JPG)

## Conclusion

In terms of modelling & predictions, we can conclude that :

- Random Forest works best with the given dataset

- Maximum R2 value obtained is 0.93

- Variable Importance are as follows:

        + Hour of Day – Best 6PM-7PM,8-9AM

        + Weekday – Weekend

        + Time of Day – Working Hour

        + Temp – Moderate Temperature – 70–90F

The insights which we got from our analysis is that on a normal day, users tend to ride a bike for commuting to offices, schools, etc. But on weekends & holidays, people prefer to use bikes for travel and leisure activity purposes. We also derive that bikes are preferred maximum in moderate temperatures and users tend to avoid bikes at high temperatures and low temperatures.

Based on our analysis we recommend that during high demand in morning and evening office hours and weekend/holiday, Capital Bikeshare should increase availability during these hours. Thus catering to more users and in turn, securing more profits.

## Refrences

Motivate International, Inc. (n.d.). Press Kit. Retrieved November 26, 2019, from https://www.capitalbikeshare.com/press-kit.

Capital Bikeshare Discount. (n.d.). Retrieved November 26, 2019, from https://benefits.gwu.edu/capital-bikeshare-discount.

Therneau, T. M. (2019, April 11). An Introduction to Recursive Partitioning Using the RPART Routines. Retrieved November 26, 2019, from https://cran.r-project.org/web/packages/rpart/vignettes/longintro.pdf.



