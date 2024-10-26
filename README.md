# trial-1
City Population Analysis
Project Description
This project involves analyzing and predicting population trends in major cities using the "City Population Annual Timeseries" dataset from the UN Statistics Division. The goal is to explore historical population data, conduct data cleaning and preprocessing, and apply various machine learning models to predict city populations, providing insights into population distribution across different regions and city types.
Dataset Description
The dataset includes annual population estimates for cities worldwide. Key columns contain city names, country names, city types, and population counts by year. Data spans multiple decades, offering a view of urban population changes over time.
Summary of Findings
Our analysis identified trends in population growth by city type, country, and sex, and highlighted the cities and countries with the largest populations. The models applied to the top 100 most populated cities produced insights into the predictive power of different algorithms.
Data Preprocessing
Data preprocessing steps included:
Column Removal: Dropped irrelevant columns such as 'Value Footnotes,' 'Reliability,' 'Record Type,' and 'Source Year.'
Handling Missing Values: Removed rows with missing values.
Renaming Columns: Standardized column headers (e.g., Country_or_Area, City_Type) and ensured consistent casing in string columns.
Cleaning Country and City Names: Removed parentheses, standardized special characters (e.g., replacing Å with A), and cleaned extraneous text.
Population Data Conversion: Converted population values from strings to integers, removing decimals.
Filtered for Analysis: Limited data to records from 1972 to 2014 to focus on a manageable timeframe for analysis.
Exploratory Data Analysis (EDA)
Population Trend from 1972 to 2014
The line plot displays the total population trend over the years 1972–2014, highlighting overall growth patterns.
 
Number of Cities by City Type
This bar plot shows the distribution of city types, with corresponding city counts for each type.
 

Total Population by Sex

This bar plot aggregates population data by sex, illustrating population distribution within the dataset.
 
 
Top 20 Countries by Population
This plot ranks the top 20 countries by total population, emphasizing countries with significant urban populations.
 
Top 25 Cities by Population
The plot showcases the top 25 cities by total population, underscoring highly populated urban areas.
 
Model Development
We focused on predicting the population for the top 100 cities using features such as city type, year, country, and city name. Categorical variables were one-hot encoded. The dataset was split into training and testing sets to evaluate model performance effectively. Four machine learning models were selected:
Linear Regression
Random Forest Regressor
Decision Tree Regressor
XGBoost Regressor
Model Evaluation
Each model was evaluated based on:
Mean Absolute Error (MAE %): Calculated as a percentage of the mean population in the test set.
R² Score (%): Expressed as a percentage.
Accuracy (%): 100% - MAE percentage.
Model	Mean Absolute Error	R2 Score	Accuracy
Linear Regression	19.018988      	83.203616     	80.981012
Random Forest Regressor	9.570583      	95.613502     	90.429417
Decision Tree Regressor	7.833003      	98.541664     	92.166997
XGBoost Regressor	9.141363      	98.132145     	90.858637

Conclusion
The analysis successfully identified trends in city populations and evaluated several regression models. The Decision Tree Regressor demonstrated the best performance, making it a reliable model for predicting city populations based on available features.
Contributors
[Your Name]

