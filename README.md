#  AI Resume Analyzer — n8n + Ollama

An AI-powered Resume Analyzer that evaluates a candidate's resume against a job description using **n8n, Ollama, and the Gemma 3 model**. It extracts text from an uploaded PDF resume and generates an AI-based analysis to help identify relevant skills, missing qualifications, and areas for improvement.

##  Features

-  **PDF Resume Upload** — Upload a resume in PDF format through an n8n form.
-  **Job Description Input** — Enter the job description for comparison.
-  **Automatic Text Extraction** — Extract resume text from the uploaded PDF.
-  **AI-Powered Analysis** — Use the Gemma 3 model through Ollama to analyze the resume.
-  **Skill Matching** — Identify matching skills and missing or unclear skills.
-  **Estimated ATS Compatibility Score** — Generate an estimated score out of 100.
-  **Job Match Score** — Estimate how closely the resume matches the job description.
-  **Improvement Suggestions** — Get recommendations to improve the resume.
-  **Local AI Processing** — Run the language model locally without relying on paid OpenAI API credits.

##  Technologies Used

- **n8n** — Workflow automation
- **Ollama** — Local large language model runtime
- **Gemma 3 (4B)** — AI model for resume analysis
- **PDF Extraction** — Extract text from uploaded resumes

## ⚙️ How It Works

1. The user uploads a resume in PDF format.
2. The user enters the target job description.
3. n8n extracts the text from the PDF.
4. The extracted resume text and job description are sent to the AI workflow.
5. Ollama runs the Gemma 3 model to analyze the resume.
6. The workflow generates a structured report containing:
   - Resume Summary
   - Matching Skills
   - Missing or Unclear Skills
   - Estimated ATS Compatibility Score
   - Resume Improvement Suggestions
   - Estimated Overall Job Match Score

##  Screenshots

Add your project screenshots below to demonstrate the workflow and its output.

### 1. n8n Workflow

![n8n Workflow](screenshots/workflow.png)

### 2. Resume Upload Form

![Resume Upload Form](screenshots/resume-form.png)

### 3. AI Resume Analysis Output

![AI Resume Analysis](screenshots/analysis-output.png)

> Replace these screenshot paths with your actual screenshot files.

##  Requirements

Before running the project, make sure you have:

- n8n installed and running
- Ollama installed and running
- The `gemma3:4b` model downloaded in Ollama
- A computer with sufficient memory and processing resources to run the model

##  Setup Instructions

### 1. Install Ollama

Download Ollama from:

https://ollama.com/

### 2. Download the Gemma 3 Model

Open PowerShell or your terminal and run:

```bash
ollama pull gemma3:4b
```

### 3. Start n8n

Start your local n8n instance using your existing installation method.

### 4. Import the Workflow

1. Download or clone this repository.
2. Open n8n in your browser.
3. Import the exported workflow JSON file.
4. Make sure the Ollama Chat Model node is configured correctly.
5. Verify that n8n can connect to your local Ollama instance.
6. Open the form and test the workflow with a sample PDF resume and job description.

##  Privacy & Limitations

- The project is designed to use a local AI model instead of a paid OpenAI API.
- Local processing can help reduce the need to send resume data to an external AI API, but privacy also depends on your n8n configuration and other connected services.
- ATS compatibility and job match scores are **AI-generated estimates**, not official scores or guarantees of getting an interview.
- Results depend on the quality of the resume, the job description, and the model's analysis.
- Keep personal resumes, credentials, API keys, and other sensitive information out of the public repository.

##  Project Goal

The goal of this project is to explore AI-powered document analysis and workflow automation using open-source tools. It demonstrates how local language models can be integrated into n8n to build practical AI applications.

##  Author

**Nagina Azhar**

Learning Python, AI, and workflow automation — building practical projects step by step.

---

 If you find this project interesting, feel free to explore the workflow and its implementation.
