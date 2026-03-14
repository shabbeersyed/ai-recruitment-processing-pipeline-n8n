<h1 align="center">🤖 AI Recruitment Processing Pipeline</h1>
<h3 align="center">Multi-Agent AI Hiring Automation using n8n, OpenAI, Gemini & JavaScript</h3>

<p align="center">
AI-powered recruitment workflow that screens resumes, generates candidate questionnaires, evaluates answers, and assists interviewers with AI-generated interview questions.
</p>

<p align="center">
<img src="https://img.shields.io/badge/n8n-Automation-orange?style=for-the-badge&logo=n8n"/>
<img src="https://img.shields.io/badge/OpenAI-LLM-black?style=for-the-badge&logo=openai"/>
<img src="https://img.shields.io/badge/Google%20Gemini-AI-blue?style=for-the-badge&logo=google"/>
<img src="https://img.shields.io/badge/JavaScript-Logic-yellow?style=for-the-badge&logo=javascript"/>
<img src="https://img.shields.io/badge/Google%20Sheets-Storage-green?style=for-the-badge&logo=googlesheets"/>
<img src="https://img.shields.io/badge/Gmail-Automation-red?style=for-the-badge&logo=gmail"/>
</p>

---

# 🚀 Project Overview

**AI Recruitment Processing Pipeline** is an AI-powered hiring automation system built using **n8n workflow automation**.

The system integrates **OpenAI and Google Gemini models in a multi-agent architecture** to automate the early stages of recruitment including:

• Resume screening  
• ATS scoring  
• Candidate questionnaire generation  
• AI evaluation of answers  
• Interview decision automation  
• Interview question generation for recruiters  

The workflow also logs candidate information automatically in **Google Sheets** for recruiter tracking.

---

# 🎯 Key Features

### AI Resume Screening
Automatically compares candidate resumes with the job description.

### ATS Score Calculation
Assigns an **ATS score from 0–50** using AI evaluation.

### AI Generated Questionnaire
Candidates who pass ATS screening receive a personalized questionnaire generated from:

• Job description  
• Candidate resume  

### AI Answer Evaluation
Candidate answers are evaluated using AI models.

Each answer receives a score between **1–10**.

### Automated Interview Decision
If the candidate score exceeds the threshold, an **interview confirmation email is sent automatically**.

### AI Interview Question Generator
Interviewers receive **AI-generated interview questions** based on the candidate's resume and the job description.

This removes the need for recruiters to manually search for interview questions.

### Recruitment Data Tracking
All candidate data and evaluation results are stored in **Google Sheets**.

---

# 🧠 Multi-Agent AI System

The system uses **multiple AI agents working together in a workflow pipeline**.

### AI Models Used

- OpenAI
- Google Gemini

These agents collaborate to perform tasks such as:

• Resume evaluation  
• Question generation  
• Candidate scoring  
• Interview question preparation  

---

# ⚙️ End-to-End Workflow

The recruitment automation pipeline works in multiple stages.

---

# Stage 1 — Resume Screening

1. Candidate submits resume
2. System compares resume with Job Description
3. AI generates ATS score

### ATS Logic

Score Range: 0 – 50
Threshold: 35


Decision rule:



If ATS Score > 35
Candidate proceeds to questionnaire stage
Else
Candidate filtered out


Candidates who pass this stage automatically receive a questionnaire email.

---

# Stage 2 — AI Generated Questionnaire

The system generates a **custom questionnaire** using:

• Job Description  
• Candidate Resume  

This ensures questions are **relevant to both the role and candidate profile**.

The questionnaire is sent to the candidate via **automated email**.

---

# Stage 3 — AI Evaluation of Candidate Answers

Once the candidate submits answers:

AI agents evaluate responses.

Each answer receives a score:



Score per question: 1 – 10
Total score: 50


Candidate evaluation threshold:



Pass Threshold: 75%


Decision rule:



If Candidate Score ≥ 75%
Interview Confirmation Email Sent
Else
Candidate rejected


---

# Stage 4 — Interviewer Assistance

A **multi-agent AI system** generates interview questions for recruiters.

The system analyzes:

• Job Description  
• Candidate Resume  
• Candidate responses  

Then produces **relevant interview questions automatically**.

This helps interviewers quickly prepare for the interview.

---

# 🗂 Data Storage

All recruitment data is automatically logged in **Google Sheets** including:

• Candidate name  
• Resume ATS score  
• Questionnaire score  
• Candidate responses  
• Interview status  

This allows recruiters to maintain a **structured candidate tracking sheet**.

---

# 🛠 Tech Stack

| Category | Technology |
|--------|-------------|
| Workflow Automation | n8n |
| AI Models | OpenAI, Google Gemini |
| Logic Processing | JavaScript |
| Data Storage | Google Sheets |
| File Handling | Google Drive |
| Email Automation | Gmail |

---

# 🔧 n8n Concepts Covered

This project explores several important **n8n automation concepts**.

• Event triggers  
• Workflow orchestration  
• Conditional logic  
• Data transformation  
• JavaScript code nodes  
• AI agent integration  
• Multi-step automation pipelines  
• Google Sheets integration  
• Google Drive integration  
• Gmail integration  
• File processing workflows  

To strengthen understanding, additional **smaller workflows** were also built to explore more n8n concepts hands-on.

---

# 🧩 Workflow Architecture



Candidate Resume Submission
↓
ATS Resume Screening (AI)
↓
ATS Score Check (>35)
↓
Questionnaire Generated & Sent
↓
Candidate Answers Submitted
↓
AI Evaluation of Answers
↓
Score Calculation (>75%)
↓
Interview Confirmation Email
↓
Candidate Data Stored in Google Sheets
↓
AI Generated Interview Questions for Recruiter


---

# 📸 Workflow Screenshots

### Workflow Overview

![Workflow](screenshots/workflow-overview.png)

---

### AI Agent Section

![AI Agents](screenshots/ai-agent-evaluation.png)

---

# 📂 Repository Structure



ai-recruitment-processing-pipeline
│
├── workflows
│ └── recruitment-workflow.json
│
├── screenshots
│ ├── workflow-overview.png
│ └── ai-agent-evaluation.png
│
└── README.md


---

# ▶️ How to Run

### 1️⃣ Clone repository



git clone https://github.com/shabbeersyed/ai-recruitment-processing-pipeline-n8n.git


### 2️⃣ Import workflow into n8n

Open n8n and import:



Workflows → Import → recruitment-workflow.json


### 3️⃣ Configure credentials

Set credentials for:

• OpenAI  
• Google Gemini  
• Google Sheets  
• Google Drive  
• Gmail  

### 4️⃣ Activate workflow

Submit a test candidate form to run the pipeline.

---

# 💡 Real-World Applications

This project demonstrates how **AI workflow automation can help HR teams**:

• automate resume screening  
• reduce manual candidate evaluation  
• generate relevant interview questions  
• automate candidate communication  
• track recruitment data efficiently  

---

# 🔮 Future Improvements

Potential enhancements include:

• recruiter dashboard  
• candidate ranking system  
• interview scheduling automation  
• Slack recruiter alerts  
• ATS integrations  

---

# 👨‍💻 Author

**Shabbeer Basha Syed**

Master’s in Information Systems & Technology  
University of North Texas  

Areas of Interest

• AI workflow automation  
• intelligent agent orchestration  
• data-driven systems  
• QA automation  

GitHub  
https://github.com/shabbeersyed

---

⭐ If you find this project interesting, feel free to star the repository!
