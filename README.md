# Puppeteer Web Scraper API

## 📌 Overview
This project is a **Node.js Express server** that uses **Puppeteer** to scrape data from the **MoneyControl Economic Calendar**.

---

## 🚀 Features
- Efficient web scraping with Puppeteer.
- Blocks unnecessary resources like images and fonts for faster page loading.
- Extracts economic event data such as **time, country, event name, impact, actual, previous, and consensus values**.
- Graceful browser handling with error management.
- API endpoint to fetch the scraped data.

---

## 🛠️ Prerequisites
Ensure you have the following installed:

- **Node.js** (v14+ recommended)
- **npm** or **yarn**

---

## 🏁 Installation

1. Clone the repository:

```bash
git clone https://github.com/pradeep123-NOW/scrap.git
```

2. Navigate to the project directory:

```bash
cd scrap
```

3. Install dependencies:

```bash
npm install
```

---

## 🌐 Usage

1. Start the server:

```bash
npm start
```

2. Access the API endpoints:

- **`/`** - Check if the server is running.
- **`/scrape`** - Scrape data from the MoneyControl Economic Calendar.

---

## 🧐 API Endpoints

### `GET /`
Returns a simple message confirming that the server is running.

### `GET /scrape`
Scrapes the economic calendar and returns the data in JSON format:

```json
{
  "success": true,
  "message": "Data retrieved successfully",
  "total": 50,
  "tableData": [
    {
      "DayAndDate": "March 17, 2025",
      "time": "09:00 AM",
      "countryCode": "TUR",
      "countryName": "Turkey",
      "eventName": "Interest Rate Decision",
      "impact": ["highImpact"],
      "actual": "5.50%",
      "previous": "5.25%",
      "consensus": "5.40%"
    }
  ]
}
```

---

## ⚡ Project Structure

```
.
├── server.js         # Main server file
├── package.json     # Node.js dependencies
├── .gitignore       # Files to be ignored in Git
└── README.md        # Documentation
```

---

## 📦 Dependencies

- `express`: Web framework for Node.js
- `puppeteer`: Headless browser for web scraping


