# Based on County-level Analysis, Which Counties Need to Adhere More Closely to Strict Social Distancing Measures and Guidelines?
As economies and populations continue to weather the harsh realities of the COVID-19 pandemic, certain sacrifices may need to be made. For counties that have a smaller age 60+ population, relatively small population, and manageable hospital bed count, social distanding guidelines may not need to be as strict as in counties that have a high 60+ age population and low hospital bed count. Analyses into this county level data can provide guidelines for social distancing measures, business reopening plans, and more.

# Business Question
How can analyses into county level data (percentage of population over 60, percentage of population under 18, number of hospital beds, hospital count, etc.) help manage the COVID-19 crisis?


# Data Question
We will be using data from the following sources:

- [Johns Hopkins University Center for Systems Science and Engineering](https://github.com/CSSEGISandData/COVID-19)
- [New York Times](https://github.com/nytimes/covid-19-data)
- [American Community Survey](https://data.census.gov/cedsci/table?q=United%20States&g=0100000US.050000&tid=ACSST5Y2018.S0101&hidePreview=false&vintage=2018&layer=VT_2018_050_00_PY_D1&cid=DP05_0001E&t=Populations%20and%20People)
- [U.S. Census](https://www.census.gov/geographies/reference-files/2018/demo/popest/2018-fips.html)
- [Homeland Infrastructure Foundation-Level](https://hifld-geoplatform.opendata.arcgis.com/datasets/hospitals)


# Data Answer/Analysis

![TotalPopulationCounty](https://github.com/drewshlee/Analyzing-County-Data-to-Determine-Level-of-Adherence-to-COVID-19-Guidelines/blob/master/TotalPopulationCounty.PNG)

Based on a preliminary analysis, given COVID-19's median R0 value of around 5.7, Los Angeles County should strictly reinforce social distancing guidelines. Without taking bed/hospital count and percentage of residents over 60 or under 18 into account, by sheer numbers, Los Angeles County outranks the 2nd and 3 largest counties by quite a bit. With a median R0 value around 5.7, just by population numbers alone, Los Angeles County is at risk (which, since this project was due, we have seen that Los Angeles County managed pretty well despite such a large population. Smart social distancing guidelines and adherence to those guidelines worked well). 


![Over60HighestCounty](https://github.com/drewshlee/Analyzing-County-Data-to-Determine-Level-of-Adherence-to-COVID-19-Guidelines/blob/master/Over60HighestCounty.PNG)

Aside from the code provided in this tutorial, I also specifically looked at the counties with the highest percentage of individuals over 60 (using a bar graph, easier to visualize than bubble map). We have seen thus far that COVID-19 is particularly dangerous in populatuons 60 and up; After a graphical analysis of the county data, Sumter County in Florida, boasting an over 60% 60+ age group, is at a major risk. With such a large elderly population that makes up the county's inhabitants, Sumter county needs to understand that a majority of its population is at risk of death. Not to mention, with such a large elderly population, if they contract COVID-19, then hospitals would be overwhelmed with large amounts of elderly who may need ventilators that put stress on hospitals' resources. This data helps us better understand that Sumter County is at risk for an increased number of COVID-19 cases + deaths.

![Under18Over60UsCountiesGraph.PNG](https://github.com/drewshlee/Analyzing-County-Data-to-Determine-Level-of-Adherence-to-COVID-19-Guidelines/blob/master/Under18Over60UsCountiesGraph.PNG)

![PercentageUnder18Over60Counties.PNG](https://github.com/drewshlee/Analyzing-County-Data-to-Determine-Level-of-Adherence-to-COVID-19-Guidelines/blob/master/PercentageUnder18Over60Counties.PNG)


