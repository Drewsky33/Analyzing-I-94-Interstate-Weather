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
