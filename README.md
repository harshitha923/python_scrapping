# 🛍️ Amazon Product Web Scraper

A Python-based web scraping script to extract product information such as title, price, rating, seller, and availability from Amazon product listings. The scraper uses `BeautifulSoup` and `requests`, and saves the scraped data in a structured `CSV` file for further analysis.

> ⚠️ This project is for educational and research purposes only. Scraping Amazon is against their [Terms of Service](https://www.amazon.in/gp/help/customer/display.html?nodeId=508088), and it’s recommended to use their official API for production applications.

---

## 📌 Features

- Scrapes product data from Amazon's listing pages
- Extracts:
  - 📦 Product Title
  - 💰 Price
  - ⭐ Rating
  - 🛒 Seller
  - ✅ Availability
- Saves the data to a CSV file (`amazon_products.csv`)
- Supports automated crawling through product links

---

## 🛠️ Technologies Used

- Python 3.x
- BeautifulSoup
- Requests
- Pandas
- NumPy
- Regex

---

## 🚀 How It Works

1. Sends a request to the Amazon category or search results page.
2. Parses the HTML using `BeautifulSoup`.
3. Extracts links to individual product pages.
4. Visits each product page and extracts:
   - Title
   - Price
   - Rating
   - Seller
   - Availability
5. Stores the results in a Pandas DataFrame and saves it as a CSV.

---

## 🧪 Sample Output (CSV)

| title                       | price | rating | seller       | availability    |
|----------------------------|-------|--------|--------------|-----------------|
| Wireless Headphones XYZ    | 2,199 | 4.3    | JBL Store    | In stock        |
| Noise Cancelling Earbuds   | 3,499 | 4.0    | boAt Official| Not Available   |
