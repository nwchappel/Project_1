# Project_1: Air Pollution, Income,  and  Health
Air pollution is a major healh concern and is associated with pulmonary morbidity and mortality. Some populations are particularly susceptible: children, elderly, and those of low socioeconomic status.

#Scope
We wanted to check if the Air Pollution had an effect on the population’s respiratory diseases by increasing the incidence in locations where the pollution is higher. We also wanted to see if it was any correlation of disease prevalence and complications with socioeconomic status. 
Air quality is measured by the Air Quality Index, AQI. AQI is calculated based on the concentration of 6 main pollutants: SO2 Sulfur Dioxide, NO2 Nitrogen Dioxide, CO Carbon Monoxide, O3 ozone and particulates PM2.5 and PM10. The polutions has an important effect on asthma, COPD, lung cancer and othe respiratory infections.  We use the data on the hospitalizations and death of COPD patients as a mesure of disease proegression. 

#Data Cleanup & Analysis

Data Sources: 
Air Pollution: https://aqs.epa.gov/aqsweb/airdata/download_files.html

USA Income and Population: https://www.countyhealthrankings.org/explore-health-rankings/rankings-data-documentation/national-data-documentation-2010-2017

Lung Cancer: https://gis.cdc.gov/Cancer/USCS/DataViz.html

Asthma:: https://www.cdc.gov/asthma/brfss/2015/tableL1.html

COPD: https://www.cdc.gov/mmwr/volumes/67/wr/mm6707a1.htm 

Google Places API: https://developers.google.com/maps/documentation/geocoding/start

The main challenge was to find the data,  to clean it, and then reformat it for the analysis. We used census api to get population and income . CeInitially we wanted to analize  disease presentation at the county level. However, findind national data sets for asthma and COPD was challenging and the analisis was done at the state label. 
Once the had the two data sets, per state and per county, the geographical coordinates where added. This two data sets were  used to do statistics and to visualize the  data using Jupyter Gmaps.
We also did a case study analyzig Massachusetts California and Texas.


#Files

The original csv files from our various sources, the Jupyter notebook used to clean the data, and the final cleaned data sets as csv files are in the data_cleanup folder.

The cleaned files are in the Resources folder

County_Analysis.ipynb has the statistical analysis and the heat maps at the countly level

US_Analysis.ipynb has the statistical analysis and the heat maps at the state level

MA_Analysis.ipynb has the statistical analysis and the heat maps of air pollution variables, income and disease for all counties in Massachusets

CA_Analysis.ipynb has the statistical analysis and the heat maps of air pollution variables, income and disease for all counties in California

TX_Analysis.ipynb has the statistical analysis and the heat maps of air pollution variables, income and disease for all counties in Texas

Stater plots and heat maps are in output_plots

#Resuts

Data showed that Asthma prevalence in 2016 had no correlation with any of the parameters associated with air polition. Lung Cancer prevalence showed a weak correlation with AQI (with unhealthy days)And COPD prevalence had no correltion with any of the ar pollution parameter and had a moderate correlation with the percentage of smokers. 
Asthma prevalence is independent of socio-economic status but Lung Cancer and COPD have a moderate correlation.


