<h1 align="center">🔐 LV.0: LLM Vulnerability Zero - Security Vulnerability Reporter</h1>
<p align="center"><strong>AI-powered Open Source Security Vulnerability Reporting Assistant</strong></p>

---

## 🛠️ Project Overview

**LV.0** is a web-based security assistant tool that automatically detects and reports vulnerabilities in open-source projects.  
Users can upload a project (either a compressed file or a GitHub repository), and the system leverages a combination of static analysis tools and an LLM (Large Language Model) to:

- Identify security vulnerabilities
- Evaluate their severity
- Explain root causes
- Suggest actionable improvements

The ultimate goal is to serve as a **practical AI-powered security assistant** that helps developers focus on writing code without worrying about complex security analysis.

---

## 🚀 Key Features

1. **Code Upload & GitHub Integration**  
   - Supports uploading source code files or connecting directly to GitHub repositories.

2. **Static Vulnerability Filtering**  
   - Applies open-source static analysis tools for initial scanning (e.g., `semgrep`, `bandit`).

3. **LLM-based Vulnerability Interpretation**  
   - Uses an LLM to assess context, risk level, and provide human-readable explanations of vulnerabilities.

4. **Natural Language Report Generation**  
   - Automatically generates markdown-based reports with summaries, risk levels, and improvement suggestions.

5. **Interactive Web GUI**  
   - Intuitive user interface to browse vulnerabilities, view details, and download reports.

---

## 🧩 System Architecture

<img width="9049" height="4151" alt="LV 0 System Architecture (2)" src="https://github.com/user-attachments/assets/6efb1ec5-c7b6-4fca-aef8-e4e2d767464a" />



---

## Frontend

<img width="1734" height="1012" alt="KakaoTalk_20250821_184030302" src="https://github.com/user-attachments/assets/cbd4a8b0-0d6b-499a-bd3d-20140961f2e3" />
<img width="1734" height="1012" alt="KakaoTalk_20250821_184018368" src="https://github.com/user-attachments/assets/d1d00ad1-5a23-48b4-83cb-091ac4686357" />
<img width="1734" height="1012" alt="KakaoTalk_20250821_183009168" src="https://github.com/user-attachments/assets/24b50c2f-b889-46d4-b94e-0dfdbcb3f280" />

---

## PDF outputs example


![3acdd0bb-8a8e-4b87-a504-c2d945ff1146_page-0002](https://github.com/user-attachments/assets/d8f17abf-fc26-436d-b106-a47163b57046)
![3acdd0bb-8a8e-4b87-a504-c2d945ff1146_page-0001](https://github.com/user-attachments/assets/e2af226d-0133-4445-9aff-09aead028311)



---
## 💡 Tech Stack

- **Frontend**: React, TypeScript, TailwindCSS  
- **Main Backend**: FastAPI (Python)  
- **Sub Logic Services**: Flask (Static Analysis), Ollama + Deepseek (LLM), Markdown-to-PDF converter  
- **LLM Models**: Deepseek Coder  
- **Static Analysis Tools**: `semgrep`, `bandit`  
- **Database / Caching**: MongoDB, Redis  
- **DevOps**: Docker, MicroK8s, GitHub Actions  

---

## 🎯 Project Goal

> "Security doesn’t have to be hard."

LV.0 aims to simplify the traditionally complex process of security analysis,  
empowering developers to **focus on building great software** while getting proactive, intelligent security assistance in the background.

---

## 👨‍👩‍👧‍👦 Team Info

**Team Name**: Guardians of Open Source  
**Affiliation**: Dankook University, Department of Cybersecurity  

- **Team Leader**: Kyoungmin Roh  
- **AI & Security Logic Developers**: Kyoungmin Roh, Seokkyung Kang  
- **Frontend & UI Designers**: Nahee Kwon, Minji Choi  
- **Backend Developers**: Ohyeon Kwon, Seungeun Lee, Hyunbeom Jeong  

---

<p align="center">
  ⭐ <em>"Making security smarter and easier with AI."</em> ⭐
</p>


