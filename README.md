# The Truth is Out There
## Module 11: UFO Sightings with JavaScript
---
### Overview
In this module, students continued to practice using Javascript, HTML, and Bootstrap to create a webpage which displays a data table of all recorded UFO sightings during the year of 2010.  Since the dataset is rather large, an input field was added to allow the user to filter the data by a specific date.
![image of module created webpage](https://github.com/murphyk2021/UFOs/blob/9ffd9fc2334ce656ff20bfec614e22ed30645f65/static/images/module_webpage.PNG)

---
### Results
To build our initial table, we simply loop through the data array and assign one object to each row and one key-value pair to each column. 
![loop to build the table](https://github.com/murphyk2021/UFOs/blob/ef6065b3ad37ddf210370cf38f97340677cfb2e7/static/images/create%20table%20from%20js%20file.png)

Filtering the data with one criteria, like the date, is a fairly simple process.  First we created an event to "listen" for when the user clicked on the "Filter Table" button.  This would then activate a function (handleClick) which retrieved the information typed into the input field.  Then, each row of the date column was examined.  If the input value and the cell value were a match, then the object became part of a new array called "filteredData".  We then rebuilt the table from this new array of objects.
![handleclick](https://github.com/murphyk2021/UFOs/blob/2536d2f14f6ed3aef448312814853b10d5ccf43e/static/images/simple%20filter2.png)

Filtering the data with more than one criteria can be a little more complicated as we must retrieve the information from each input field and loop through our dataset to locate the objects which matched all of the criteria.


---
### Moving Forward
One way we could improve on this web page would be to find another source for our ufo sightings which is continously updated with the latest information(for example, The National UFO Reporting Center).  If we could scrape that data and integrate it into our dataset it would really take our dataset to the next level!  
![UFO reporting Center HomePage](https://github.com/murphyk2021/UFOs/blob/7875f67ea5ee36f8863f533e7de144b6269ef297/static/images/national%20UFO%20reporting%20center.png)

Another potential opportunity for improving our search is the type of user input fields we are using.  It might be more user friendly to use dropdown menus for the states and/or a date range for the dates (shown below).
![image of date ranges input fields](https://github.com/murphyk2021/UFOs/blob/6779754dc1bb4ff77d6065fa31419353b5729dca/static/images/improvement_1.PNG)

One final improvement which could be made would be to add a map that shows where the sighting(s) occured  based on the user criteria - Zillow-style!
