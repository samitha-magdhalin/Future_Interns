# Web Application Security Testing – Task 1

## Internship
Future Interns – Cyber Security Internship

## Target Application
OWASP Juice Shop (Localhost)

## Tools Used
- Kali Linux
- OWASP Juice Shop
- Web Browser

## Vulnerabilities Identified

### 1. SQL Injection
Description:
SQL Injection vulnerability was tested on the login page using manual input manipulation.

Payload Used:
' OR 1=1--

Impact:
Authentication bypass and unauthorized access.

Mitigation:
- Use prepared statements
- Validate user input
- Parameterized queries

---

### 2. Cross-Site Scripting (XSS)
Description:
XSS vulnerability was identified using the search functionality.

Payload Used:
<img src=x onerror=alert(1)>

Impact:
Execution of malicious JavaScript.

Mitigation:
- Encode user input
- Implement Content Security Policy (CSP)

---

## Conclusion
The application contains critical security flaws that can be exploited if not properly secured.

