DataBase:
column names:   name	    continent   area    population  gdp
rows:           Afghanistan	Asia	    652230  25500100    20343000000
                Albania	    Europe	    28748   2831741	    12960000000
                Algeria	    Africa	    2381741 37100000	188681000000
                Andorra	    Europe	    468	    78115	    3712000000
                Angola	    Africa	    1246700 20609294	100990000000


1. The example uses a WHERE clause to show the population of 'France'. Note that strings (pieces of text that are data) should be in 'single quotes';

Example:
SELECT population FROM world
    WHERE name = 'Germany'

Returns:
population
80716000


2. Checking a list The word IN allows us to check if an item is in a list. The example shows the name and population for the countries 'Brazil', 'Russia', 'India' and 'China'.

Example:
SELECT name, population FROM world
    WHERE name IN ('Brazil', 'Russia', 'India', 'China');

Returns:
name	population
Brazil	202794000
China	1365370000
India	1246160000
Russia	146000000

Example:
SELECT name, population FROM world
    WHERE name IN ('Sweden', 'Norway', 'Denmark');

Returns:
name	population
Denmark	5634437
Norway	5124383
Sweden	9675885


3. Which countries are not too small and not too big? BETWEEN allows range checking (range specified is *inclusive* of boundary values). The example below shows countries with an area of 250,000-300,000 sq. km. Modify it to show the country and the area for countries with an area between 200,000 and 250,000.

Example:
SELECT name, area FROM world
    WHERE population BETWEEN 250000 AND 300000

Returns:
name	        area
Burkina Faso	272967
Ecuador	        276841
Gabon	        267668
New Zealand	    270467

Example:
SELECT name, area FROM world
    WHERE population BETWEEN 250000 AND 300000

Returns:
name	        area
Belarus	        207600
Ghana	        238533
Guinea	        245857
Guyana	        214969
Laos	        236800
Romania	        238391
Uganda	        241550
United Kingdom	242900
