# Flipkart Review Scraper

## Project Overview
The **Flipkart Review Scraper** is a Flask-based web application that automatically extracts customer reviews of products from Flipkart.  

The application allows users to search for a product, scrape customer reviews from the Flipkart product page, and store the extracted data in a **MongoDB database** for further analysis.

This project demonstrates the use of **web scraping, backend development with Flask, and database integration using MongoDB**.

---

## Problem Statement
E-commerce platforms like Flipkart contain thousands of customer reviews that provide valuable insights about products. Manually collecting and analyzing these reviews is time-consuming.

This project automates the process by scraping reviews and organizing them in a structured format.

---

## Features

- Search products directly from Flipkart
- Automatically extract product reviews
- Collect key review details:
  - Product Name
  - Customer Name
  - Rating
  - Review Heading
  - Customer Comment
- Store reviews in **MongoDB Atlas**
- Save scraped data in **CSV format**
- Display reviews on a web interface

---

## Tech Stack

### Programming Language
- Python

### Backend Framework
- Flask

### Web Scraping
- BeautifulSoup (bs4)
- Requests
- urllib

### Database
- MongoDB
- PyMongo

### Frontend
- HTML
- Jinja Templates

---

## Project Workflow

1. User enters a product name in the web interface.
2. Flask backend sends a request to the **Flipkart search page**.
3. The scraper identifies the first product from the search results.
4. The scraper extracts reviews from the product page.
5. Review details are processed and structured.
6. Data is stored in:
   - MongoDB database
   - CSV file
7. The scraped reviews are displayed on the results page.

---

## Project Structure

```
review_scrap_pwskills/
│
├── templates/
│   ├── index.html
│   └── result.html
│
├── scrapper.log
├── app.py
├── requirements.txt
└── README.md
```


---

## Installation

### 1 Clone the repository

```
git clone https://github.com/Ktrimalrao/review_scrap_pwskills.git
```

###2 Navigate to project folder
```
cd review_scrap_pwskills
```

### 3 Install dependencies
```
pip install -r requirements.txt
```

### 4 Run the application
```
python app.py
```

### 5 Open in Browser
```
http://localhost:5000
```

| Product | Customer Name | Rating | Heading   | Comment           |
| ------- | ------------- | ------ | --------- | ----------------- |
| iPhone  | Rahul         | 5      | Excellent | Very good product |
| iPhone  | Ankit         | 4      | Good      | Value for money   |


## Database Storage

The scraped reviews are stored in **MongoDB Atlas**.

### Database
review_scrap

### Collection
review_scrap_data

## Requirements
flask
flask_cors
requests
bs4
pymongo


---

## Author

**K. Trimal Rao**

🔗 **LinkedIn**  
https://www.linkedin.com/in/k-trimal-rao-397924253/

💻 **GitHub**  
https://github.com/Ktrimalrao
