# ETC5521 Assignment 1 

Team name: [rosella]

Team members:

* [Yunzhi Chen]
* [Xianghe XU]

## Introduction
Africa, one of the seven continents, is the world's second-largest, covering approximately 30.3 million square kilometers and constituting 6% of Earth's total surface area. With a population of 1.4 billion, Africa accounts for 18% of the global human population and comprises 54 countries. Despite its vast natural resources, Africa is the least wealthy continent per capita. This analysis delves into specific aspects of the African continent, aiming to explore beyond provided data values and gain a comprehensive understanding of the regions under investigation, drawing conclusions from the analysis.

## Data description
### Source of the data:
The data sets come from two packages which are afrilearndata and afrihealthsites. These two packages are provided by the afrimapr team. The afrimapr team started in 2020 and is funded through the Wellcome Open Research Fund and Wellcome Data for Science and Health, afrimapr team creates R packages and learning resources where it helps public to perform spatial techniques and to make data-driven maps in Africa in an easier way.

### The structure of the data:
*Package: afrilearndata*
The package afrilearndata provides small African spatial data-sets in an aim of helping people to perform spatial techniques and mapping in Africa, and it contains 8 objects (data sets) which are named as africontinent, africountries, afrihighway, africapitals, afriqirports, afripop2020, afripop2000 and afrilandcover, and each of these data sets contains spatial variables (geometry variables are in a type of multipolygon and points) as well as some other variables (character type and numeric type) which make it easier to understand each of object and making maps in Africa.

- The data sets africontinent and africountries are polygons, which contains the geometry variable for continent outline and 51 African country boundaries respective. The object africountries contains not only the geometry variable, and also it contains the names, GDP, population, income level and last census date for each African country.
- afrihighway consists the name and geometry variables for 100 lines of African highway network.
- africapitals has 5 variables which are capital name, country name, population, iso3c (country codes) and geometry point for each country’s capital city in Africa.
- The data set afriairports contains 3348 observations and 22 variables about the airport data in Africa. This data-set contains variables which can categories into the airport name, ID, type, elevation level, continent name, country name, geographic region codes , airport website link, score, last-update date and geometry point of the airport.
- The data set afripop2020 and afripop2000 are in a form of raster grid, which is a kind of data storage format and normally represents geographic data as a matrix of cells that each contains an attribute value. afripop2000 and afripop2020 store the population density from WorldPop aggregated to 20km squares for the years 2000 and 2020 respectively.
- The object afrilandcover is also raster grid, and it contains the data about landcover in 2019, categorical, 20km from MODIS

*Package: afrihealthsites*
The package afrihealthsites provides an access to geographic locations of African health facilities from different sources. This implies that the afrihealthsites package enables people to view the geographic locations of health sites in each African country by choosing different data sources and in various plotting forms. This package contains 5 data sets which are named as afcountries, df_who_sites, sf_healthsites_af, sfssd and who_type_lookup and these data sets contains spatial variables (geometry variables are in a type of points) as well as some other variables (character type and numeric type).

- The data set afcountries has two variables (country name and iso3c country code) and both variables are character type.
- The data set df_who_sites comes from WHO (World Health organisation) and it has 12 variables which are country name, admin, facility name, facility type, ownership, latitude, longitude, iso3c country code, facility type 9, tier and tier name for each of health site in Africa. There appears to be 98745 rows which represents there are 98745 health sites in Africa.
- sf_healthsites_af and sfssd data sets are other sources about data of the health sites in Africa, the data sets has some similar variables compared with df_who_sites such as country name, iso3c country code, types and location for the health sites.
- who_type_lookup contains 3 variables which are country name, type and facility type nice, this data set may be used as type look-up for health site in African countries.

## Questions of interest
- How many observations do data have?
- What is the data type of each feature?
- Do data have null values?
- How much memory does this dataset use? Could this pose a problem for later on?
- What is the distribution of each variable?
- Any values that look like errors?
- Is there any duplicated data?
- Is the null value a result of the way data was recorded?
- Can drop the rows with null values without it significantly affecting analysis?
- Are there so many missing values for a variable that should drop that variable from dataset?
- Are there any variables that represent the same information? Can one be dropped?
- What is the distribution of each type of Healthsite in different parts of Africa?
- What does the change in population in 2000 compared to 20 years later tell us?
- What is the distribution of the airports’ elevation levels?
- Which type of airports is more commonly seen in African countries?
- Does a greater population country have more of airports regardless types of airport, and vice versa?
- What is the distribution of the counts of airport for countries in Africa?
- Which airport obtains the highest score?
- Which elevation level has highest number of airports?
- Are the airports in Africa located in a favor of high elevation level or a low elevation level?
- Are the airports in each country built in similar elevation levels?
- How does the GDP of each African country compare to each other?

## Expected findings
- What is the distribution of each type of Healthsite in different parts of Africa?
The hospital occupies the largest proportion, much higher than the number of Dispensary, followed closely by various health clinics or health centers.

- Does a greater population country have more of airports regardless types of airport, and vice versa?
It depends on the country’s GDP and the degree of national development, a country has a greater size of population should have more airports to meet the travelling needs.

- What is the distribution of the counts of airport for countries in Africa?
The distribution of the counts of airport for each countries should display a bell shape (Normal distribution), which implies some countries has more airports and some has less. Moreover, It seems that South Africa had a large number of airports, making it the leading country in Africa in terms of airport ownership.

- How does the GDP of each African country compare to each other?
The GDP of the each African country should vary from each other, despite of that all the countries are in a same continent, the economic development of each country will be hardly the same. South Africa occupies the top of the list, followed by Egypt.
