# Web_Scraping_Challenge
Mission to Mars

This challenge is to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup from Mars news and weather data websites.

This new assignment consists of two technical products:
1)  Scrape titles and preview text from Mars news articles. Optionally export the data into a JSON file or a MongoDB database.
2)  Scrape and analyze Mars weather data, which exists in a table.

## Deliverable 1: Scrape Titles and Preview Text from Mars News
The following steps were followed to scrape the Mars News website:
1)  Use automated browsing to visit the Mars NASA news site (https://redplanetscience.com/). Inspect the page to identify which elements to scrape.
2)  Create a Beautiful Soup object and use it to extract text elements from the website.
3)  Extract the titles and preview text of the news articles that were scraped. Store the scraping results in Python data structures as follows:
    -   Store each title-and-preview pair in a Python dictionary. And, give each dictionary two keys: title and preview.
    -   Store all the dictionaries in a Python list.
    -   Print the list in the jupyter notebook.
4)  Optionally, store the scraped data in a file or database (to ease sharing the data with others). To do so, export the scraped data to either a JSON file or a MongoDB database.

## Deliverable 2: Scrape and Analyze Mars Weather Data
The following steps were followed to scrape and analyze Mars weather data:
1)  Use automated browsing to visit the Mars Temperature Data Site (https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html). Inspect the page to identify which elements to scrape.
2)  Create a Beautiful Soup object and use it to scrape the data in the HTML table. 
3)  Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website.
4)  Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
5)  Analyze the dataset by using Pandas functions to answer the following questions:
    -   How many months exist on Mars?
    -   How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    -   What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
        -   Find the average the minimum daily temperature for all of the months.
        -   Plot the results as a bar chart.
    -   Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
        -   Find the average the daily atmospheric pressure of all the months.
        -   Plot the results as a bar chart.
    -   About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
        -   Consider how many days elapse on Earth in the time that Mars circles the Sun once.
        -   Visually estimate the result by plotting the daily minimum temperature.
6)  Export the DataFrame to a CSV file.

## Files Uploaded
-   **Deliverable 1 jupyter notebook**: part_1_mars_news.ipynb
-   **Deliverable 2 jupyter notebook**: part_2_mars_weather.ipynb
-   **Output JSON and CSV files**: output_files/