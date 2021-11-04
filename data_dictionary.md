# Data Dictionary

## Dim States

|Field|Description|
|-----|-----------|
|state_code|3 character code used for I94 ports|
|state_name|U.S. state name of port|

## Dim Countries

|Field|Description|
|-----|-----------|
|country_code|3 character country code|
|country|country name|

## Dim Date

|Field|Description|
|-----|-----------|
|arrdate| The SAS timestamp (days since 1/1/1960)|
|arrival_iso_date| iso date converted from arrdate|
|arrival_year|4 digit year|
|arrival_month|Month (1-12)|
|arrival_day|Day (1-31)|
|arrival_dayofweek|Day of Week (1-7)|

## Dim Demographics

|Field|Description|
|-----|-----------|
|city_code|port code|
|state_code|character code used for I94 ports|
|median_age|The median age for the demographic|
|male_population|Count of male population for city|
|female_population|Count of female population for city|
|total_population|Count of total population for city|
|foreign_born|Count of foreign born persons|
|avg_household_size|Average household size in city|
|native_population|American native population of city|
|asian_population|Asian population of city|
|black_population|Black population of city|
|latino_population|Latino population of city|
|withe_population|Latino population of city|
|city|port name|

## Dim Temperatures

|Field|Description|
|-----|-----------|
|city_code|port code|
|dt|Date in format YYYY-MM-DD|
|temperature|Average temperature in a given city|
|latitude|Latitude|
|longitude|Longitude|
|year|year|
|month|month|
|rank|Rank avg temperature partitioned by city_code|

## Fact Immigration

|Field|Description|
|-----|-----------|
|cicd|Unique identifier per record|
|I94bir|Age of respondent in years|
|I94cit|3 digit code Born Country|
|I94res|3 digit code Residence Country|
|arrdate|Arrival date in sas format|
|depdate|Departure date in sas format|
|dtadfile|Character date field|
|visapost|Department of state where visa was issued|
|occup|Ocupation that will be performed in US|
|entdepa|Arrival flag|
|entdped|Departure flag|
|entdpeu|Update flag|
|matflag|Match flag|
|biryear|Immigrant birth year|
|dtaddto|Character date field when admitted in the US|
|gender|Gender|
|insnum|INS number|
|airline|Airline used to arrive in US|
|admnum|Admission number|
|fltno|Flight number of airline used to arrive in US|
|visatype|Type of visa|
|age|Age of immigrant|
|state_code|character code used for I94 ports|
|city_code|port code|
|visa_mode|Immigrant VISA category|
|visa_category|Immigrant VISA category|