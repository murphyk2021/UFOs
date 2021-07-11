# The Truth is Out There
## Module 11: UFO Sightings with JavaScript
---
### Overview
In this module, students continued to practice using Javascript, HTML, and Bootstrap.  

**The task:** to create a webpage which displays a data table of all recorded UFO sightings during the year of 2010.  Since the dataset is rather large, an input field was added to allow the user to filter the data by a specific date.

![image of module created webpage](https://github.com/murphyk2021/UFOs/blob/9ffd9fc2334ce656ff20bfec614e22ed30645f65/static/images/module_webpage.PNG)

---
### Results
**To build our initial table,** we simply loop through the given data array (.js file) and assign one object to each row and one key-value pair to each column. 

![loop to build the table](https://github.com/murphyk2021/UFOs/blob/ef6065b3ad37ddf210370cf38f97340677cfb2e7/static/images/create%20table%20from%20js%20file.png)


**Filtering the data with one criteria,** like the date, is a fairly simple process.  

1.  Tell the code to "listen" for when the user clicks on the "Filter Table" button.  
2.  When the click event occurrs, call the function, "handleClick". 
3.  Retrieve the date typed into the input field (variable "date").  
4.  Examine each row of the date column.  If the input value and the cell value are a match, then the object is included in a new array called "filteredData".  
5.  The data table is then rebuilt using the information in the new array of objects.

![handleclick](https://github.com/murphyk2021/UFOs/blob/fd01eb760ad9ca6a9072fbc4c171bf624a0c8c4a/static/images/simple%20filter2.png)

**Filtering the data with more than one criteria**
![frontend of webpage with multiple search criteria](https://github.com/murphyk2021/UFOs/blob/b78bd7f1b4e6d5955bc1bd81f73a5eb15c8272d9/static/images/challenge_webpage.PNG)

Filtering the data with more than one criteria can be a little more complicated as we must retrieve and save any changes to any of the input fields as an object. Then we will need to loop through our original dataset to locate the objects which match all of the requested criteria and generate a new array which will be used to populate the table.
![code for multiple search criteria](https://github.com/murphyk2021/UFOs/blob/7d70c2c697fa8ae26a55a6c2d79316db4ec40aaa/static/images/code%20for%20multiple%20search%20criteria.png)


---
### Moving Forward
One way we could improve on this web page would be to find another source for ufo sighting reports which is **continously updated with the latest information**(for example, The National UFO Reporting Center).  If we can scrape that data and integrate it into our dataset it would really take our it to the next level!  
![UFO reporting Center HomePage](https://github.com/murphyk2021/UFOs/blob/7875f67ea5ee36f8863f533e7de144b6269ef297/static/images/national%20UFO%20reporting%20center.png)

Another potential opportunity for improving our search is the type of user input fields we are using.  It might be more user friendly to use dropdown menus for the states and/or a date range for the dates (shown below).  This might help the user if they were interested in UFO sighting trends ("Is there a peak Earth tourist season?") or if they were looking for a particular event but could not recall the specific date which it occurred.
![image of date ranges input fields](https://github.com/murphyk2021/UFOs/blob/6779754dc1bb4ff77d6065fa31419353b5729dca/static/images/improvement_1.PNG)

One final improvement which could be made would be to add a Google Earth map that shows where the sighting(s) occured based on the user input criteria!
![map](https://github.com/murphyk2021/UFOs/blob/1711c2b29921d5c78c89b71947f0f4a2b277d4e0/static/images/UFO%20sightings%20in%20texas.PNG)
