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

In this project, bubble maps were also created, displaying a somewhat of a negative correlation between percentage of population over 60 and percentage of population under 18. Since COVID-19 is most deadly in the middle-aged to elderly age groups, for the counties that have a large population of citizens under age 18, those counties may not need to follow as closely to very strict social distancing guidelines (complete shutdown of all businesses, etc.). However, these counties also need to take into account the percentage of their other age groups, given that children/teens/young adults are often vectors of disease. If there are any counties with a high percentage of under 18ers and a relatively lower percentage of 60+ers, if the county sees promising results (not too many deaths, etc.), perhaps these counties can provide resources to counties like Sumter County, for example.


![CorrelationHeatMap.PNG](https://github.com/drewshlee/Analyzing-County-Data-to-Determine-Level-of-Adherence-to-COVID-19-Guidelines/blob/master/CorrelationHeatMap.PNG)

Lastly, a heat map was created to determine correlations among various factors, including cases, hospitals, hospital bed counts, deaths, etc. As noted in the gitbook tutorial, the "number of hospital beds per 1,000 people almost has a 0 correlation with both the number of COVID-19 cases or deaths per 1,000 people. We might assume that more hospital beds per capita would correlate negatively with the number of deaths (if more people are able to get more individualized care), but this suggests that there are some other factors (potentially population density, social mobility, number of airports or estimated daily travelers/tourists, number of restaurants or tourist attractions, weather, etc)." There's a lot more depth to the COVID-19 pandemic than we think, and sometimes that assumptions that we make, such as the correlation between hospitals beds per 1000 people and number of COVID-19 cases/deaths per 1,000 people, can be misguided. 

Another interesting insight to this correlation heat map is the correlation between cases and hospital count. Hospitals seem like such an easy way for COVID-19 to proliferate, stemming from the lack of PPE, to being in such a dense environment where patient and doctor interaction is necessary. This kind of data should be used to convince federal and state governments that PPE is an absolute necessity, to protect the doctors and nurses that are putting their lives on the line to treat COVID-19 patients. 


# Business Answer Interpretation
From our county level data analyses, it is clear that counties will have different needs and different experiences in light of the COVID-19 pandemic. Additionally, social distancing guidelines, and reopening phases + measures, will differ based on metrics like total population size and percentage of elderly/60+. From our bar graphs analyses, we can conclude that Sumter County is at major risk, given their >60% elderly population. It is likely to be composed of retirement communities, but at the same time, it is likely a community that is, on average, wealthier than other communities, with greater access to healthcare. Meanwhile, in the other side of the country, in Los Angeles county, residents need to be aware of the sheer size of the county (~10 million), and the drawbacks of such a population size. Although further analyses into traffic data and population density are required to make a conclusive insight into Los Angeles County's COVID-19 future, population size alone is a good metric of study in light of COVID-19's relatively high R0 value. Thus, with that being said, Sumter County and Los Angeles County, at least according to this analysis, are two of the highest at-risk counties during this COVID-19 pandemic.

Further analyses regarding county specific data can include an analysis of the number of hospitals by county. Yes, we can generally presume that a greater number of hospitals means more access to care during this COVID-19 pandemic, but it is also a possibility that a greater number of hospitals increases the number of COVID-19 cases in the area. Health professionals continue to lack PPE that adequately protects them during patient treatment/care, and given the ungodly amount of stress these healthcare professionals are facing, they are at risk of becoming vectors of disease. 
