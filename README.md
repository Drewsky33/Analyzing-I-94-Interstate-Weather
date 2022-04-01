# Analyzing-I-94-Interstate-Weather

During this project I attempted to analyze what kind of data from the dataset **Metro Interstate Traffic Volume** contributed most to heave traffic. The dataset can be located here: https://archive.ics.uci.edu/ml/datasets/Metro+Interstate+Traffic+Volume

The workflow of this project consisted of:
- Importing Packages
- Pulling in Data
- Segmenting Data
- Running statistical summaries on the data
- Exploring these summaries via data visualization
- Using data visualization to identify trends related to heavy traffic. 

The dataset dictionary can be seen below:

- `holiday` Categorical US National holidays plus regional holiday, Minnesota State Fair
- `temp` Numeric Average temp in kelvin
- `rain_1h` Numeric Amount in mm of rain that occurred in the hour
- `snow_1h` Numeric Amount in mm of snow that occurred in the hour
- `clouds_all` Numeric Percentage of cloud cover
- `weather_main` Categorical Short textual description of the current weather
- `weather_description` Categorical Longer textual description of the current weather
- `date_time` DateTime Hour of the data collected in local CST time
- `traffic_volume` Numeric Hourly I-94 ATR 301 reported westbound traffic volume

## Traffic Volume Analysis

<img width="595" alt="image" src="https://user-images.githubusercontent.com/77873198/161188392-7e21a311-bf09-439b-8009-b86d4136d715.png">

### Observations of `traffic_volume`

- During the time frame **from 2012-10-02 09:00:00 and 2018-09-30 23:00:00** the hourly traffic volume ranged from 0 to 7,280 cars. 
- The average number of cars was around 3,260 cars. 
- Around 25% of the time there 1,193 cars. 
- 75% of the time there was 4,933 cars. 

## Visualizing the differences between traffic_volume: Day vs. Night
<img width="641" alt="image" src="https://user-images.githubusercontent.com/77873198/161188601-1cb36676-0590-489a-8cc1-1e73c4363145.png">

<img width="597" alt="image" src="https://user-images.githubusercontent.com/77873198/161188838-82e86de9-dd3a-4fb4-9d8b-327cee280581.png">

### Analysis

Day
- The histogram above shows that the distribution of the day-time traffic volume is left-skewed. Interpreting this, I'd say that most of the traffic volumes are high. 75% of the tie there are more than 4,252 cars in traffic. 

Night
- The histogram for the night traffic volume histogram is right skewed indicating that the traffic volumes during this time of day are relatively small overall. 
- The average number of cars during this period are 1,785 cars. 
- 75% of the time the number of cars passing the station was less than 2,819. 
- There are a few points where the number of vehicles gets above 5,000, but overall the totals at night are much lower than during the daytime.


## Exploring time as an indicator of Heavy Traffic- (Line chart)

<img width="597" alt="image" src="https://user-images.githubusercontent.com/77873198/161188759-b40f1cf7-f2af-4942-8658-3db8f9c45b27.png">

### Observations (Month)

- First, the traffic volume numbers seem to tumble during the winter months and start to rise when Spring comes. 
- There's an exception to this observation though. Traffic plummets during the warm month of July? What could be the cause of this? Summer vacation? People avoiding the heat?

## Time as an indicator by day (Grid Chart)

<img width="625" alt="image" src="https://user-images.githubusercontent.com/77873198/161189061-33e5d819-f487-4dc7-b620-6595e668fc9c.png">

### Observation

The traffic is generally higher at every hour of the day compared to on the weekend. The rush hour on weekdays tends to be around 5:00 pm. 

#### Weekdays
- The quiet period is from 10:00 am until 2:00 pm. The exception to this is when people return home in the afternoon around 6:00 pm.

#### Weekends
- Traffic on the weekends peak from 7:00 am until around 12:00 pm. 

## Weather Indicators Traffic vs. Volume (Scatterplot)

<img width="541" alt="image" src="https://user-images.githubusercontent.com/77873198/161189217-ff50d68d-12b7-4b71-9a2e-5b964e649879.png">

### Observation
- Looking at the chart above there doesn't seem to be a correlation in either the positive or negative direction when `temp` and `traffic_volume` are compared. Therefore, temp isn't a reliable indicator for heavy traffic. 

## Weather types as an Indicator (Horizontal Barplot)

<img width="632" alt="image" src="https://user-images.githubusercontent.com/77873198/161189339-1441557a-64ab-4490-9a85-f5b5a112cf33.png">

### Observations
- There are no weather types that exceed 5000 cars. It's difficult to ascertain whether or not `weather_type` is a reliable indicator of heavy traffic. 


## Final Conclusions

### Conclusion

During this project we had a look at two possible indicators of heavy traffic on the I-94 Interstate Highway. These indictators were:

- Time Indicators
    - Summer months typically have heavier traffic volumes. 
    - Traffic is heavier during the week. 
    - The rush hour for traffic on weekdays starts around 5:00 pm. 
    
- Weather Indicators
    - light snow
    - heavy snow
    - Thunderstorms in close proximity with drizzle. 


