# EDA OF AnnualCO2Emmision
- Our data set has four columns; Entity, Code,Year and annual CO2 emmisions and it contains records from the year 1750 to 2023.
- The emmision value has been given in tonnes hence we renamed the column indicating the units. 
- From our exploration, we realise that dropping null values will cost us to lost annual CO2 records of some entities. In the real world some of these entities donot actually have codes but to preserve our information we cleaned the missing values by assigning codes to entities with no codes. 
- After doing this every unique entity had a unique code. 
## Classification Of Entities
- we observed also that each entities was either a continent, belong to a continent, is a regional groupings, territory, Income classification and some fall under special events. We Classified these entities under the categories( Continents( Asia, AFrica,Europe, North America,South America, Oceania,Antarctica), continents itself for entities that are continents, Territories etc.
- We created a new column for this classification named "Region" and created a new Csv File(classified_countries) having five columns( entity, code, year, Annual CO2 emmission(tonnes)) and Region).
## Data Visualization
- We got the following insights from some of our visualization;
- Asia was the continent with the highest CO2 emmission in the year 2023.
- There has been a slight change in the annual emmission of CO2 in Cameroon from the year 2020 t0 2023.
  ## Reducing bias
  - The number of years for which CO2 was emmited for each entity is not uniform that is not thesame. This issue will cause bias in our analysis and visualization. We solved this issue by applying the set method on the year of each unique entity and getting their intersection. The intersection gave us yeats from 1994 to 2023. We went futher to create a new csv file that contains just the intersection of the years and futher repeated some visualizations which gave us better results.
