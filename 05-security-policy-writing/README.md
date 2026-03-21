Exercise 05 — Access Control Policy
## BrightCloud Systems — Document Reference: BCS-POL-SEC-001

> 🎓 **Academic Context**
> Produced as part of the **Women4Cyber CyberAgents Programme (EQF Level 6)**
> [![Women4Cyber](https://img.shields.io/badge/Women4Cyber-CyberAgents_EQF6-purple)](https://platform.cyberagents.eu)
>
> ⚠️ **Disclaimer:** BrightCloud Systems is a **fictional company**
> created for educational purposes. This policy is an original
> professional deliverable based on ISO/IEC 27001:2022 and GDPR.

---

## Document Information

|
 Field 
|
 Details 
|
|
-------
|
---------
|
|
**
Title
**
|
 Access Control Policy 
|
|
**
Reference
**
|
 BCS-POL-SEC-001 
|
|
**
Version
**
|
 1.0 
|
|
**
Owner
**
|
 CISO 
|
|
**
Approved by
**
|
 CEO 
|
|
**
Created
**
|
 July 2024 
|
|
**
Next Review
**
|
 July 2025 
|
|
**
Classification
**
|
 Internal — Confidential 
|

---

## Context & Purpose

**BrightCloud Systems** is a cloud-based document management
company serving 500+ European SME clients.
A recent security audit identified the **absence of a formal
Access Control Policy**, creating significant risks:

- ❌ No controlled access to client data
- ❌ No access revocation procedure when staff leave
- ❌ Staff using personal cloud storage for work documents
- ❌ Unable to demonstrate GDPR or ISO 27001 compliance

This policy defines who can access what, under what conditions,
and for how long — aligned with **ISO/IEC 27001:2022**
and **GDPR Articles 5, 25 and 32**.

---

## Core Principles

### 1. Least Privilege
*ISO/IEC 27002:2022 — Control 5.15*

Every user receives **only the access strictly necessary**
for their role. No default access is granted.

Examples:
- A junior developer has no access to client production data
- A sales representative only sees their own client portfolio
- An accountant has no access to server logs

### 2. Separation of Duties
*ISO/IEC 27002:2022 — Control 5.17*

Sensitive functions are distributed between multiple people
to prevent conflicts of interest.

Examples:
- The person requesting access cannot approve it
- A developer cannot deploy to production alone

### 3. Traceability
All access to sensitive resources is **logged, timestamped
and auditable**.

### 4. Periodic Review
Access rights are **reviewed regularly** to ensure they
still reflect actual needs.

---

## Access Levels

|
 Level 
|
 Description 
|
 Examples 
|
 Approved By 
|
|
-------
|
-------------
|
---------
|
------------
|
|
**
1 — Standard
**
|
 Day-to-day tools 
|
 Email, Intranet 
|
 Direct Manager 
|
|
**
2 — Business
**
|
 Client data & business apps 
|
 BrightDocs, CRM 
|
 Manager + CISO 
|
|
**
3 — Sensitive
**
|
 Confidential data 
|
 HR, Finance 
|
 CISO + CEO 
|
|
**
4 — Admin
**
|
 System administration 
|
 Servers, databases 
|
 CISO only 
|

---

## Key Rules

### Authentication
- ✅ **MFA mandatory** for all Level 2, 3 and 4 access
- ✅ **MFA mandatory** for all remote access
- ✅ Minimum **12-character passwords** with complexity requirements
- ❌ No password sharing — ever
- ❌ No generic passwords (admin, Password1, etc.)

### Remote Work
- ✅ **VPN mandatory** for all access outside office network
- ✅ Company-provided devices only
- ❌ No personal cloud storage:
  Google Drive, Dropbox, WeTransfer — **strictly forbidden**
- ❌ No unsecured public WiFi without active VPN

### Third Parties & Contractors
- ✅ NDA + Data Processing Agreement (GDPR Art. 28)
  required before any access
- ✅ Access limited to mission scope only
- ✅ Automatic revocation at contract end

---

## Access Revocation

|
 Trigger 
|
 Deadline 
|
 Process 
|
|
---------
|
---------
|
---------
|
|
 Employee departure 
|
**
4 hours
**
|
 HR notifies IT + CISO same day 
|
|
 Disciplinary suspension 
|
**
Immediate
**
|
 HR + CEO instruction 
|
|
 Suspected compromise 
|
**
Immediate
**
|
 CISO or IT alert 
|

---

## Periodic Access Reviews

|
 Frequency 
|
 Scope 
|
 Responsible 
|
|
-----------
|
-------
|
-------------
|
|
 Monthly 
|
 Admin accounts (Level 4) 
|
 CISO + IT 
|
|
 Quarterly 
|
 Sensitive access (Level 3) 
|
 CISO + Managers 
|
|
 Semi-annual 
|
 All active access rights 
|
 CISO + HR + Managers 
|
|
 Annual 
|
 Full access matrix audit 
|
 CISO + Internal Audit 
|

---

## Non-Compliance

|
 Level 
|
 Examples 
|
 Consequences 
|
|
-------
|
---------
|
-------------
|
|
 Minor 
|
 Non-compliant password 
|
 Reminder + training 
|
|
 Moderate 
|
 Credential sharing, personal cloud use 
|
 Written warning 
|
|
 Serious 
|
 Deliberate unauthorised access 
|
 Disciplinary action 
|
|
 Critical 
|
 Data exfiltration 
|
 Dismissal + legal action 
|

---

## References

- ISO/IEC 27001:2022 — Controls 5.15-5.18
- ISO/IEC 27002:2022 — Implementation guidelines
- GDPR (EU) 2016/679 — Articles 5(1)(f), 25, 32
- NIS2 Directive (EU) 2022/2555 — Article 21
- ANSSI (2021). *Recommandations relatives à l'administration sécurisée des SI*
- CNIL (2023). *Guide de la sécurité des données personnelles*
