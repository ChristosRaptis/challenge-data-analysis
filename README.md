# challenge-data-analysis
Take the dataset collected in the previous project (challenge-collecting-data) and perform data analysis on it.

Perform data cleaning and identify/analyze inputs correlated to property price in Belgium. 


## Installation
- pandas
- numpy
- Matplotlib
- Seaborn
- Scipy

## Usage
Environment: Jupiter Notebook (python 3.11).

All code and analysis inside data-analyssi-immo_eliza.ipynb

## Procedure

### Dataset cleaning
- Removed variables with very high percentage of empty values.
- Removes rows with empty values.
- Stripped spaces from string values.
- Stripped letters from postal code variable.
- Removed postal codes with more than 4 digits (not belonging to Belgium).
- Removed duplicate values.

### Data Analysis
- Calculated correlation between property price and the other varaiables.
- Removed "type_of_sale" and "has_open_fire" variables due to negative correlation with price.
- Plotted correlation between price and other variables.
- Plotted correlation heatmap to display correlations between all variables.

### Data Interpretation
- Plotted the outliers with both a scatter plot and a boxplot.
- Filtered and removed outliers using the IQR method.
- Removed some outlier values on the lower end of price and habitable surface which were missed by the IQR method.
- Plotted a histogram of number of properties over surface.
- Plotted mean, median and price per square meter for Belgium, Flanders, Wallonia and Brussels.

### Conclusions
From our undserstanding of tha analysis, we surmised that the variables that affect property price the most are:
- Habitable surface
- Number of rooms
- Presence of swimming pool
- Presence of terrace
- Presence of garden

We also noted that the Brussels region, although very small in comparison to the other two regions, has a sizeble share 
of the real estate market.



![download](https://github.com/ChristosRaptis/challenge-data-analysis/assets/18227773/6f455519-f5cf-4c44-9f9c-16fd3afb8735)
