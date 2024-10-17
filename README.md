# mars_weather_data

## Introduction
This project consists of two parts: scraping Mars news headlines and preview text, and extracting Mars weather data for analysis. Using Python's automation and data parsing tools such as **Splinter** and **BeautifulSoup**, the scripts automate the process of collecting data from specific Mars-related websites and prepare it for analysis.

- **Part 1**: Scrapes the latest news articles (title and preview text) from a Mars News website.
- **Part 2**: Scrapes Mars weather data from a temperature tracking website and provides tools for analysis and visualization.

## Table of Contents
- [Introduction]
- [Installation]
- [Usage]
  - [Part 1: Mars News Scraper]
  - [Part 2: Mars Weather Scraper]
- [Contributors]

## Installation
1. Clone the repository or download the `.ipynb` files.
2. Install the necessary Python packages using the following command:
    ```bash
    pip install splinter beautifulsoup4 matplotlib pandas
    ```
3. **Browser Setup**: The project relies on **Splinter**, which automates browser interactions. You need to install a browser driver (In my case, I installed ChromeDriver) that corresponds to your browser version. I

4. Ensure that the driver is available in your system's PATH, or specify the path in the code.

## Usage

### Part 1: Mars News Scraper
The first part of the project scrapes news titles and preview text from the Mars News website.

1. **Run the code**: 
    - The script uses **Splinter** to open a browser, visit the Mars News site, and scrape the latest news article data.
    - The website URL used is: `https://static.bc-edx.com/data/web/mars_news/index.html`.
  
2. **Extracted Data**:
    - Titles and preview text for the most recent articles are extracted from the website’s HTML.
  
3. **Code Breakdown**:
    - **Step 1**: Opens a browser session using `splinter`.
    - **Step 2**: Scrapes the HTML for specific elements containing the title and preview text using `BeautifulSoup`.

### Part 2: Mars Weather Scraper
The second part scrapes Mars weather data and provides tools to analyze the temperature data.

1. **Run the code**:
    - The script opens the Mars Temperature site and scrapes temperature data related to Mars.
    - The data is stored in a structured format for analysis, with the website URL being `https://static.bc-edx.com/data/web/mars_facts/temperature.html`.

2. **Data Visualization**:
    - Uses **Matplotlib** to generate visualizations from the scraped weather data.
    - The script includes methods for scraping the temperature data and plotting daily or monthly average temperatures.

3. **Code Breakdown**:
    - **Step 1**: Browser session is opened and data is scraped from the Mars temperature page.
    - **Step 2**: The data is being processed and visualized using Pandas and Matplotlib.

## Dependencies
This project requires the following Python libraries:
- **Splinter**: For automating browser interaction.
- **BeautifulSoup**: For parsing HTML content.
- **Matplotlib**: For visualizing data (Part 2).
- **Pandas**: For data handling and manipulation (Part 2).

Installed all dependencies via:
```git bash
pip install splinter beautifulsoup4 matplotlib pandas

## Contributors
J. Naum
