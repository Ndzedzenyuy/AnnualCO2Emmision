# EDA OF AnnualCO2Emmision
Our data set has four columns; Entity, Code,Year and annual CO2 emmisions and it contains records from the year 1750 to 2023.
The emmision value has been given in tonnes hence we renamed the column indicating the units
From our exploration, we realise that dropping null values will cost us to lost annual CO2 records of some entities. To preserve this information we cleaned the missing values by assigning codes to entities with no codes. In the real world some of these entities donot have codes. 
After doing every unique entity had a unique code. 
## Classification Of Entities
we observed also that each of entities was either a continent, belong to a continent, is a regional groupings, territory, Income classification and some fall under special events. We Classified these entities under the categories( Continents( Asia, AFrica,Europe, North America,South America, Oceania,Antarctica), continents itseld for entities that are continents, Territories etc.
We created a new column for this classification named "Region" and created a new Csv File having five columns( entity, code, year, Annual CO2 emmission(tonnes)) and Region).
## Data Visualization
We got the following insights from some of our visualization
Asia was the continent with the highest CO2 emmission in the year 2023.
