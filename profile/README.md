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

<img width="5588" height="7228" alt="System Architecture" src="https://github.com/user-attachments/assets/2f21e8b0-a145-4483-be88-897879bf9b2b" />


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


