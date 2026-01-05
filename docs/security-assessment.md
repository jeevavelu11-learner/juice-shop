# OWASP Juice Shop - Security Compliance Assessment

## Purpose
This document assesses the security posture of OWASP Juice Shop.  
**Note:** The application is **intentionally insecure** and should never be used in production.

## Compliance with Standards
- **OWASP Top 10 (2021 & later versions)**:  
  The app deliberately covers **all** categories of the OWASP Top 10 (and more) for training purposes.

- **OWASP ASVS (Application Security Verification Standard)**:  
  Many controls are missing or weakened on purpose to create challenges.

- **Other References**:  
  - OWASP API Security Top 10  
  - MITRE CWE  
  - OWASP Automated Threat Handbook

## Current Security Status
- **Intentionally Vulnerable Areas**: Broken Access Control, Cryptographic Failures, Injection (SQL/NoSQL), XSS, Insecure Deserialization, etc.  
- **Compliance Level**: 0% secure by design — this is expected behavior for a vulnerable training app.  
- **Recommendations for Real Applications**: Follow OWASP Cheat Sheets to mitigate each vulnerability demonstrated here.

## Risks
High – all major web application risks are present intentionally.

Version: Demo (January 2026)  
Author: [Jeeva]
