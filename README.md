# ETL Project

## Extract: 

For this project, we used data from the OECD (education statistics) and the World Bank (select economic indicators) for the same set of countries. We extracted data for both from csv files downloaded from their respective websites. 

## Transform: 

Two of us worked on transforming the OECD data, and the other two worked on transforming the World Bank data. We performed those transformations in two separate jupyter notebooks but later combined them in the file named ETL_Project_Combined. We focused specifically on the year 2012 (the last year certain education data was available) for both data sets and arranged the data in two dataframes showing the selected stats (columns) by country (rows). 

The process for creating these dataframes was a bit cumbersome. The variables we used as column heads in our tables were originally rows in the csv files, so much of the transformation involved converting those row entries to column headings one at a time and then combining them into one dataframe. Both pairs took a different approach to this, which you'll see in the combined file (we suspect there's a more efficient way than the ones we stumbled on).  

## Load:

We loaded these two dataframes as two tables -- called oecd_education_data and world_bank_data -- into a SQL database (also shown in the combined jupyter notebook. 
