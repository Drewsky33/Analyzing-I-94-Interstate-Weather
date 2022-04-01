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

### Analysis

Day
- The histogram above shows that the distribution of the day-time traffic volume is left-skewed. Interpreting this, I'd say that most of the traffic volumes are high. 75% of the tie there are more than 4,252 cars in traffic. 

Night
- The histogram for the night traffic volume histogram is right skewed indicating that the traffic volumes during this time of day are relatively small overall. 
- The average number of cars during this period are 1,785 cars. 
- 75% of the time the number of cars passing the station was less than 2,819. 
- There are a few points where the number of vehicles gets above 5,000, but overall the totals at night are much lower than during the daytime.

## Exploring time as an indicator of Heavy Traffic- Line chart

<img width="597" alt="image" src="https://user-images.githubusercontent.com/77873198/161188759-b40f1cf7-f2af-4942-8658-3db8f9c45b27.png">



