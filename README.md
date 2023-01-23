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
    
        ![image](https://user-images.githubusercontent.com/111614210/213948615-ad1cc3b3-abde-4617-ac71-d4833c1a02a1.png)

4)  Optionally, store the scraped data in a file or database (to ease sharing the data with others). To do so, export the scraped data to either a JSON file or a MongoDB database.

## Deliverable 2: Scrape and Analyze Mars Weather Data
The following steps were followed to scrape and analyze Mars weather data:
1)  Use automated browsing to visit the Mars Temperature Data Site (https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html). Inspect the page to identify which elements to scrape.
2)  Create a Beautiful Soup object and use it to scrape the data in the HTML table. 
3)  Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website.
4)  Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
5)  Analyze the dataset by using Pandas functions to answer the following questions:
    -   How many months exist on Mars?
        
        ![image](https://user-images.githubusercontent.com/111614210/213948726-1f997668-9f27-464e-a016-cb700d068666.png)

    -   How many Martian (and not Earth) days worth of data exist in the scraped dataset?
        
        ![image](https://user-images.githubusercontent.com/111614210/213948750-856498aa-97e6-403c-9d4d-34697e8040bb.png)

    -   What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
        -   Find the average the minimum daily temperature for all of the months.
        
            ![image](https://user-images.githubusercontent.com/111614210/213948770-73ca6846-c13e-4b10-94db-444945a9326a.png)

        -   Plot the results as a bar chart.
            
            ![image](https://user-images.githubusercontent.com/111614210/213948812-095818d6-2dd6-41a4-ab77-5cb283d1f81b.png)
            ![image](https://user-images.githubusercontent.com/111614210/213948889-bd73eea0-7d6a-497d-a6fb-7040e885d631.png)

    -   Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
        -   Find the average the daily atmospheric pressure of all the months.
            
            ![image](https://user-images.githubusercontent.com/111614210/213948961-3a3cba49-bfc0-48ef-b34b-09adb86726d5.png)

        -   Plot the results as a bar chart.
        
            ![image](https://user-images.githubusercontent.com/111614210/213948989-d90be323-7514-420c-aa55-4b9a53667e6c.png)

    -   About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
        -   Consider how many days elapse on Earth in the time that Mars circles the Sun once.
        -   Visually estimate the result by plotting the daily minimum temperature.
        
            ![image](https://user-images.githubusercontent.com/111614210/213949033-ce09b0ce-e103-4e63-a3dd-cee5ad64fbb0.png)
            ![image](https://user-images.githubusercontent.com/111614210/213949399-00037817-0af6-4353-a33d-1b0c716d3b78.png)

6)  Export the DataFrame to a CSV file.

## Files Uploaded
-   **Deliverable 1 jupyter notebook**: part_1_mars_news.ipynb
-   **Deliverable 2 jupyter notebook**: part_2_mars_weather.ipynb
-   **Output JSON and CSV files**: output_files/
