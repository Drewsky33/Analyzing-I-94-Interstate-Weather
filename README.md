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

