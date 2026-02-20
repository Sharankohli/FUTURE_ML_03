📄 AI Resume Screening System

An intelligent Resume Screening and Candidate Ranking System built using NLP and Machine Learning techniques.

This project simulates a real-world Applicant Tracking System (ATS) that evaluates multiple resumes against a recruiter-provided job description and ranks candidates based on role fit.

🚀 Project Overview

Hiring teams often receive hundreds of resumes for a single role. Manual screening is slow, inconsistent, and prone to bias.

This system automates resume evaluation by:

Extracting skills from job descriptions and resumes

Performing skill-weighted similarity matching

Ranking candidates based on role alignment

Identifying missing skills

Generating AI-based resume summaries

Providing an interactive recruiter dashboard

The system is built as a Streamlit-based web application for practical usability.

🧠 How It Works
1️⃣ Job Description Input

Recruiter pastes a job description into the system.

2️⃣ Resume Upload

Multiple resumes are uploaded in PDF format.

3️⃣ NLP Processing

Text cleaning (lemmatization, stopword removal)

Skill extraction

Feature vectorization (TF-IDF)

4️⃣ Skill-Weighted Scoring Model

Final Score =

0.6 × Text Similarity (TF-IDF Cosine Similarity)
+ 0.4 × Skill Match Ratio


This ensures candidates are ranked based on both textual relevance and actual required skill overlap.

5️⃣ Dashboard Output

For each candidate, the system displays:

Final Score

Skill Match Ratio

Matched Skills

Missing Skills

Candidate Category (Strong / Good / Weak Fit)

AI-generated resume summary

View / Close full PDF resume

🛠 Tech Stack

Python

Streamlit

Scikit-learn (TF-IDF, Cosine Similarity)

PyMuPDF (PDF parsing)

Custom Skill Extraction Engine

Hybrid Scoring Model

📊 Dataset Used

For job role analysis and skill vocabulary reference:

📄 Resume Entities & Job Roles Dataset
🔗 https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset

This dataset was used for:

Job description structure understanding

Skill extraction experimentation

NLP preprocessing practice

📁 Project Structure
FUTURE_ML_03/
│
├── src/
│   ├── app.py
│   ├── preprocess.py
│   ├── matcher.py
│   ├── skills.py
│   ├── pdf_reader.py
│   ├── summary_generator.py
│
├── data/
│   └── jobs_small.csv
│
├── .gitignore
├── requirements.txt
└── README.md

⚙ Installation
1️⃣ Clone Repository
git clone https://github.com/Sharankohli/FUTURE_ML_03.git
cd FUTURE_ML_03

2️⃣ Create Virtual Environment
python -m venv venv
venv\Scripts\activate   # Windows

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Run Application
streamlit run src/app.py

🎯 Key Features

📌 Job description input from recruiter

📄 Multiple PDF resume upload

🧠 NLP-based skill extraction

📊 Skill-weighted ranking model

🟢 Candidate categorization

⚠ Skill gap detection

🧠 AI-generated resume summary

👁 View/Close full resume inside dashboard

📈 Future Improvements

GPT-based intelligent resume summarization

Skill importance weighting

Resume keyword highlighting

Export ranking report (CSV/PDF)

Advanced semantic embeddings (Sentence Transformers)

👨‍💻 Author

Sharan Raj J
