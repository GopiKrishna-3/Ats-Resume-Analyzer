# ATS Resume Analyzer

An enterprise-grade, AI-powered Applicant Tracking System (ATS) optimization tool. Built with Python, Flask, and the **Google Gemini API**, this application provides a rigorous, evidence-based evaluation of resumes against targeted job descriptions to identify precise skill alignments and critical gaps.

## 🚀 Live Demo
**https://ats-resume-analyzer-3-w4s2.onrender.com/**

---

## 🎯 Overview

Modern recruitment relies heavily on Applicant Tracking Systems to filter candidates. The ATS Resume Analyzer bridges the gap between candidate submissions and automated screening systems by providing transparent, actionable insights. By leveraging advanced natural language processing (Gemini 2.5 Flash), the tool parses complex PDF resumes and strictly evaluates them against provided job descriptions without assuming undocumented competencies.

## ✨ Key Features

- **Input Validation:** Automatically detects and rejects invalid or overly brief job descriptions to ensure analysis integrity.
- **Evidence-Based Scoring:** Generates an objective ATS Match Score (0-100) based strictly on documentable evidence found within the uploaded resume.
- **Comprehensive Skill Matrix:**
  - **Matched Competencies:** Identifies successfully demonstrated skills, categorized by priority (Must-Have vs. Nice-to-Have), complete with direct citations from the resume.
  - **Skill Gap Analysis:** Highlights critical missing requirements and articulates the business justification for each skill within the context of the role.
- **Structural Diagnostics:** Pinpoints concrete weaknesses in resume construction (e.g., lack of quantifiable metrics, vague phrasing).
- **Actionable Remediation:** Provides specific, targeted suggestions detailing exact sections and bullet points requiring modification to improve ATS compatibility.

## 🏗️ Architecture & Technology Stack

- **Backend Framework:** Python / Flask
- **AI / LLM Engine:** Google Gemini API (`gemini-2.5-flash`)
- **Document Processing:** PyPDF2 (PDF text extraction)
- **Frontend Design:** Vanilla HTML/CSS/JS with a responsive, modern glassmorphism UI
- **Deployment:** Production-ready configuration using Gunicorn

---

## 💻 Local Development Setup

### Prerequisites
- Python 3.9+
- A valid Google Gemini API Key

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/GopiKrishna-3/Ats-Resume-Analyzer.git
   cd Ats-Resume-Analyzer
   ```

2. **Initialize a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure environment variables:**
   Create a `.env` file in the project root and append your API credential:
   ```env
   GEMINI_API_KEY=your_gemini_api_key_here
   ```

5. **Start the application:**
   ```bash
   python main.py
   ```
   The application will be accessible at `http://localhost:8000`.

---

## 📄 License
This project is open-source and available under standard MIT licensing parameters.
