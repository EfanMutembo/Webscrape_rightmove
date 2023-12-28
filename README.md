
Rightmove Web Scraping
Overview
This project involves web scraping property data from the Rightmove website for listings in Nottingham. The ultimate goal is to create a geographical map visualizing rental prices across the city.

Prerequisites
Ensure you have the required Python libraries installed:

Selenium
Webdriver_manager
Pandas
NumPy
BeautifulSoup4
Install them using:

bash
Copy code
pip install selenium webdriver_manager pandas numpy beautifulsoup4
Code Structure
1. Initiating the Driver
The code begins by initializing the Edge driver using Selenium and the webdriver_manager library. It navigates to the Rightmove website and accepts cookies.

2. Dynamic Web Scraping
A function parse_website() is defined to dynamically scrape multiple pages of property listings. The code utilizes Selenium to change pages, and BeautifulSoup is employed to parse the HTML content.

3. Extracting and Formatting Data
The create_df function is responsible for extracting relevant information such as address, house type, bedrooms, bathrooms, and guide prices from the HTML content. The extracted data is formatted and stored in a Pandas DataFrame.

4. Data Export
The resulting DataFrame is exported to a CSV file named rightmove_data.csv. This CSV file contains the collected property data for further analysis.

Usage
Run the provided Python script to initiate the web scraping process.
The script will dynamically navigate through the Rightmove website, collect property data, and store it in a CSV file.
Use the exported CSV file for data analysis or further processing.
Future Steps
The project outlines plans for training a predictive model and using GeoPandas to visualize property prices and locations on a map.

Feel free to explore and modify the code to suit your specific requirements.
