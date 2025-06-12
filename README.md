A.R.E.S. – Automated Resume Evaluation System

A.R.E.S. is your AI-powered, automated, and intelligent screening system
designed to transform how you evaluate talent.

It reads, ranks, summarizes, and matches resumes with job descriptions 
using state-of-the-art NLP models and real-time reasoning – no manual 
keyword lists, no guesswork.


🚀 Features

✔ Upload and parse resumes (PDF, DOCX, TXT)

✔ Upload job descriptions and extract required skills dynamically

✔ Automatically infer job roles using zero-shot classification

✔ Generate AI summaries of resumes for fast recruiter review

✔ Score and rank candidates using weighted Must-Have / Nice-to-Have logic

✔ View resumes as images or full previews

✔ Draft and send personalized messages to candidates

✔ Clean multipage Streamlit interface

------------------
Project Structure
------------------
Resume-Screener/
├── app.py
├── requirements.txt
├── README.md
│
├── modules/
│   ├── parser.py
│   ├── screener.py
│   ├── utils.py
│   └── job_infer.py
│
├── pages/
│   ├── 1_Home.py
│   ├── 2_ScreeningResults.py
│   └── 3_CandidateDetails.py


-----------------------------------
🧠 Requirements
-----------------------------------
Python 3.8 or above

Install all dependencies with:
> pip install -r requirements.txt

Or manually:
> pip install streamlit python-docx PyMuPDF docx2txt pdf2image pillow
> pip install sentence-transformers scikit-learn transformers torch

You’ll also need:
- poppler (for `pdf2image` support)
  • Windows: https://github.com/oschwartz10612/poppler-windows/releases/
  • macOS: `brew install poppler`

-----------------------------------
💻 Running A.R.E.S.
-----------------------------------
1. Activate your virtual environment (optional)
2. Launch with:
> streamlit run app.py

3. Use the sidebar to upload a Job Description and a batch of resumes
4. A.R.E.S. will take care of the rest
