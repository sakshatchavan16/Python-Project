# Python-Project
IPL 2022 Player Auction Web Scraper 

# 🏏 IPL 2022 Player Auction Web Scraper

A Python web scraper that extracts IPL 2022 auction team data from the [official IPL website](https://www.iplt20.com/auction/2022) and saves it as a clean CSV file.

---

## 📦 Features

- Scrapes team auction summary: funds remaining, overseas players, total players
- Handles HTTP errors and malformed rows gracefully
- Cleans currency symbols from fund values automatically
- Exports tidy, analysis-ready CSV output

---

## 🗂️ Output Columns

| Column              | Description                          |
|---------------------|--------------------------------------|
| `SR_NO`             | Serial number                        |
| `TEAM`              | IPL franchise name                   |
| `FUNDS_REMAINING`   | Remaining purse after auction        |
| `OVERSEAS_PLAYERS`  | Number of overseas players bought    |
| `TOTAL_PLAYERS`     | Total players in the squad           |

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/ipl-auction-2022-scraper.git
cd ipl-auction-2022-scraper
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the scraper

```bash
python ipl_auction_2022_scraper.py
```

The output file `IPL_Auction_2022.csv` will be saved in the current directory.

---

## 🛠️ Requirements

- Python 3.9+
- `requests`
- `beautifulsoup4`
- `lxml`
- `pandas`

Install all at once:

```bash
pip install requests beautifulsoup4 lxml pandas
```

---

## 📁 Project Structure

```
ipl-auction-2022-scraper/
├── ipl_auction_2022.py   # Main scraper script
├── IPL_Auction_2022.csv          # Generated output (after running)
└── README.md
```

---

## 📝 Sample Output

```
SR_NO  TEAM                  FUNDS_REMAINING  OVERSEAS_PLAYERS  TOTAL_PLAYERS
1      Mumbai Indians        5.15             4                 25
2      Chennai Super Kings   10.75            4                 25
...
```

---

