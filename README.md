# Lifestyle Store VAPT Report 🔒  

## Problem Statement 📋  
As part of a practical ethical hacking exercise, the objective is to test a real-life e-commerce platform for vulnerabilities and loopholes.  
The tasks include:  
- Identifying all possible vulnerabilities in the system.  
- Collecting proofs of concept (PoCs) for each vulnerability.  
- Preparing a detailed developer-level report that includes:  
  - Title of the vulnerability.  
  - A short description.  
  - The exact vulnerable URL.  
  - Affected parameters (GET, POST, Cookie, Header, etc.).  
  - Payload used to trigger the vulnerability.  
  - Steps to replicate the exploit with PoCs.  
  - Business impacts of the vulnerabilities.  
  - Recommendations to fix them.  
  - References to reputed sources for each vulnerability.  

The application contains 28 deliberately introduced vulnerabilities, including but not limited to:  
- **SQL Injection**  
- **Reflected and Stored Cross-Site Scripting (XSS)**  
- **Insecure Direct Object Reference (IDOR)**  
- **Rate Limiting Issues**  
- **Insecure File Uploads**  
- **Weak Passwords**  
- **Open Redirection**  
- **Command Execution Vulnerabilities**  
- **Cross-Site Request Forgery (CSRF)**  

The goal is to identify and report these vulnerabilities while providing actionable recommendations to secure the system.  

---

## Introduction 📋  
This repository contains a comprehensive Vulnerability Assessment and Penetration Testing (VAPT) report for the **"Lifestyle Store"** website. The report identifies critical security vulnerabilities and provides detailed analysis, proofs of concept, business impacts, and expert recommendations to mitigate the risks.

---

## Key Vulnerabilities Identified 🛡️  
1. **SQL Injection (Critical)** 🚨  
   - 🔗 Vulnerable URLs and parameters.  
   - 🛑 Risk: Complete access to database and user credentials exposure.  

2. **Account Takeover via OTP Bypass (Critical)** 🔑  
   - 🚪 OTP brute force vulnerabilities.  
   - 🚨 Risk: Admin account compromise.  

3. **Insecure Direct Object Reference (IDOR) (Critical)** 🔍  
   - 📂 Access to other users' details.  
   - ⚠️ Risk: Information leakage and phishing attacks.  

4. **Cross-Site Scripting (XSS) (Severe)** 💻  
   - ⚔️ Multiple reflected XSS vulnerabilities.  
   - 🛑 Risk: Phishing and user data theft.  

5. **Directory Listings (Severe)** 📂  
   - 📜 Exposed sensitive directories and files.  
   - 🔓 Risk: Admin panel compromise.  

6. **Information Disclosure (Low)** ℹ️  
   - 🛠️ Server details exposure.  
   - 🔧 Risk: Server mapping for further attacks.  

7. **Personally Identifiable Information (PII) Leakage (Critical)** 🛡️  
   - 📁 Exposed sensitive user data.  
   - 🚨 Risk: Phishing and malicious file uploads.  

8. **Misconfigured Blog Site** 📝  
   - ⚔️ Temporary XSS and admin account access.  
   - 💣 Risk: Full site takeover.  

---

## Business Impact 📉  
The identified vulnerabilities can lead to severe consequences, including:  
- 🛡️ Data breaches exposing sensitive customer information.  
- 🔓 Full server compromise resulting in operational disruption.  
- 💸 Financial losses and reputational damage.  

---

## Recommendations 🛠️  
- ✅ Use prepared statements to prevent SQL Injection.  
- 🛡️ Apply rate limiting and enhance OTP security.  
- 🔒 Enforce strict access control mechanisms to prevent IDOR.  
- 🧹 Sanitize and encode all user inputs to mitigate XSS.  
- 📂 Disable directory listings and restrict access to sensitive files.  
- 🔑 Encrypt PII and ensure secure storage.  

---

## References 📚  
- [OWASP SQL Injection](https://owasp.org/www-community/attacks/SQL_Injection)  
- [OWASP XSS](https://owasp.org/www-community/attacks/xss/)  
- [Burp Suite](https://portswigger.net/burp)  




---

**Note:** This report is intended for educational and awareness purposes only. 🚫 Unauthorized penetration testing or exploitation of vulnerabilities is strictly prohibited.  
