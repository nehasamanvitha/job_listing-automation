# 🚀 Job Listing Automation using n8n

## 📌 Overview
This project is an automated job scraping and filtering pipeline built using n8n.

It fetches job listings from Indeed using Apify, filters them using AI, and stores structured results into Google Sheets for easy tracking.

---

## ⚙️ Workflow Architecture

Schedule Trigger → Apify Scraper → Dataset Fetch → Limit → OpenAI Filtering → Code Parsing → Google Sheets

---

## 🔧 Tech Stack

- n8n (Workflow Automation)
- Apify (Job Scraping)
- OpenAI (AI Filtering & Scoring)
- Google Sheets (Data Storage)

---

## 🚀 Features

- ⏱️ Automated scheduled job scraping
- 🌐 Fetches real-time job listings (SEO roles)
- 🤖 AI-powered filtering using GPT
- 📊 Structured output with:
  - Title
  - Company
  - Location
  - Apply Link
  - Score
  - Reason
- 📈 Auto-stores results in Google Sheets

---

## 🧠 How It Works

### 1. Trigger
Workflow runs on a schedule using n8n Schedule Trigger.

### 2. Scraping
Uses Apify Indeed Scraper to collect job listings based on query.

### 3. Data Fetch
Retrieves dataset items from Apify.

### 4. Filtering (AI)
OpenAI processes job data and:
- Filters relevant jobs
- Scores them
- Adds reasoning

### 5. Data Cleaning
Custom JavaScript node extracts clean JSON from AI response.

### 6. Storage
Filtered jobs are appended to Google Sheets.

---

## 📂 Project Structure
job_listing-automation/
│
├── job_listing.json # n8n workflow export
└── README.md

---

## 🎥 Demo Video

👉 Add your screen recording here:

[Watch Demo]

https://github.com/user-attachments/assets/091bb4d5-0d0a-46c7-87d2-9a9113bfe4c8



---

## ⚠️ Important Notes

- API keys and credentials are not included for security reasons
- Configure your own:
  - Apify API
  - OpenAI API
  - Google Sheets OAuth

---

## 💡 Future Improvements

- Add email notifications for new jobs
- Filter based on salary/experience
- Support multiple job roles (AI/ML/DS)
- Deploy as a SaaS tool

---

## 👩‍💻 Author

Neha Samanvitha  
Aspiring AI Engineer 🚀
