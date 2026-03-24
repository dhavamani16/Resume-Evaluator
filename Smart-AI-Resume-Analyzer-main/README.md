# Smart AI Resume Analyzer

A Streamlit application for analyzing, optimizing, and building resumes with AI-assisted feedback, dashboards, and job search helpers.

**Live demo:** [resumind.streamlit.app](https://resumind.streamlit.app/)

---

## Features

- **Resume analysis:** ATS-oriented scoring, keyword gaps, role-aware feedback, skills gap summary
- **AI resume builder:** Multiple themes (Modern, Minimal, Professional, Creative), suggestions, ATS-friendly layout
- **Optimization:** Keyword highlighting, content tips, industry-oriented insights
- **Dashboard and analytics:** Visual summaries of resume metrics
- **Job search tools:** Integrations and helpers for exploring roles (see `jobs/`)

---

## Tech Stack

| Area | Technologies |
|------|----------------|
| App framework | [Streamlit](https://streamlit.io/), Python |
| Frontend styling | HTML, CSS, JavaScript (where used by Streamlit/custom UI) |
| Data / files | SQLite, PDF/Word handling (PyPDF2, python-docx), Excel (openpyxl) |
| NLP / ML | spaCy, scikit-learn, NLTK |
| Visualization | Plotly |

---

## Prerequisites

- Python 3.x
- [Google AI Studio API key](https://aistudio.google.com/app/apikey) for Gemini (required for AI analysis features)

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/dhavamani16/Resume-Evaluator.git
cd Resume-Evaluator/Smart-AI-Resume-Analyzer-main
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
```

**Activate:**

- Windows: `venv\Scripts\activate`
- macOS / Linux: `source venv/bin/activate`

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Download the spaCy English model

```bash
python -m spacy download en_core_web_sm
```

### 5. Environment variables

Create a file named `.env` inside the `utils/` directory (see `utils/.env.example` if present).

```env
GOOGLE_API_KEY=your_google_gemini_api_key
```

Do not commit `.env`. It should remain listed in `.gitignore`.

### 6. Run the app

```bash
streamlit run app.py
```

The app typically serves on `http://localhost:8501`.

---

## PDF processing (Windows)

If the project bundles or expects [Poppler](https://poppler.freedesktop.org/) for PDF utilities, ensure binaries are on your `PATH` or follow paths used in the project configuration.

---

## Admin login (if enabled)

- **Username:** `admin@example.com`
- **Password:** `admin123`

The admin area appears after login, near the Dashboard section, when this feature is enabled in the app.

---

## Known issue: browser autofill in Resume Builder

Using the browser autofill for name, email, or phone can leave fields visually filled while validation still fails (for example, “Please enter your email address”). Editing the field manually (delete one character and retype) usually clears the error. This comes from how autofill interacts with Streamlit form validation.

---

## Project layout (overview)

```
Smart-AI-Resume-Analyzer-main/
├── app.py                 # Main Streamlit entry
├── config/                # Job roles, courses, DB helpers
├── dashboard/             # Dashboard UI
├── feedback/              # Feedback module
├── jobs/                  # Job search / scraper utilities
├── resume_analytics/      # Analytics helpers
├── style/                 # CSS
├── utils/                 # Core logic, AI analyzer, parsers
├── requirements.txt
├── README.md
└── ...
```

---

## Contributing

1. Fork the repository
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit changes with clear messages
4. Open a Pull Request

See `.github/CONTRIBUTING.md` for more detail if included in this repo.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Repository

**Upstream reference (original project):** [Hunterdii/Smart-AI-Resume-Analyzer](https://github.com/Hunterdii/Smart-AI-Resume-Analyzer)

**This fork / copy:** [dhavamani16/Resume-Evaluator](https://github.com/dhavamani16/Resume-Evaluator)

---

## Additional documentation

- [AI_MODELS.md](AI_MODELS.md) – model and provider notes
- [DEPLOYMENT.md](DEPLOYMENT.md) – deployment notes
- [SECURITY.md](SECURITY.md) – security and reporting
