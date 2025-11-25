# House-Price-Extraction-Bot

This script automatically updates property prices in a Google Sheet using Zillow listing URLs and flags any price changes. It retrieves each URL, extracts the current listing price, compares it with the previous price stored in the sheet, and updates the sheet accordingly. The script also includes logic to parse different Zillow price formats and handle potential failures or missing data.

# Key features include:

1.Iterates through Zillow URLs stored in column A of a Google Sheet.

2.Fetches the latest property price for each listing using a custom scrapeZillowDetails(url) function.

3.Compares new prices with previously stored values to detect changes.

4.Updates the sheet with the latest price and a status message indicating change or no change.

5.Converts various price formats (including values with K or M suffixes) into comparable numbers.

6.Includes error handling and adjustable delays to reduce scraping frequency.

This script serves as a foundation for building a fully automated Zillow price-monitoring tool using Google Apps Script. If needed, the scrapeZillowDetails function can be extended with headers, proxies, or external APIs to handle Zillow’s bot protection and improve data reliability
