# Rental-Analysis-Plotting
In this project, we are using HvPlot (geomaps) to visualize Rental Properties in the Los Angeles area!  We read in multiple CSV files that contain information on the Rentals and the lenders that hold the titles to the home.  After extracting the "Lender" data, we use HvPlots to visualize the data.  We are able to search the properties by lender,by property type and by council ditsrict. Enjoy!



Filter out the “housing_units” column to create a DataFrame that includes only the sale_price_sqr_foot and gross_rent averages per year.
For this part of the assignment, use interactive visualizations and widgets to explore the average sale price per square foot by neighborhood. 
Using the original sfo_data_df Dataframe, create a DataFrame named all_neighborhood_info_df that groups the data by neighborhood. Aggregate the results by the mean of the group.
Review the two code cells that concatenate the neighborhood_locations_df DataFrame with the all_neighborhood_info_df DataFrame

## Dependencies
import os
import hvplot.pandas
import pandas as pd
from pathlib import Path

Question: How does the trend in rental income growth compare to the trend in sales prices? Does this same trend hold true for all the neighborhoods across San Francisco?

Answer: For almost all of the San Francisco neighborhoods included in the data, the increase in gross rent well-outpaced the increases in average sale price per square foot over the period. In neighborhoods like Anza Vista, where the sale price per square foot declined, the gross rent increased substantially. However, in some neighborhoods, like the Union Square District, recent increases in the sale price per square foot are starting to exceed the increase in gross rent.

Question: What insights can you share with your company about the potential one-click, buy-and-rent strategy that they're pursuing? Do neighborhoods exist that you would suggest for investment, and why?

Answer: The company should be selective in choosing a neighborhood in which to implement its one-click, buy-and-rent strategy. It should avoid neighborhoods like the Union Square District, where the cost to buy the property is increasing relative to the rental income. The company should focus on neighborhoods where the cost to purchase the property has held steady, but the gross rent numbers continue to increase. These are neighborhoods like Bayview, Central Sunset, and Inner Mission.

Question: Which neighborhood has the highest gross rent, and which has the highest sale price per square foot?

Answer: Based on the size of the circles, Union Square has the highest sale price per square foot at 903.99. The highest gross rent figure, as defined by its yellow circle, is Westwood Park at 3959.


Use the san_francisco_housing.ipynb notebook to visualize and analyze the real-estate data.

Note that this assignment requires you to create a visualization by using hvPlot and GeoViews. Additionally, you need to read the sfo_neighborhoods_census_data.csv file from the Resources folder into the notebook and create the DataFrame that you’ll use in the analysis.
