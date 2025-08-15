# Job Aggregator using SERP API

## Overview
This project uses the [SERP API](https://serpapi.com/) to scrape job postings, process them, and output clean datasets for analytics or further integration into ETL pipelines. It’s designed to be extended into a Bronze → Silver → Gold layered data pipeline.

---

## 1. Prerequisites
- Python 3.8 or higher
- A valid **SERP API Key** from [serpapi.com](https://serpapi.com/)
- Git installed
- Jupyter Notebook or VS Code

---

## 2. Setup SERP API
1. Sign up at [https://serpapi.com/](https://serpapi.com/)
2. Get your API key from the dashboard  
3. Keep it safe, do not commit to GitHub

---

## 3. Clone the Repository
```bash
git clone https://github.com/<your-username>/JobAggregator.git
cd JobAggregator

---

## 3. Clone the Repository
```bash
git clone https://github.com/<your-username>/JobAggregator.git
cd JobAggregator
```
---

## 4. Install Dependenositorycies
python -m venv venv
source venv/bin/activate     # Mac/Linux  
venv\Scripts\activate        # Windows  

pip install -r requirements.txt


---

## 5.  Add Environment Variables
Create a .env file in the root directory:
SERP_API_KEY=your_serp_api_key_here


---

## 6. Run the Notebook
Open 1.JobAggregator.ipynb
Adjust search parameters (keywords, location, etc.)
Run all cells to scrape and process jobs data
Output will be saved as CSV/JSON in the output/ folder

---

## 7. Pipeline Extension
Bronze Layer: Raw data directly from SERP API
Silver Layer: Clean and standardized job data
Gold Layer: Aggregated analytics-ready dataset
Use Databricks, Airflow, or MWAA for orchestration

---

## 8. Requirements 
The requirements.txt file should include:

requests
pandas
python-dotenv
jupyter

