# AI Resume Parser & Candidate Matching System

## Overview

An AI-powered Resume Parser and Candidate Matching System built with Python, Groq LLM, and Pydantic. This project automates the recruitment screening process by extracting structured information from job descriptions and resumes, then evaluating how well each candidate matches a specific role.

Instead of relying on keyword matching, the system uses Large Language Models (LLMs) to understand the semantic meaning of both resumes and job descriptions, producing structured JSON outputs and AI-generated candidate scores.

---

## Features

* Extracts structured information from job descriptions
* Parses PDF and DOCX resumes
* Extracts candidate details such as:

  * Name
  * Contact Information
  * Skills
  * Education
  * Work Experience
  * Projects
  * Certifications
* Converts unstructured resume text into validated JSON using Pydantic
* Compares candidate profiles with job requirements
* Generates AI-based match scores (0–100)
* Identifies matching skills and missing skills
* Provides an overall hiring recommendation
* Automatically ranks candidates from best to worst

---

## Workflow

1. Load the job description.
2. Extract structured job requirements using an LLM.
3. Read resumes from the `resumes/` folder (PDF/DOCX).
4. Parse each resume into structured JSON.
5. Compare every resume against the job requirements.
6. Generate:

   * Match Score
   * Matching Skills
   * Missing Skills
   * Experience Analysis
   * Final Verdict
7. Rank all candidates based on their scores.

---

## Tech Stack

* Python
* Groq API
* GPT-OSS-120B
* Pydantic
* PyPDF
* python-docx
* JSON
* dotenv

---

## Project Structure

```text
.
├── resumes/
│   ├── candidate1.pdf
│   ├── candidate2.docx
│   └── ...
├── resume_parser.py
├── pyproject.toml
├── .env
└── README.md
```

---

## Learning Outcomes

This project helped me understand:

* Prompt Engineering for structured AI outputs
* Schema-based validation using Pydantic
* Resume parsing from PDF and DOCX documents
* Information extraction using Large Language Models
* Designing end-to-end AI pipelines
* Building reliable AI applications with structured JSON
* AI-powered candidate evaluation and ranking
* Integrating multiple libraries into a practical automation workflow

---

## Future Improvements

* Support for OCR-based scanned resumes
* Batch processing with parallel execution
* Interactive web interface
* ATS compatibility scoring
* Export results to CSV or Excel
* Skill gap visualization
* Support for multiple job descriptions
* Resume recommendations for candidates

---

## Disclaimer

This project is intended for educational purposes and demonstrates how Large Language Models can assist in resume screening. It should not replace human decision-making in real-world hiring processes.

---

## Author

Aryan

If you found this project useful, consider giving it a ⭐ on GitHub.
