# 🛠️ Automated CRM & Customer Data Cleaning System (Python & Pandas)

A robust, production-ready Python pipeline designed to instantly transform messy, inconsistent, and error-ridden client datasets into clean, standardized, and audit-ready business intelligence assets.

## 💼 The Business Problem
Non-technical business operations often suffer from "dirty data"—mismatched date formats, duplicate records, messy text capitalisation, and corrupted financial values. Manually fixing thousands of rows in Excel wastes hours and introduces human data-entry errors. 

This project demonstrates how a **custom Python automation script** handles complex data cleansing tasks instantly with 100% precision.

---

## 📉 Before vs. 📈 After (The Transformation)

### Mismatched Input Data (`messy_customer_data.csv`)
* Erratic capitalisation (`john smith` vs `  SARAH JONES`)
* Corrupted monetary text (`twelve dollars`, `$450.00`)
* Mixed date formats (`YYYY/MM/DD`, `DD-MM-YYYY`, `MM/DD/YYYY`)
* Hidden duplicates, missing details, and broken email formats

### Standardized Output Data (`clean_customer_data.csv`)
* All names converted to clean Title Case with zero trailing spaces.
* All financial data stripped of symbols, parsed, and converted to uniform floats.
* All signup dates unified into standard ISO database format (`YYYY-MM-DD`).
* Exact duplicate entries purged; invalid emails flagged for operational safety.

---

## 🛠️ Core Features & Technical Implementation

This automated script processes data through a 7-stage data cleaning pipeline using **Python & Pandas**:

1. **Blank Value Mitigation:** Drops completely empty rows or entries missing core identifiers (`Customer_ID`) to save database storage.
2. **Deduplication:** Automatically scans and drops duplicate records while preserving the original historical entry.
3. **Text Normalization:** Strips trailing/leading whitespaces and normalizes case inconsistencies across all text fields.
4. **Smart Date Parsing:** Leverages Pandas' advanced parsing engine to safely interpret mixed date standards and unify them.
5. **Regex Phone Extraction:** Uses Regular Expressions (`re`) to clear symbols/country codes, standardizing phone contacts into a uniform 10-digit string.
6. **Financial Data Coercion:** Safely extracts numerical text and currency symbols, converting contaminated fields into safe statistical numbers.
7. **Syntax Email Validation:** Flags broken or poorly formatted email addresses to protect company email domain deliverability scores.

---

## 🚀 How to Run the Script

### Prerequisites
Ensure you have Python 3.x and the `pandas` library installed on your system:
```bash
pip install pandas numpy
```

### Execution
1. Place your raw file named `messy_customer_data.csv` in the root folder.
2. Run the automation script:
```bash
python clean_data.py
```
3. Find your pristine dataset ready for deployment inside `clean_customer_data.csv`.

---

## 📬 Need Your Data Cleaned? Let's Connect!
Do you have thousands of rows of messy Excel sheets, broken client contact lists, or conflicting CSV datasets slowing down your business? Avoid manual entry mistakes and let code handle the heavy lifting.

* **Upwork Profile:** [Insert Your Upwork Link]
* **Fiverr Gig:** [Insert Your Fiverr Link]
* **LinkedIn:** [Insert Your LinkedIn Link]
* **Email:** your.email@example.com
