AC 209a, Group 25
Modeling COVID-19 in the US

Nick Normandin, Bliss Perry, 
Sam Thau, and Michael Yin

Hello, thanks for checking out the code for our project! The functionality of each notebook is as follows:

demographic_data.ipynb: Imports, cleans, and conducts EDA on a variety of county characteristic data (mostly demographic)
election_cleaning.ipynb: Imports and cleans 2016 presidential election data by county
restriction_cleaning.ipynb: Imports and cleans metrics for stringency of COVID-related restrictions by state
protest_data.ipynb: Processes raw protest data, resulting in compilation of protests with sizes by FIPS code and date
covid_spread.ipynb: Processes raw COVID case data from JHU, resulting in cases by FIPS code and date, and conducts EDA

combine_data.ipynb: Takes in the data from the above notebooks, and processes and combines them to create the final dataframe for the RNN and treatment effect calculation
rnn_model.ipynb: Sets up, trains, and tests RNN model for predicting COVID cases for a given county and date
similarities.ipynb: Defines several helper functions used by treatment.ipynb, particularly for determining similarities between counties
treatment.ipynb: Calculates the average "treatment effect" of protests for counties that had a protest in the week after George Floyd's death

(outdated) baseline_model.ipynb: Simple linear regression for modelling COVID cases, used in milestone 3
(outdated) milestone3.ipynb: Combines parts of demographic_data, protest_data, covid_spread, and baseline_model for milestone 3