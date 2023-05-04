# Big Data Analysis White Paper

This is a report on the impact of the epidemic on the aviation industry.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the package to run the python code

```bash
pip install pandas numpy statsmodels
```

## Datasets

Some raw datasets are too large to upload in Canvas, we upload them in google drive instead. All datasets must be placed in a relative directory named "./dataset" under the same directory name as the Python file.

The method to read the datasets in Python would be 

```Python
import pandas as pd

df = pd.read_csv('./dataset/airline.csv')
```
### Raw data

1. cb_2017_us_county_5m: This is a file containing information about counties in the United States, including their boundaries and other relevant data.

2. cb_2017_us_state_5m: This is a file containing information about states in the United States, including their boundaries and other relevant data.

3. US_counties_COVID19_health_weather_data.csv: This is a CSV file containing COVID-19 cases, health, and weather data for counties in the United States.

4. COVID-19_Vaccinations_in_the_United_States_County.csv: This is a CSV file containing information about COVID-19 vaccinations in counties in the United States.

5. alljoined_airlines.csv: This is a CSV file containing information about all airlines from 18-22, including their origin airports, destination, cancellation, cancellation reason, and other relevant data.

6. airline key.csv: This is a CSV file containing an identification code for each airport in the alljoined_airlines.csv file.

7. airport info.csv: This is a CSV file containing information about airports, including their names, locations, and other relevant data.


### Generated data
1. covid_airline.csv: This is a CSV file after merging covid and airlines datasets, containing airline data, including the county's name, number of flights, number of cancellations, etc.

2. covid_geo.csv: This is a CSV file containing geographical information about covid, such as location and population data.

3. airline_county_gdf.csv: This is a CSV file containing information about the airlines and counties, including their locations, names, and other relevant data.

4. covid_county_week.csv: This is a CSV file containing information about the number of COVID-19 cases in different counties, organized by week.

5. covid_clean_df_date.csv: This is a cleaned version of the COVID-19 data, organized by date.

6. geo_airports_week.csv: This is a CSV file containing information about the airports in different locations, organized by week.

7. us-counties.csv: This is a CSV file containing information about counties in the United States, including identical the state and county code.

8. covid_gdf.csv: This is a CSV file containing information about COVID-19 cases, organized by location.

9. geo_airports.csv: This is a CSV file containing information about airports, including their locations and names.



## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.
