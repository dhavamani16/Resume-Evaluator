#  AI Resume Analyzer & ATS Optimization System

##  Overview

The **AI Resume Analyzer** is a smart application that analyzes resumes, checks ATS (Applicant Tracking System) compatibility, and provides actionable insights to improve job selection chances.

It uses **Natural Language Processing (NLP)** and **Machine Learning (ML)** techniques to extract skills, compare resumes with job descriptions, and generate meaningful reports.

---

##  Features

*  Extract text from PDF resumes
*  NLP-based keyword extraction
*  ATS compatibility analysis
*  Resume scoring & ranking
*  Interactive data visualization
*  Export results to Excel
*  Resume customization (Word format)

---

##  Tech Stack

### 🔹 Core Libraries

* **Python**
* **PyPDF2** – Extract text from PDF resumes
* **spaCy** – NLP processing and keyword extraction
* **NLTK** – Text preprocessing
* **scikit-learn** – Machine learning & similarity scoring
* **Plotly** – Interactive data visualization
* **python-docx** – Resume editing and generation
* **openpyxl** – Excel file handling

---

## ⚙️ Project Workflow

1.  **Upload Resume (PDF)**
2.  **Text Extraction** using PyPDF2
3.  **Text Cleaning** using NLTK
4.  **Keyword Extraction** using spaCy
5.  **Similarity Scoring** using scikit-learn
6.  **Visualization** using Plotly
7.  **Export Results** using openpyxl
8.  **Resume Enhancement** using python-docx

---

##  Project Structure

```
AI-Resume-Analyzer/
│── app.py
│── requirements.txt
│── README.md
│
├── data/
│   └── sample_resumes/
│
├── models/
│   └── ml_model.pkl
│
├── utils/
│   ├── pdf_parser.py
│   ├── nlp_processor.py
│   ├── scorer.py
│   ├── visualizer.py
│   └── doc_generator.py
│
└── outputs/
    ├── results.xlsx
    └── updated_resume.docx
```

---

##  Installation

```bash
git clone https://github.com/your-username/AI-Resume-Analyzer.git
cd AI-Resume-Analyzer
pip install -r requirements.txt
```

---

##  Run the Project

```bash
python app.py
```

---

##  Example Output

* Resume Score: **85%**
* Missing Skills: **SQL, Docker**
* Suggested Improvements: Add project experience and certifications

---

## Future Enhancements

*  Web deployment (Streamlit / Vercel)
*  Deep Learning-based resume analysis
*  Automated job recommendations
*  Multi-format resume support (PDF, DOCX, TXT)

---

##  Contributing

Contributions are welcome!
Feel free to fork the repository and submit a pull request.

---

##  License

This project is licensed under the **MIT License**.

---

##  Author

**Dhavamani A**

---
