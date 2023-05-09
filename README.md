# sraping-challenge
Module 11 challenge

# Background
You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

As you work on this Challenge, remember that you’re strengthening the same core skills that you’ve been developing until now: collecting data, organizing and storing data, analyzing data, and then visually communicating your insights.

# What You're Creating
This new assignment consists of two technical products. You will submit the following deliverables:

Deliverable 1: Scrape titles and preview text from Mars news articles.

Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

## Part 1: Scrape Titles and Preview Text from Mars News
For the first deliverable, I imported Splinter and BeautifulSoup in order to parse through the html webpage. 

I extracted all of the text elements on the page and stored them into an empty python list called 'mars'.

Using a for loop, I looped through the text elements in order to extract the content_title and article_teaser_body, which I labeled 'title' and 'preview' respectively into a dictionary called 'mars_dict'. The 'mars_dict' was appended to the empty mars list I created. I lastly printed the mars list to confirm the extraction success.

I saved the first deliverable notebook as "part_1_mars_news.ipynb" which is located in the "Starter_Code folder. 

## Part 2: Scrape and Analyze Mars Weather Data
For the second deliverable, I again imported Splinter and BeautifulSoup in order to parse through the html webpage but also matplotlib and pandas to perform analysis on the mars weather data.

I started off by scarping/finding the table that I would be extracting the row data from. I then extracted all the rows of data from that table.

Next I created two empty lists to store the data in. 

- The first list was called 'temp_header'. I used a for loop to append the header columns.
- The seceond list was called 'temp_data. I used a nested for loop to find a  data row and then created another empty list called 'data_list' and appended the individual data values to it. The data_list was then appended to the initial temp_data list.

The temp_data and temp_header was the turned into a Pandas Dataframes with the temp_data as the list of rows and temp_header as the list of column names.

After the dataframe was created I conducted the analysis on the mars weather data.
Analysis was conducted based on the following questions:
- How many months exist on Mars?
- How many Martian (and not Earth) days worth of data exist in the scraped dataset?
- What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
  - Find the average the minimum daily temperature for all of the months. 
  - Plot the results as a bar chart.
  - ![Average min temp](https://github.com/kirbyjudd/sraping-challenge/blob/main/Starter_Code/Graphs/Ordered_Temperature_Bar.png?raw=true)
- Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
  - Find the average the daily atmospheric pressure of all the months.
  -  Plot the results as a bar chart.
  -  ![Average atmospheric pressure](https://github.com/kirbyjudd/sraping-challenge/blob/main/Starter_Code/Graphs/Ordered_Pressure_Bar.png?raw=true)
- About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
  - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
  - Visually estimate the result by plotting the daily minimum temperature.
  - ![Number of terrestrial days](https://github.com/kirbyjudd/sraping-challenge/blob/main/Starter_Code/Graphs/Terrestial_Days_graph.png?raw=true)

I exported the final dataframe to the "Output" folder and called it "mars_temp_data.csv"

The graphs to the main questions can be found in the "Graphs" folder.

### Peer Cooperation
I worked together on this assignment with my classmate Riddhi Sodagar.






