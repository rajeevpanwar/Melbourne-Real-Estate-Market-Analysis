<<<<<<< HEAD

## Real Estate Hunting - Down Under by Rajeev Panwar 

# Project Overview & Business Case

Scenario: You are an expat planning to move to Melbourne and need to which region might be a good market to look for housing? Your turn to your friend who is an aspiring data scientist to answer some basic question about the Melbourne real estate market. The friend (i.e. I) decided to answer the following questions:

*  What is a realistic budget range for a particular region?
*  What factors correlate the most with price and could be used to predict future price of housing in Melbourne? Which variables are most likely (distance from downtown, size of dwelling unit, age of property etc.) to influence your choice? 

# Solution Engineering 

My process had 4 parts:
*  use a suitable dataset from Kaggle that covers almost 2 years of pricing data for Melbourne and its surrounding regions (Suburbs that combine to form the Melbourne Metropitian Area so to say) - I used https://www.kaggle.com/anthonypino/melbourne-housing-market 
* Cleaning and analyzing the data
* Identify key features that influence the price of housing in Melbourne 
* Develop Multiple regression models using features to predict price.

# Gathering Data
The dataset that was downloaded from Kaggle includes complete address of property sold, Suburb: Suburb, Rooms: Number of rooms, Price: Price in dollars, Method: Status of property sale, SellerG: Real Estate Agent, Date: Date sold
Distance: Distance from CBD
Regionname: General Region (West, North West, North, North east …etc)
Popertycount: Number of properties that exist in the suburb.
Bedroom2: Number of Bedrooms
Bathroom: Number of Bathrooms
Car: Number of carspots
Landsize: Land Size
YearBuilt: Year the house was built

# Gathering Additional Data 
I imported Australian benchmark bon yeild data for the corresponding period to create a new feature - benchmark_bond_yields in the cleaned up dataframe 

# Cleaning the Data using Pandas
I spent many hours cleaning the data using Pandas Dataframes and Series to prepare it for analysis.  I removed or updated Null values.  The original dataset from Kaggle had more than 34,000 out of which I could only end up using 8700 odd observations as the rest of data has missing values or in-correctly entered values. I also changed the datatypes of many columns so I could make calculations and comparisions acorss columns.

# Analysis using Pandas and Seaborn
I did some 'feature engineering' by adding two new features added - benchmark bond yields and age of property (DateSold - YearBuilt)
We used many DataFrame methods to analyze the data including .describe, .groupby, and .apply. Then I made new dataframes to answer my guiding questions and then visualize the analysis using various Seaborn graphs and charts.

# Findings
Statitical tests used - I used a two Tail T-Test (Independant) to compare the average house prices in the two most popular markets (by sales count) and hoped to run a Welch T test to compare two regions with unequal N (unfortunately my notebook is running too slow to complete this in time right now)


# Findings
 Subject to Welch T-Test 

On best fit model to predict price - 2nd degree Polynomial with all features
# Recommendations

I recommend...
<<<<<<< HEAD
*  
=======
*  
>>>>>>> cb2a9bbbd31b7aa00bf57eb910137378b5867e44
