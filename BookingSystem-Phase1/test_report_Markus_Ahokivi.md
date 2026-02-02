# 1️⃣ Introduction

**Tester(s):**  
- Name: Markus Ahokivi

**Purpose:**  
- Identifying vulnerabilities on a Booking System (WEB)


**Test environment & dates:**  
- Start: 9:00 AM 2/2/2026
- End:  10:00 AM 2/2/2026
- Test environment details: SQL, WEB, ZAP

**Assumptions & constraints:**  
- New devices and applications
- Limited time and resurces

---

# 2️⃣ Executive Summary

**Short summary (1-2 sentences):**  

**Overall risk level:** (Low / Medium / High / Critical)

**Top 5 immediate actions:**  
1.  Path Traversal - Acces to files, directories, commands etc
2.  SQL Injection - Acces is possible
3.  Absence of Anti-CSRF Tokens - No token on html
4.  Content Security Policy (CSP) Header Not Set - Layer of security 	
5.  Format String Error - submitted data of an input string is evaluated as a command by the application

---

# 3️⃣ Severity scale & definitions

|  **Severity Level**  | **Description**                                                                                                              | **Recommended Action**           |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
|      🔴 **High**     | Path Traversal | *Immediate fix required* - Reject any input that does not strictly conform to specifications        |
|     🟠 **Medium**    | Absence of Anti-CSRF Tokens                              | *Fix ASAP* - Ensure that your web server, application server, load balancer, etc|
|      🟡 **Low**      |   Application Error Disclosure                                                 | *Fix soon* -       Review the source code of this page. Implement custom error pages                 |
| 🔵 **Info** | No direct risk - User Agent Fuzzer                                 | *Monitor and fix in maintenance* - Check for differences|


---

# 4️⃣ Findings (filled with examples → replace)

> Fill in one row per finding. Focus on clarity and the most important issues.

| ID | Severity | Finding | Description | Evidence / Proof |
|------|-----------|----------|--------------|------------------|
| F-01 | 🔴 High | SQL Injection in registration | Input field allows `' OR '1'='1` injection | Screenshot or sqlmap result |
| F-02 | 🟠 Medium | Session fixation | Session ID remains unchanged after login | Burp log or response headers |
| F-03 | 🟡 Low | Weak password policy | Accepts passwords like "12345" | Screenshot of registration success |

---

> [!NOTE]
> Include up to 5 findings total.   
> Keep each description short and clear.

---

# 5️⃣ OWASP ZAP Test Report (Attachment)

**Purpose:**  
- Attach or link your OWASP ZAP scan results (Markdown format preferred).

---

**Instructions:**
1. Check lecture recordings
2. Save the report as `zap_report_round1.md` and link it below.

---
> [!NOTE]
> 📁 **Attach full report:** → `check itslearning` → **Add a link here**

---
