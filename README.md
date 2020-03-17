# Analysis of Covid-19 data

## Current situation 
The new Coronavirus (Covid-19) is spreading quickly - we want to analyse if it follows an exponential trend and what this could mean, looking into the near future.

## Data
- case reports are published by JHU CSSE on github (https://github.com/CSSEGISandData/COVID-19) and updated on a daily basis. 
- the data includes daily report files and aggregated timeseries for confirmed, recovered and deaths numbers.
- The analysis was performed on data from 2020/03/16.

## Preparation of Data
- based on the timeseries data we determin the number of current infections and analyse the latest available numbers (2020/03/16)
- Missing Data: The provided dataset contained no missing data. 
- Removed Data: Some columns containing geographical information where dropped

## Data Modeling
- a simple exponential forecast model was fit to the timeseries data of infections
- r2 score was used to evaluate the model accuracy

## Evaluatation
- the fitted exponential Model was used to make a projection into the future
- we can se

## Code

libraries used:
- data wrangling: numpy and pandas
- Modelling: sklearn and scipy 
- plots: matplotlib

files:
- covid19_analysis.ipynb: contains the python code
- /JohnsHopkins Data/csse_covid_19_time_series: timeseries data from JHU
- /Bilder: contains images generated from analysis

## acknowledgements
- Novel Coronavirus (COVID-19) Cases, provided by JHU CSSE
- https://github.com/CSSEGISandData/COVID-19
- https://systems.jhu.edu/research/public-health/ncov/
