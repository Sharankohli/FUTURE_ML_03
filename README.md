# 📄 AI Resume Screening System

An AI-powered Resume Screening and Candidate Ranking System built using NLP and Machine Learning techniques.

This project simulates a real-world Applicant Tracking System (ATS) that evaluates multiple resumes against a recruiter-provided job description and ranks candidates based on role fit.

---

## 🚀 Overview

Hiring teams often receive hundreds of resumes for a single job role.  
Manual screening is time-consuming, inconsistent, and error-prone.

This system automates resume evaluation using:

- NLP-based skill extraction  
- TF-IDF similarity scoring  
- Skill-weighted ranking model  
- AI-generated candidate summaries  
- Interactive Streamlit dashboard  

---

## 🧠 How It Works

### 1️⃣ Job Description Input  
Recruiter pastes a job description into the system.

### 2️⃣ Resume Upload  
Multiple resumes are uploaded in PDF format.

### 3️⃣ NLP Processing  
- Text cleaning  
- Skill extraction  
- TF-IDF vectorization  
- Cosine similarity scoring  

### 4️⃣ Hybrid Skill-Weighted Scoring Model  

Final Score:

0.6 × Text Similarity (TF-IDF Cosine Similarity)  
+ 0.4 × Skill Match Ratio  

This ensures ranking is based on both textual relevance and required skill overlap.

---

## 📊 Key Features

- 📌 Job description input from recruiter  
- 📄 Multiple PDF resume upload  
- 🧠 NLP-based skill extraction  
- 📊 Skill-weighted ranking model  
- 🟢 Candidate categorization (Strong / Good / Weak Fit)  
- ⚠ Skill gap detection  
- 🧠 AI-generated resume summary  
- 👁 View / Close full resume inside dashboard  

---

## 📁 Project Structure

```
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
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 📊 Dataset Used

For job role analysis and skill vocabulary reference:

Resume Entities & Job Roles Dataset  
https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset  

This dataset was used for:

- Job description structure understanding  
- Skill extraction experimentation  
- NLP preprocessing practice  

---

## ⚙ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/Sharankohli/FUTURE_ML_03.git
cd FUTURE_ML_03
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Download spaCy Model

```bash
python -m spacy download en_core_web_sm
```

### 5️⃣ Run Application

```bash
streamlit run src/app.py
```

---

## 🛠 Tech Stack

- Python  
- Streamlit  
- Scikit-learn  
- spaCy  
- PyMuPDF  
- Custom Skill Extraction Engine  
- Hybrid Scoring Model  

---

## 👨‍💻 Author

Sharan Raj J  
B.Tech Computer Science – AI & ML  
SRM Institute of Science & Technology  


👤 Author

Sharan Raj

Machine Learning Intern – Future Interns (2026)
