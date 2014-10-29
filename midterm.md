### Query the database and create a list of every county (with state) that has acquired at least one mine-resistant armored vehicle. Then map that list
I first used SQLite to get the list of all the counties that possessed at least one Mine Resistant Vehicle. I realized that the MRV were entered into the data as both 'Mine Resistant Vehicles' and 'Mine Resistant Vehi', so I had to account for both those listings
![Imgur](http://i.imgur.com/Pw419O1.png)
I then produced a [Google Fusion Heat Map](https://www.google.com/fusiontables/DataSource?docid=1Mw31BUJnLUbfHhMwE_QyRUDFDk3QpQ7xOwn6D4c5#map:id=3) that mapped the counties that had the MRVs

### Query the database and find the most expensive single item that can be acquired through the 1033 program. Then generate a list of all counties that has so far acquired at least one of these things
The single most expensive item is listed as 'Aircraft, rotary wing' and each one costs 18000000. Apparently, Florida is the only state that has them, in Brevard county.
![Imgur](http://i.imgur.com/BTd5Suk.png)

### Query the database to get the top 10 counties ordered by the total number of guns acquired through the 1033 program. Your answer should look very similar to what NPR found under the Total Guns Acquired graph (e.g. 3,452 guns for Los Angeles)

### Query the database to get the top 10 counties ordered by number of guns acquired per 1,000 people using the Census's 2013 population estimate. Again, your answers should look similar (but not exact) to what NPR found, e.g. 28 guns/1,000 people in Franklin, KY.

### Create a time-series/histogram showing something you find interesting in the 1033 Program data. Examples: Number of gas masks versus night-goggles distributed by year. Monetary value of pants and trousers versus rifles, by year.

### Find all of the counties that have not acquired a single thing in the leso table, and then map those counties.

### Find the county that has acquired the most from the 1033 Program in terms of total acquisition cost and generate a list of the items that county has acquired.

### Write a 300-word story memo on an interesting query (or queries) of your own. The memo should include examples/results of a data query and why you think said results are newsworthy or worth further investigation. Your memo, ideally, would involve some additional research to see if anyone else has found anything related to your inquiry. A chart/graphic is optional.
