# Foreclosures-Analysis-Plotting
In this project, we are using HvPlot (geomaps) to visualize foreclosures in the Los Angeles area!  We read in a CSV file that dsplays information on the foreclosures in the LA area and the lenders that hold the titles to the home.  After extracting the "Lender" data, we use HvPlots to visualize the data.  We visualize the foreclosures by lender,by property type and by council ditsrict. Enjoy!

## Dependencies
import os
import hvplot.pandas
import pandas as pd
from pathlib import Path
