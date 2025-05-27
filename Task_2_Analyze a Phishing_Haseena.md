
# Task 2 – Phishing Email Analysis Report

## 📌 Objective

Analyze a suspicious email and identify phishing indicators using email header analysis and file scanning tools.

---

## 📧 Sample Email Analyzed

- **Subject**: Security alert
- **From**: Google <no-reply@accounts.google.com>
- **To**: haseena8102003@gmail.com
- **Date**: May 27, 2025
- **File Name**: `Security alert.eml`

---

## 🔍 Email Header Analysis

Header was analyzed using [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)

| Security Protocol | Status | Notes |
|--------------------|--------|-------|
| **SPF** (Sender Policy Framework) | ✅ Pass | Email sent from a verified Google IP: `209.85.220.73` |
| **DKIM** (DomainKeys Identified Mail) | ✅ Pass | Signed by `accounts.google.com` |
| **DMARC** (Domain-based Message Authentication) | ✅ Pass | Fully aligned with sender domain |

🟢 **Result**: All header checks passed. No spoofing or forgery detected.

📎 **Screenshot**: `Screenshot_2025-05-27_112904.png`

---

## 🧪 VirusTotal Scan

- **File Scanned**: `Security alert.eml`
- **Size**: 11.9 KB
- **Tool Used**: [VirusTotal Email Scanner](https://virustotal.com)
- **Scan Result**: ✅ 0/63 antivirus engines flagged it

📎 **Screenshot**: `Screenshot_2025-05-27_113040.png`

---

## 🧠 Content Inspection

- **Content Summary**: Notification about Microsoft apps & services being granted access to the user’s Google Account.
- **Call to Action**: “Check activity” button links to `accounts.google.com` — a legitimate Google domain.
- **Tone**: Informative and non-threatening.
- **Language**: No spelling or grammatical errors detected.

---

## ✅ Conclusion

After careful inspection of the email headers, links, and content, this email appears to be a **genuine security alert** sent from Google. It is **not a phishing attempt**, and it passed all major authentication checks.

---

## 🛠 Tools Used

- ✅ [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- ✅ [VirusTotal File Scanner](https://virustotal.com)
- ✅ Manual link inspection and verification

---

## 📁 Repository Contents

```
task-2-phishing-analysis/
│
├── README.md
├── Security alert.eml
├── Screenshot_2025-05-27_112904.png
└── Screenshot_2025-05-27_113040.png
```

---

