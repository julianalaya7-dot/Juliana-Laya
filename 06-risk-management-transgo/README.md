Risk Management & Security Governance
## Case Study: TransGo Global

---

> 🎓 **Academic Context**
> Produced as part of the **Women4Cyber CyberAgents Programme (EQF Level 6)**
> [![Women4Cyber](https://img.shields.io/badge/Women4Cyber-CyberAgents_EQF6-purple)](https://platform.cyberagents.eu/en/higherEductation/23b2af04-aa11-4c9c-8ce0-e2d52e19b3c1?difficultyLevel=EQF+6)

> ⚠️ **Disclaimer:** TransGo Global is a fictional company created for educational purposes.
> All analysis is based on real frameworks (ISO 27001, NIST CSF, GDPR).

---

## 📋 Assignment Details

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
Role
**
|
 Cybersecurity Risk Analyst 
|
|
**
Organisation
**
|
 TransGo Global 
*
(fictional)
*
|
|
**
Sector
**
|
 International Logistics 
|
|
**
Framework
**
|
 ISO/IEC 27001, NIST CSF 2.0 
|
|
**
Deliverable
**
|
 Risk Report to Security Steering Committee 
|

---

## 📁 Table of Contents

1. [Executive Summary](#1-executive-summary)
2. [Organisational Context](#2-organisational-context)
3. [Current Governance Weaknesses](#3-current-governance-weaknesses)
4. [Risk Analysis & Risk Matrix](#4-risk-analysis--risk-matrix)
5. [Recommendations](#5-recommendations)
6. [Implementation Roadmap](#6-implementation-roadmap)
7. [Conclusion](#7-conclusion)
8. [References](#references)

---

## 1. Executive Summary

**TransGo Global** is a logistics company that has grown fast digitally
but hasn't kept up with cybersecurity. A recent internal audit found
several serious gaps:

- ❌ No one is clearly in charge of cybersecurity decisions
- ❌ No plan exists if a cyberattack happens
- ❌ Old VPN systems that are easy to hack
- ❌ No dedicated security lead (CISO)
- ❌ No formal list of risks

This report explains the main risks and what the company should do
to fix them — presented to the **Security Steering Committee**.

---

## 2. Organisational Context

### About TransGo Global

TransGo Global operates in **24 countries** and manages supply chains
for manufacturing, retail, and pharmaceutical clients.
Over the last 3 years, the company has digitised rapidly:

|
 Capability 
|
 Current State 
|
|
------------
|
--------------
|
|
**
IoT Sensors
**
|
 12,000+ connected devices in warehouses 
|
|
**
Cloud
**
|
 AWS and Azure — not fully migrated yet 
|
|
**
Remote Work
**
|
 60% of staff work remotely or hybrid 
|
|
**
Legacy Systems
**
|
 Old VPN systems still in use 
|
|
**
Partners
**
|
 80+ supplier API connections 
|
|
**
Data
**
|
 Shipment data, financial records, personal data 
|

### Governance Today

> ⚠️ There is no formal security structure.
> Responsibilities are split between IT, Compliance, and managers
> — with **no single person in charge**.

---

## 3. Current Governance Weaknesses

### 3.1 Nobody Is Clearly in Charge

Security tasks are shared between the IT Director, the Compliance Officer,
and various managers. But no one has the final say.

When an incident happens, this creates confusion and delays —
what's called an **"accountability gap"**.

> *"Companies without a dedicated security leader take
> **74 days longer** to contain a data breach."*
> — IBM Cost of a Data Breach Report 2024

---

### 3.2 Old VPN Systems

The company uses **outdated VPN protocols** (PPTP and L2TP without IPSec)
that have known security flaws:

- 🔴 **PPTP** — can be cracked in under 24 hours
- 🔴 **L2TP without IPSec** — data travels with no encryption at all

With 60% of staff working remotely, this is the **biggest entry point**
for attackers right now.

---

### 3.3 No Incident Response Plan

If a ransomware attack or data breach happened today,
nobody knows:

- ❓ Who shuts down the affected systems?
- ❓ Who tells the clients?
- ❓ Who calls the authorities?
- ❓ Who informs the Board?
- ❓ Who sends the **GDPR notification within 72 hours**?

This lack of a plan could turn a bad situation into a crisis.

---

### 3.4 IoT Devices Left Unsecured

12,000+ IoT sensors were deployed without any security rules:

- No list of which devices exist
- No updates or patches for device software
- Many devices still use default passwords
- No separation between IoT devices and core business systems

---

## 4. Risk Analysis & Risk Matrix

### 4.1 Main Risks Identified

|
 Risk ID 
|
 Risk 
|
 Source 
|
|
---------
|
------
|
--------
|
|
 R-01 
|
 Ransomware through old VPN 
|
 Hacker 
|
|
 R-02 
|
 Hacker access via IoT devices 
|
 External 
|
|
 R-03 
|
 Data breach — no one in charge 
|
 Internal / External 
|
|
 R-04 
|
 GDPR fine — no breach plan 
|
 Regulatory 
|
|
 R-05 
|
 Supply chain attack via partner API 
|
 External 
|
|
 R-06 
|
 System failure from unpatched software 
|
 Technical 
|

---

### 4.2 Risk Matrix

|
 Likelihood ↓ / Impact → 
|
 Low 
|
 Medium 
|
 High 
|
 Critical 
|
|
--------------------------
|
-----
|
--------
|
------
|
----------
|
|
**
High
**
|
|
 R-06 
|
 R-03 
|
**
R-01
**
|
|
**
Medium
**
|
|
|
 R-02 
|
 R-05 
|
|
**
Low
**
|
|
 R-04 
|
|
|

> 🔴 **Act now:** R-01, R-05
> 🟠 **Act within 30 days:** R-02, R-03
> 🟡 **Act within 90 days:** R-04, R-06

---

## 5. Recommendations

### 🔴 Immediate — Week 1

- **Appoint an interim CISO**
  Someone needs to be officially in charge of security decisions

- **Replace old VPN systems**
  Switch to a modern Zero Trust solution (ex: Zscaler, Cloudflare)
  and enforce **two-factor authentication (MFA)** for all remote access

- **Create an Incident Response Team**
  A small team (5 people) with a clear plan:
  who does what if an attack happens

---

### 🟠 Short Term — Month 1

- **List all IoT devices and reset default passwords**
- **Separate IoT devices from the main network** (using VLANs)
- **Start a risk register** — a simple document tracking all known risks
- **Hold monthly security meetings** with the Steering Committee

---

### 🟡 Medium Term — Quarter 1

- **Start ISO 27001 certification process**
- **Review all 80+ partner connections** for security risks
- **Add cybersecurity clauses** to all supplier contracts

---

## 6. Implementation Roadmap

|
 Phase 
|
 When 
|
 What 
|
|
-------
|
------
|
------
|
|
**
Phase 1
**
|
 Week 1 
|
 Appoint CISO · Disable old VPN · Enable MFA · Form response team 
|
|
**
Phase 2
**
|
 Month 1 
|
 IoT inventory · Reset passwords · Network separation · Risk register 
|
|
**
Phase 3
**
|
 Month 1–3 
|
 Partner audit · Staff training · ISO 27001 gap analysis 
|
|
**
Phase 4
**
|
 Ongoing 
|
 Quarterly reviews · Security tests · Incident simulations 
|

---

## 7. Conclusion

TransGo Global is at a turning point.
The company has grown fast digitally — but its security hasn't kept up.

The good news: **the most critical fixes can be done in days**,
and they cost far less than doing nothing.

|
 Scenario 
|
 Cost 
|
|
----------
|
------
|
|
 Fixing everything now 
|
 €150,000 – €250,000 
|
|
 Average ransomware attack 
*
(logistics)
*
|
 €2.5M – €8M 
|
|
 GDPR fine 
*
(serious breach)
*
|
 Up to 4% of global turnover 
|
|
 72h system downtime 
|
 €500,000 – €2M 
|
|
**
If just 1 incident is avoided
**
|
**
ROI x15
**
|

> 💡 **Fixing security now costs a fraction of a single attack.**

The Security Steering Committee is asked to **approve immediate actions**
and schedule a follow-up review in **30 days**.

---

## 📚 References

- **ISO/IEC 27001:2022** → [iso.org](https://www.iso.org/standard/27001)
- **NIST Cybersecurity Framework 2.0** → [nist.gov](https://www.nist.gov/cyberframework)
- **ENISA Threat Landscape 2024** → [enisa.europa.eu](https://www.enisa.europa.eu/publications/enisa-threat-landscape-2024)
- **IBM Cost of a Data Breach 2024** → [ibm.com](https://www.ibm.com/security/data-breach)
- **ANSSI Panorama des menaces 2025** → [cyber.gouv.fr](https://cyber.gouv.fr/publications)
- **GDPR (EU) 2016/679** → [eur-lex.europa.eu](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32016R0679)
- **NIS2 Directive (EU) 2022/2555** → [eur-lex.europa.eu](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32022L2555)
- **Verizon DBIR 2024** → [verizon.com](https://www.verizon.com/business/resources/reports/dbir/)

---

> ✍️ **Author's note:** This is an academic deliverable produced as part of the
> **Women4Cyber CyberAgents Programme (EQF Level 6)**.
> It covers cybersecurity risk management and security governance.

