# AI-Job-Market-Analyzer

An end-to-end AI-powered platform that analyzes job market trends, predicts salaries, recommends roles, and evaluates resume compatibility using NLP and Machine Learning.

# Problem Statement
Freshers and job seekers face three major challenges:

* Skill Confusion — Unclear which skills are in demand
* Salary Blindspot — No idea of realistic salary expectations
* Role Mismatch — Difficulty mapping their profile to the right job roles

This project solves all three using real data, AI, and interactive dashboards.

# Features
  Feature  --------------------------------------------  Description
* 📈 Skill Demand Analyzer  --------------------------   Identifies top skills from 1.62M+ job postings
* 💰 Salary Predictor  --------------------------------  Predicts salary based on skills, experience & location
* 🎯 Job Recommender  ---------------------------------- Suggests job roles using Cosine Similarity
* 🧠 Resume Matcher  ----------------------------------- Compares your resume against job descriptions
* 🔍 Skill Gap Analyzer -------------------------------  Tells you exactly what skills you're missing
* 📄 ATS Score Checker  -------------------------------  Scores your resume against a target job role
* 📊 Interactive Dashboard  ---------------------------  Power BI dashboard with filters by location, role & experience
* 🤖 AI Chatbot  -------------------------------------   Basic chatbot for job-related queries

   # Tech Stack
    Layer  ----------------------------------  Tools
  * Data Collection  -----------------------   Python, BeautifulSoup, Selenium, Scrapy
  * Data Sources  ---------------------------  LinkedIn, Naukri, Indeed, Kaggle Datasets
  * Data Cleaning  --------------------------  Pandas
  * EDA & Visualization  --------------------  Matplotlib, Seaborn, Power BI
  * NLP  ------------------------------------  spaCy, NLTK, HuggingFace Transformers, TF-IDF
  * Machine Learning  -----------------------  Scikit-learn (Linear Regression, Random Forest, Cosine Similarity)
  * Deployment  ----------------------------   Streamlit
  * Dashboard  -----------------------------   Power BI

    # 📂 Project Structure

```text
job-market-analyzer/
│
├── 📂 data/
│   ├── raw/                    # Raw scraped CSVs
│   └── processed/              # Cleaned datasets
│
├── 📂 notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda.ipynb
│   ├── 04_nlp_skill_extraction.ipynb
│   └── 05_ml_models.ipynb
│
├── 📂 src/
│   ├── data_cleaning.py        # Null removal, normalization
│   ├── eda.py                  # Charts and analysis
│   ├── model.py                # Salary prediction model
│   └── recommender.py          # Job recommendation engine
│
├── 📂 app/
│   └── streamlit_app.py        # Web app UI
│
├── 📂 dashboard/
│   └── powerbi.pbix            # Power BI dashboard file
│
├── 📄 requirements.txt
└── 📄 README.md
```

# 📊 Dashboard Insights
Key findings from the Power BI dashboard (1.62M+ job postings, 216 countries):

* Top Roles: User Interface Designer (14,036), User Experience Designer (13,935), UX/UI Designer (7,028)
* Top Job Portals: FlexJobs (8.04%), Stack Overflow Jobs (8.01%), Jobs2Careers (8%)
* Top Hiring Locations: Valletta, Yaren District, Willemstad
* Qualification Distribution: Fairly uniform across BBA, BA, BCA, M.Tech, MBA, PhD (~10% each)
* Work Types: Full-time, Part-time, Contract, Intern, Temporary
* Gender Preference: Male (539K), Both (538K), Female (538K) — near equal distribution
