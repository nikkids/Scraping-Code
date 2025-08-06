# 📥 Data Scraping Pipelines
This repository contains custom web scraping pipelines to collect social media data related to the 2019 and 2024 Indonesian general elections. The datasets extracted here serve as the foundation for downstream sentiment, hate speech, and geospatial analysis.

## 📁 Repository Structure

- `ScrapingTweet.ipynb`:  
  Scrapes **tweets** using keyword-based queries and date filtering. Captures text, user metadata, engagement metrics, and location information (if available).

- `ScrapYourVids.ipynb`:  
  Extracts **YouTube video comments** from political channels or content related to election discussions. Supports comment threading, author info, and like counts.

- `GMaps_Converter.ipynb`:  
  Converts **latitude-longitude coordinates and locations** from scraped data into administrative regions (e.g., province, city) using a geocoding API (Google Maps API or similar).

## ⚙️ Key Functionalities

- Supports scraping in **Bahasa Indonesia**
- Structured export in CSV/JSON format
- Ready for integration into NLP and GIS workflows
- API rate-limit handling and basic error resilience

## 📦 Tools & Libraries

- `snscrape` – Twitter scraping  
- `youtube-comment-scraper-python` or `Google API` – YouTube comment extraction  
- `Geopy`, `Google Maps API` – Reverse geocoding  
- `Pandas`, `Requests`, `JSON` – Data handling  

## 📌 Usage Notes

- Some scripts may require API keys (especially for geocoding).  
- Respect platform scraping policies and fair use guidelines.  
- Recommended to use environment variables or `.env` files for storing credentials.

## 📝 License & Credits

Developed as part of the **WRAP (Work Ready Program)** research project for political discourse analysis during the Indonesian elections. Supervised by **Fitriyani, S.Si., M.Kom.** at Telkom University.
