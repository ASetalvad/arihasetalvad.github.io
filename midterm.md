### 1. Query the database and create a list of every county (with state) that has acquired at least one mine-resistant armored vehicle. Then map that list
I first used SQLite to get the list of all the counties that possessed at least one Mine Resistant Vehicle. I realized that the MRV were entered into the data as both 'Mine Resistant Vehicles' and 'Mine Resistant Vehi', so I had to account for both those listings
![Imgur](http://i.imgur.com/93maBKW.png)
I then produced a [Google Fusion Heat Map](https://www.google.com/fusiontables/DataSource?docid=1dR5unVhqwWP-f5K_Ec4lBKYy4sIP0uQAbs_A-HuU) that mapped the counties that had the MRVs

### 2. Query the database and find the most expensive single item that can be acquired through the 1033 program. Then generate a list of all counties that has so far acquired at least one of these things
I first ran a query to find what the single most expensive item listed in the data was. Turns out it was 'Aircraft, rotary wing' and each one costs 18000000.
![Imgur](http://i.imgur.com/d53b8JX.png)
I then ran a query to get the list of all the counties that has at least one Aircraft, rotary wing. There were multiple counties that possessed at least one of these items, but not all counties paid the same price for their Aircraft Rotary Wing (i.e.- they didn't all pay 18000000)
![Imgur](http://i.imgur.com/aECVn0B.png)
And then added the total number of these items that each county has, grouped by county
![Imgur](http://i.imgur.com/FJmw0vp.png)

### 3. Query the database to get the top 10 counties ordered by the total number of guns acquired through the 1033 program. Your answer should look very similar to what NPR found under the Total Guns Acquired graph (e.g. 3,452 guns for Los Angeles)
I first ran a query to find all the items that contained the words gun, rifle or pistol, since those were the words I noticed in the raw data. I then created a column of the totals of those items and grouped them by county, then limited the results to just include the top ten.
![Imgur](http://i.imgur.com/68ef3Z1.png)

### 4. Query the database to get the top 10 counties ordered by number of guns acquired per 1,000 people using the Census's 2013 population estimate. Again, your answers should look similar (but not exact) to what NPR found, e.g. 28 guns/1,000 people in Franklin, KY.
![Imgur](http://i.imgur.com/szICIP5.png)


### 5. Create a time-series/histogram showing something you find interesting in the 1033 Program data. Examples: Number of gas masks versus night-goggles distributed by year. Monetary value of pants and trousers versus rifles, by year.
I used a query similar to the one I used to find the guns per 1000 people to find total guns by the female population in 2013 in each county
![Imgur](http://i.imgur.com/TJtNKKZ.png)
I then exported that data into Google spreadsheets and used it to create a [bar chart](https://docs.google.com/spreadsheets/d/1kK6th-fSlkSTBxxrWVN16FcEn_9RBO6eGIHAmsJiwww/edit?usp=sharing) that depicts the number of guns per female population, sorted by county. 

### 6. Find all of the counties that have not acquired a single thing in the leso table, and then map those counties.
Assuming that all the counties listed in leso received something from the 1033 program, I ran a query to find the list of counties that were listed in county_ansi but not in leso
![Imgur](http://i.imgur.com/8eTmxud.png)
I used that list to create [this map](https://www.google.com/fusiontables/data?docid=1jW7gNmjmj5s2sckSBNvwLw1Wxc9vWT12a6a6KL5t#map:id=3) with Fusion Tables

### 7. Find the county that has acquired the most from the 1033 Program in terms of total acquisition cost and generate a list of the items that county has acquired.
I first ran a query to find the single county that has received the most from the 1033 program, and found that it was Brevard country in Florida.
![Imgur](http://i.imgur.com/Xc7RnYU.png)
I then ran a second query to get the list of all the items that Brevard county has received.
![Imgur](http://i.imgur.com/W52TAq4.png)

### 8. Write a 300-word story memo on an interesting query (or queries) of your own. The memo should include examples/results of a data query and why you think said results are newsworthy or worth further investigation. Your memo, ideally, would involve some additional research to see if anyone else has found anything related to your inquiry. A chart/graphic is optional.
