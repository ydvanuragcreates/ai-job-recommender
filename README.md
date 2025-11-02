# 🤖 AI Job Recommender

A smart web application built with Streamlit and the OPENAI API. This tool acts as a personal career assistant, allowing users to upload their PDF resume to receive an instant, AI-powered analysis of their skills, a personalized career roadmap, and real-time job recommendations.


---

## ✨ Features

* **AI Resume Analysis:** Uses the OPENAI API to instantly read and summarize a user's resume, highlighting key skills, work experience, and education.
* **Skill Gap Identification:** Provides actionable feedback on which critical skills, certifications, or experiences are missing from the resume for their desired career path.
* **Personalized Career Roadmap:** Generates a custom, step-by-step future roadmap suggesting new skills to learn and certifications to acquire.
* **Smart Job Keyword Extraction:** AI intelligently identifies the best job titles and keywords to use for job hunting based on the resume's content.
* **Real-Time Job Matching:** Connects to the Apify API to fetch and display current job openings from **LinkedIn** and **Naukri** that match the user's AI-generated keywords.

---

## 🛠️ Tech Stack

* **Frontend:** Streamlit
* **Backend:** Python
* **AI/LLM:** OPENAI API
* **Job APIs:** Apify (for LinkedIn & Naukri data)
* **PDF Parsing:** PyMuPDF (`fitz`)
* **Environment & Package Management:** `uv`
* **Secrets Management:** `python-dotenv`

---

## 🚀 How to Run Locally

Follow these instructions to get the project running on your local machine.

### 1. Prerequisites

* Python 3.10+
* [uv](https://github.com/astral-sh/uv) (or you can use `pip`)
* API keys for:
    * OPENAI API
    * Apify

### 2. Clone & Setup

```bash
# Clone the repository
git clone [https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git)
cd YOUR-REPO-NAME

# Create and activate the virtual environment
uv venv
source .venv/bin/activate  # (Linux/macOS)
.\.venv\Scripts\activate   # (Windows PowerShell)

# Install the required dependencies
uv pip install -r requirements.txt
```

### 3. Configure API Keys

You must create a `.env` file to store your secret API keys.

1.  Create a file named `.env` in the root of the project folder.
2.  Add your API keys to this file:

    ```
    GOOGLE_API_KEY="YOUR_GOOGLE_AI_STUDIO_API_KEY"
    APIFY_API_KEY="YOUR_APIFY_API_KEY" 
    ```

### 4. Run the App

With your environment active and keys in place, run the Streamlit app:

```bash
streamlit run app.py
```

Open your browser and go to `http://localhost:8501` to use the application!