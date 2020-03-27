Business Problem - 

1. You are an expat planning to move to Melbourne and need to which region might be a good market to look for housing? Also you want to understand which factors influence pricing the most so you can 

Hypothesis H1 - The price of houses is correlated with Distance from CBD and landsize.

2. Since you are investing your life savings - you would like to engage a bright data scientist to build a predictive model that can explain which variables are most likely (distance from downtown, size of dwelling unit, affordability etc.) to influence your choice given a budget constraint (real world scenario) 

Solution Engineering - 

DataSet - 
I have used a dataset of Melbourne property sales pertaining to 2016-2018 to identify if there a difference in pricing between the top 3 regions(geographic sub-markets) - 

Additionally I have combined Australian Benchmark 10-year bond yields from https://fred.stlouisfed.org/series/IRLTLT01AUM156N to help explain pricing.

Key Variables Considered  - 



Key Findings - 

Problem 1. 

Problem 2. 

The dataset includes Address, Type of Real estate, Suburb, Method of Selling, Rooms, Price, Real Estate Agent, Date of Sale and distance from C.B.D.

3.2 Data
The data was scraped from publicly available results posted every week from Domain.com.au. The variables used in our analysis are as follows:

Suburb: Suburb

Rooms: Number of rooms

Price: Price in dollars

Method: Status of property sale -

S - property sold; 
SP - property sold prior; 
PI - property passed in; 
PN - sold prior not disclosed; 
SN - sold not disclosed; 
VB - vendor bid; 
W -  withdrawn prior to auction; 
SA - sold after auction; 
SS - sold after auction price not disclosed.
Type: Type of house -

h - house,cottage,villa, semi,terrace; 
u - unit, duplex; 
t - townhouse;
SellerG: Real Estate Agent

Date: Date sold

Distance: Distance from CBD

Regionname: General Region (West, North West, North, North east …etc)

Propertycount: Number of properties that exist in the suburb.

Bedroom2: Number of Bedrooms

Bathroom: Number of Bathrooms

Car: Number of carspots

Landsize: Land Size

YearBuilt: Year the house was built


Feature engineering done - two new features added - benchmark bond yields and age of property 