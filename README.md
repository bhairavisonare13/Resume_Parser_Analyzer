# 🧠 AI-Powered Resume Parser & Evaluator

A Flask-based web application that leverages Google's Gemini API to extract structured data from resumes, evaluate resume quality, provide suggestions for improvement, and recommend relevant jobs via the Jooble API.

---

## 🚀 Features

- ✅ Extracts resume details (name, contact, skills, education, etc.) from PDFs
- 📊 Provides a realistic resume score out of 100
- 💡 Gives 5 AI-generated suggestions to improve the resume
- 💼 Recommends relevant job roles and fetches job listings
- 🔐 User authentication system (Signup/Login)
- 🗂️ Stores resume details and scores in SQLite database
- 📄 Downloadable feedback file for user reference

---

## 🛠️ Tech Stack

- **Backend**: Flask, SQLite
- **AI Integration**: Google Gemini API (via `google.generativeai`)
- **Resume Parsing**: PyMuPDF (`fitz`)
- **Job Listings**: Jooble API
- **Authentication**: Werkzeug Security (Password Hashing)
- **Frontend**: HTML (Jinja2), CSS

---

## 🔧 Setup Instructions

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/Resume_Parser_Analyzer.git
    cd Resume_Parser_Analyzer
    ```

2. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Set up `.env` file**:
    Create a `.env` file in the root directory and add:
    ```
    SECRET_KEY=your-secret-key
    GOOGLE_API_KEY=your-gemini-api-key
    JOOBLE_API_KEY=your-jooble-api-key
    ```

4. **Initialize the database**:
    ```bash
    python app.py  # Database will be initialized automatically
    ```

5. **Run the application**:
    ```bash
    python app.py
    ```
    Navigate to `http://localhost:8001` in your browser.

---

## 📂 Folder Structure


