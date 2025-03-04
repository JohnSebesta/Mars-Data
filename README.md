# Mars-Data

Overview

This project involves scraping and analyzing data from two different sources related to Mars: the Mars News website and the Mars Weather website. In Part 1, we focus on scraping the latest Mars news articles, extracting the titles and preview text. In Part 2, we scrape Mars weather data from the Curiosity rover’s temperature data, perform basic analysis, and visualize the results. These tasks utilize Python libraries such as BeautifulSoup, Pandas, and Matplotlib.

Methodology

Part 1: Scrape Titles and Preview Text from Mars News
1. Set Up Automated Browsing

We begin by using Python’s BeautifulSoup and Requests libraries to automate browsing and scrape the Mars News website. After inspecting the page’s structure, we identify the HTML elements containing the titles and preview texts of the news articles.

2. Scrape Data

We create a BeautifulSoup object to parse the HTML content.
We extract the title and preview text from each article by navigating to the relevant HTML tags.
Each title and preview pair is stored in a Python dictionary with keys title and preview.
3. Store Data

All the dictionaries containing title and preview pairs are stored in a Python list.
Optionally, the data is exported to a JSON file for easier sharing.
4. Display Data

The list of dictionaries is printed within the notebook to show the extracted information.

Part 2: Scrape and Analyze Mars Weather Data
1. Scrape Mars Weather Data

We use BeautifulSoup to scrape data from the Mars Temperature Data website (URL: https://static.bc-edx.com/data/web/mars_facts/temperature.html). We inspect the page’s structure and locate the HTML table containing the weather data.

2. Assemble Data

The data is parsed and organized into a Pandas DataFrame.
The DataFrame contains the following columns:
id: The identification number for a transmission from the Curiosity rover.
terrestrial_date: The date on Earth.
sol: The number of elapsed Martian days.
ls: The solar longitude.
month: The Martian month.
min_temp: The minimum temperature in Celsius for a single Martian day.
pressure: The atmospheric pressure at the Curiosity rover's location.
3. Data Type Conversion

We examine the data types of each column in the DataFrame.
If necessary, we cast the columns to the appropriate data types (e.g., datetime, int, float).
4. Data Analysis

We perform the following analysis using Pandas:

Mars Months: Count how many distinct Martian months exist in the dataset.
Martian Days: Calculate the total number of Martian days (sols) represented in the dataset.
Temperature Analysis:
Find the coldest and warmest months on Mars by calculating the average minimum temperature for each month.
Plot the monthly average temperatures as a bar chart.
Atmospheric Pressure Analysis:
Find the months with the lowest and highest atmospheric pressure by calculating the average daily pressure for each month.
Plot the monthly average pressure as a bar chart.
Martian Year Length: Estimate how many terrestrial days elapse in a Martian year by visually analyzing the daily minimum temperatures across the dataset.
5. Data Export

The DataFrame is exported to a CSV file for further use or sharing.
Results

Part 1: Mars News Scraping
Data Extraction: We successfully scraped the Mars News website to extract titles and preview text for the latest news articles.
Data Storage: The scraped data was stored as a list of dictionaries, and optionally exported as a JSON file.
Output: The list of dictionaries was printed in the notebook for review.
Part 2: Mars Weather Data Scraping and Analysis
Data Scraping: We successfully scraped the Mars weather data from the Mars Temperature Data site and parsed it into a Pandas DataFrame.
Data Analysis:
We identified the number of unique Martian months and the total number of Martian days (sols).
The average minimum temperature for each Martian month was calculated, revealing the coldest and warmest months. A bar chart was generated to visualize the temperature variation.
We calculated the average atmospheric pressure for each Martian month, revealing the months with the highest and lowest pressures. A bar chart was also generated for this analysis.
We estimated the number of terrestrial days in a Martian year by visually plotting the daily minimum temperature data.
Data Export: The cleaned and analyzed data was successfully exported to a CSV file.

References
ChatGPT
XperLEarning Assistant
The tutor Fred Logan
