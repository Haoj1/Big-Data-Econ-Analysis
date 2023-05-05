# Big Data Analysis White Paper

This is a report on the impact of the epidemic on the aviation industry.

[Github Link](https://github.com/Haoj1/Big-Data-Econ-Analysis)

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

6. airline_key.csv: This is a CSV file containing an identification code for each airport in the alljoined_airlines.csv file.

7. airport_info.csv: This is a CSV file containing information about airports, including their names, identification codes, locations, and other relevant data.

8. passenger data csv: This is a CSV file containin the number of passengers of each airline company from 2002 to 2022, including both international and domestic.

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

### The link of the dataset

Since some of the datasets are too large (over 1 GB), we organize them into a google drive.

[Dataset Link to Google Drive](https://drive.google.com/drive/folders/1meuEqb81q4-Gjq2OZwNXn0zn1_0Vac5X?usp=share_link)

## Instructions of Python code and Dataset Dependencies

### Domestic and International Airline Analysis during Pandemic


1. ### Import required libraries: 
    - pandas
    - numpy
    - matplotlib
    - sklearn
    - geopandas

2. ### Load the raw datasets:
    - passenger_data.csv
    - COVID-19_Vaccinations_in_the_United_States_County.csv
    - alljoined_airlines.csv
    - airline_key.csv
    - airport_info.csv
    - cb_2017_us_county_5m
    - cb_2017_us_state_5m

3. ### Clean and preprocess the data:
    - Execute the AirportFilter.ipynb, CovidFilter.ipynb
    - Handle missing values
    - Convert data types
    - Remove unnecessary columns
    #### Generate clean data
    - geo_airports_week.csv
    - airline_county_gdf.csv
    #### Merged two datasets to study their correlation.
    - Execute Covid_Airline_Merge.ipynb
    - Generate covid_airline.csv

4. ### Analyze the data.
    - Execute Data_Analysis.ipynb
    - international_domestic_stuff.ipynb

5. ### Perform exploratory data analysis (EDA):
    - Plot histograms of the decreasing of airlines from 2018 to 2022
    - Plot scatter plots
    - Plot line plots to show the changes before and after pandemic

6. ### Perform statistical analysis:
    - Calculate the mean, median, and sum of the total airline numbers
    - Calculate the standard deviation
    - Perform hypothesis testing
    - Perform linear regression for hypotheses of possible correlation.

7. ### Create visualizations:
    - Plot bar charts
    - Plot line charts
    - Plot the result of each airport in a domestic geo graph 

8. ### Save the final analysis results to a file including all figures and regression results:
    - [Data_Analysis.html](https://github.com/Haoj1/Big-Data-Econ-Analysis/blob/main/Data_Analysis.html)
    - [international_domestic_stuff.ipynb](https://github.com/Haoj1/Big-Data-Econ-Analysis/blob/main/international_domestic_stuff.ipynb)


## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.
