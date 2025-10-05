# E-Commerce & Quotes Web Scraper

## Description
This Python project is a versatile web scraper that extracts meaningful data from websites that allow scraping. It is designed to work on *most basic websites, and for more complex or unverified websites, it falls back to **verified working sites* for reliable scraping.

The scraper can extract:
- Products from e-commerce sites (name, price, rating, reviews, description, URL)
- Books from books.toscrape.com (title, price, rating, availability, URL)
- Quotes from quotes.toscrape.com (quote text, author, tags)

All extracted data is saved into a *CSV file*.

---

## Verified Working Websites
The following websites are verified to work with this scraper:

| Name | URL | Description |
|------|-----|-------------|
| WebScraper.io Test Site | [Link](https://webscraper.io/test-sites/e-commerce/allinone) | Best for testing - specifically made for web scraping practice |
| Books to Scrape | [Link](http://books.toscrape.com/) | Book store practice site - very reliable |
| Quotes to Scrape | [Link](http://quotes.toscrape.com/) | Quotes website - always works |
| Demo Blaze Store | [Link](https://www.demoblaze.com/) | Demo e-commerce site for testing |

---

## Installation

1. Make sure you have Python 3.x installed.
2. Install required Python libraries:

bash
pip install requests beautifulsoup4 pandas lxml


---

## Usage

1. Run the scraper:

bash
python working_scraper.py


2. Choose one of the following options:
   - *Use a recommended website* (from the verified list above)
   - *Enter a custom URL* (the scraper will attempt to extract data from most basic websites)

3. The scraper will display the first few results in the console and prompt you to save the data as a CSV file.

---

## Example

### Input URL:


http://books.toscrape.com/


### Sample Output (CSV):

| name                        | price   | rating | availability | category | url                     |
|------------------------------|--------|--------|--------------|---------|------------------------|
| A Light in the Attic         | £51.77 | 3/5    | In stock     | Books   | http://books.toscrape.com/catalogue/... |
| Tipping the Velvet           | £53.74 | 1/5    | In stock     | Books   | http://books.toscrape.com/catalogue/... |

---

## Features

- Works on most basic websites
- Automatically falls back to verified working sites if the target website is complex
- Saves scraped data in CSV format
- Displays a preview of scraped items
- Error handling for invalid URLs or connection issues

---

## Notes

- Ensure the website allows web scraping before using a custom URL.
- This scraper is intended for *educational and testing purposes* only.

---

## License
This project is open-source and free to use for learning and practice purposes.
