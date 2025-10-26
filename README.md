# 🕵️‍♂️ Async Job Scraper — Playwright + BeautifulSoup + Excel Styling

A **fully asynchronous** job scraper that collects listings from  
**[Real Python Fake Jobs](https://realpython.github.io/fake-jobs/)** and outputs a **professionally formatted Excel report**.

---

## 🚀 Overview

This scraper demonstrates **modern web automation and data cleaning** using:
- **Playwright (async)** for browser automation  
- **BeautifulSoup** for HTML parsing  
- **Tenacity** for retries  
- **Pandas** for structuring data  
- **OpenPyXL** for Excel styling  

It’s clean, reliable, and production-ready — ideal for portfolio or Upwork demonstration.

---

## 🧠 Key Features

✅ Asynchronous scraping (non-blocking)  
✅ Retry logic with exponential backoff  
✅ Graceful handling of missing data  
✅ Automatic Excel formatting (colors, borders, filters)  
✅ Timestamped footer and data source reference  

---

## 🧩 Tech Stack

| Category | Technology |
|-----------|-------------|
| Automation | [Playwright (async)](https://playwright.dev/python/) |
| Parsing | [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/) |
| Data | [Pandas](https://pandas.pydata.org/) |
| Retry | [Tenacity](https://tenacity.readthedocs.io/) |
| Excel | [OpenPyXL](https://openpyxl.readthedocs.io/) |
| Logging | Python `logging` module |

---

## ⚙️ Setup

### 1. Install Requirements
```bash
pip install playwright beautifulsoup4 pandas openpyxl tenacity
python -m playwright install
```

### 2. Run the Script
```bash
python fake_jobs.py
```

The script will:
1. Scrape all job listings  
2. Fetch details (location + description)  
3. Clean and structure the data  
4. Save everything to `fake_jobs.xlsx` with full styling  

---

## 🎨 Excel Output

**Formatted Excel Includes:**
- Dark blue header (`#1F4E78`), white bold text  
- Alternating light-grey rows (`#F5F5F5`)  
- Borders on all cells  
- Auto-fit column widths  
- Frozen header + filters  
- Footer with source and timestamp  

| Job Title | Company Name | Location | Date Posted | Logo URL | Job Detail URL | Job Description |
|------------|---------------|-----------|--------------|-----------|----------------|----------------|
| Python Developer | Real Python | Remote | 2025-10-23 | [Logo](#) | [Link](#) | Build exciting Python apps! |

---

## 📜 Example Log Output

```
2025-10-23 14:02:01 | INFO | Loading page 1...
2025-10-23 14:02:03 | INFO | Found 20 job cards.
✅ Saved 80 job records to fake_jobs.xlsx
```

---

## 📈 Project Structure

```
📁 fake_jobs_scraper/
├── fake_jobs.py       # Main scraper
├── fake_jobs.xlsx     # Output file
├── requirements.txt   # Dependencies
└── README.md          # Documentation
```

---

## 🧩 Future Enhancements

- [ ] Parallelize detail page fetching  
- [ ] Add CLI options (`--headless`, `--output`)  
- [ ] Include progress bar with `rich.progress`  
- [ ] Add CSV/JSON export options  

---

## 👨‍💻 Author

**Onyekachi Ejimofor**  
_Data Extraction • Web Automation • Data Cleaning Specialist_  

