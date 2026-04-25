# 🔷 Project Samanvay — AI Document Intelligence Pipeline

> A no-code GenAI automation pipeline simulating a multinational green energy 
> infrastructure corridor spanning India, Germany, and the UAE.

Built as part of the **Gen AI Bootcamp** under coach **Dr. Asma Shora**.

---

## 🎯 What It Does

A field engineer submits a document validation request via a Tally form.  
The pipeline automatically:
1. Captures the submission via **Zapier**
2. Sends it to **Google Gemini AI** for intelligent validation & analysis
3. Auto-generates a structured **Google Doc** report saved to Drive
4. Emails a formatted **HTML management report** to leadership — instantly

No code. No manual steps. Fully automated.

---

## 🛠️ Tech Stack

| Tool | Role |
|---|---|
| Tally | Form intake (field engineer submission) |
| Zapier | Workflow automation & orchestration |
| Google Gemini AI (gemini-2.5-flash) | AI validation & report generation |
| Google Docs + Drive | Auto-generated report storage |
| Gmail | HTML management report delivery |
| Lovable | Landing page |

---

## 🏗️ Pipeline Architecture

Tally Form → Zapier → Google Gemini AI → Google Docs (saved to Drive)
→ Gmail (HTML Management Report)

---

## 🔗 Live Links

- 🌐 Landing Page: [samanvay-ai-insight.lovable.app](https://samanvay-ai-insight.lovable.app)

---

## 💡 Key Technical Decisions

- **Pure HTML output from Gemini** — instructed to use only `h3` and `p` tags to avoid markdown rendering issues in Gmail
- **3 sequential Zapier Formatter steps** — each strips one character type (`\n`, `['`, `']`) since free plan doesn't support multi-replace
- **"Candidates Content Parts Text" field** used from Gemini (not "Step Output") to avoid array bracket wrapping
- **Individual step retesting** in Zapier to avoid stale cached data issues

---

## 👩‍💻 Built By

**Bhuvaneshwari V Raghavan**  
BI & Data Analytics Professional | IIT Roorkee Executive PG — Data Analytics  
🔗 [LinkedIn](https://www.linkedin.com/in/bhuvaneshwari-vijay-data-analyst) | 📧 bhuvaneshwari.vijay@gmail.com
