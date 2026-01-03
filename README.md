![AI](https://img.shields.io/badge/AI-Local%20LLM-blue)
![Automation](https://img.shields.io/badge/Automation-n8n-orange)
![Platform](https://img.shields.io/badge/Bot-Telegram-26A5E4)
![Status](https://img.shields.io/badge/Status-Early%20MVP-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

# SkillBridge 🤖

SkillBridge is an **AI-powered resume analysis and learning guidance bot** that helps job seekers understand **why their resume fails ATS screening** and **what to fix or learn next**, without guessing.

It focuses on clarity over hype:
**What you have → What’s missing → What to improve → What to learn next**

---

## 🚩 Problem Statement

Most resumes don’t fail because candidates lack skills.
They fail because resumes don’t align with job descriptions or how **ATS (Applicant Tracking Systems)** evaluate them.

Common problems faced by candidates:

* Not knowing which **skills are missing**
* Getting filtered out by ATS without feedback
* Randomly learning skills without direction
* Resume tools that overpromise or fabricate experience

SkillBridge solves this by providing **realistic, ATS-aware, and actionable guidance**.

---

## 🚀 What SkillBridge Does

* Analyzes a resume against a target job role
* Identifies **only essential skill gaps** (no noise)
* Estimates a **realistic ATS score** (calibrated, not inflated)
* Suggests **ATS-friendly resume improvements** without fabricating experience
* Recommends **long-form YouTube learning resources** to close skill gaps

No hype. No fake scores. Just clarity.

---

## 🧠 How It Works (High-Level Flow)

1. User interacts with the bot on Telegram
2. Bot detects intent (casual vs career-related)
3. Resume is uploaded (PDF only)
4. Resume text is extracted
5. Skills are identified from the resume
6. Required skills are generated for the target role
7. Skill gap and ATS score are calculated
8. Resume improvement suggestions are generated
9. Learning resources are fetched via search
10. Results are delivered back to the user

---

## 🧱 Architecture Overview

* **Telegram Bot** → User interface
* **n8n** → Workflow orchestration and routing
* **Local LLaMA 3.2** → Reasoning, analysis, and content generation
* **Perplexity Search API** → Real YouTube learning resources

All logic is handled inside n8n workflows.

---

## 🛠️ Tools & Technologies

* **n8n** – Automation and workflow orchestration
* **Local LLaMA 3.2** – AI reasoning and text generation
* **Perplexity Search API** – Search-based learning resources
* **Telegram Bot API** – User interaction layer
* **PDF parsing** – Resume text extraction

---

## 📂 Repository Structure (Suggested)

```
SkillBridge/
│
├── workflows/
│   └── skillbridge-n8n-workflow.json
│
├── prompts/
│   ├── intent-detection.txt
│   ├── resume-improvement-prompt.txt
│   └── Job-Requirements-Generator.txt
│
├── assets/
│   ├── demo.mp4
│   └── bot-demo.png
│
└── README.md
```

---

## 🤖 Telegram Bot (Live Demo)

Bot Link:

```
https://t.me/CareerLens_bot
```

### ⚠️ Note

This bot is running on a **locally self-hosted n8n setup (not a VPS)**.
Since it relies on HTTP tunneling, the bot may not always be online.

If you try the bot and it’s inactive, please notify me on **LinkedIn**, and I’ll bring it online.

---

## ⚠️ Important Disclaimers

* This tool does **not** make hiring decisions
* ATS score is an **estimate**, not a guarantee
* Resume suggestions do **not fabricate experience**
* Learning resources are recommendations, not endorsements

---

## 🧪 Project Status

* Current stage: **Early / MVP version**
* Focus: Functionality, correctness, and clarity
  
---


## 🤝 Contributions

This is a personal build-in-public project.
Feedback, suggestions, and improvements are welcome.

---

## 📬 Contact

If you tested the bot or have feedback:

* Reach out via LinkedIn
* Open an issue in this repository

---

## ⭐ Acknowledgement

Built to solve a real problem faced during job applications — and shared to help others facing the same challenge.

---

**SkillBridge** — stop guessing, start fixing.
