# 🤖 AI Recruiting Agent [HR-Assistant](https://eu2.make.com/public/shared-scenario/EHewIKVW9Di/hr-assistant)

An automated hiring assistant built in **Make (Integromat)** that screens resumes, evaluates candidates, and logs structured results — saving hours of manual work while ensuring consistent, bias-free shortlisting.

---

## 🚀 What It Does
This AI Recruiting Agent automates the early stage of hiring:

- **Monitors** a Google Drive folder for new resumes  
- **Extracts** candidate details (name, email, LinkedIn, etc.)  
- **Analyzes** resumes to answer 4 predefined screening questions  
- **Scores** each response (0–2) and calculates a total  
- **Logs** all results in a Google Sheet — ready to review and rank  

---

## 🧠 Who Should Use It
Ideal for **HR teams, recruiters, and startups** that need:
- Faster, hands-free resume screening  
- Consistent, objective evaluations  
- A structured, data-driven candidate list  

---

## ⚙️ How It Works
The system runs through two connected scenarios in **Make**:

1. **Resume Intake Scenario**
   - Watches a Google Drive folder for new resumes  
   - Converts each PDF to JSON using PDF.co  
   - Sends structured data to the AI Agent for analysis and scoring  

2. **Google Sheets Logging Scenario**
   - Receives the AI Agent’s output  
   - Appends candidate details, answers, and scores to Google Sheets  

---

## 🧩 Apps Used
| App | Purpose |
|-----|----------|
| **Google Drive** | Watch folder for new resumes |
| **PDF.co** | Convert PDF to JSON |
| **HTTP Module** | Retrieve JSON data |
| **Make AI Agent** | Read and evaluate resumes |
| **Google Sheets** | Store and rank candidate data |

---

## 🧭 Setup Guide

1. **Create** a Google Drive folder for incoming resumes  
2. **Build** both Make scenarios (`Resume Intake` and `Log to Sheet`)  
3. **Connect** your **PDF.co**, **Google**, and **AI Agent** modules  
4. **Set up** your Google Sheet with columns for contact info, answers, and scores  
5. **Test** by uploading a sample resume — results appear automatically in Sheets  

Once configured, every new resume is automatically processed and scored.

---

## 🔗 Try It Here
👉 [AI Recruiting Agent Template on Make](https://eu2.make.com/public/shared-scenario/EHewIKVW9Di/hr-assistant)

---

### 💡 Example Output
| Name | Email | LinkedIn | Q1 | Q1 Points | Q2 | Q2 Points | Q3 | Q3 Points | Q4 | Q4 Points | Total |
|------|--------|-----------|----|------------|----|------------|----|------------|----|------------|--------|
| John Doe | john@example.com | linkedin.com/in/johndoe | "Has written YouTube scripts" | 2 | "Experience with marketing content" | 2 | "No team management shown" | 1 | "Not found" | 0 | **5** |

---

Made with ❤️ using [Make.com](https://www.make.com)

