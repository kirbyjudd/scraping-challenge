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
For part 1 I imported Splinter and BeautifulSoup in order to parse through the html webpage. I extracted all of the text elements on the page and stored them into an empty python list called "mars".

Using a for loop, I looped through the text elements in order to extract the content_title and article_teaser_body, which I labeled 'title' and 'preview' respectively into a dictionary called 'mars_dict. The mars_dict was appended to the empty mars list I created. I then printed the mars list to confirm the extraction success.
