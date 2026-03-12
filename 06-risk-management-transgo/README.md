🚛 Risk Management & Security Governance
## Case Study: TransGo Global

> 🎓 **Academic Context**
> Produced as part of the **Women4Cyber CyberAgents Programme (EQF Level 6)**
> [![Women4Cyber](https://img.shields.io/badge/Women4Cyber-CyberAgents_EQF6-purple)](https://platform.cyberagents.eu/en/higherEductation/23b2af04-aa11-4c9c-8ce0-e2d52e19b3c1?difficultyLevel=EQF+6)
>
> ⚠️ **Disclaimer:** TransGo Global is a **fictional company**
> created for educational purposes. All analysis and recommendations
> are original work based on real frameworks (ISO 27001, NIST CSF, GDPR).

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
 TransGo Global (fictional) 
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
|
**
Word Count
**
|
 ~1,600 words 
|

---

## 📄 Table of Contents

1. [Executive Summary](#1-executive-summary)
2. [Organisational Context](#2-organisational-context)
3. [Current Governance Weaknesses](#3-current-governance-weaknesses)
4. [Risk Analysis & Risk Matrix](#4-risk-analysis--risk-matrix)
5. [Governance Improvement Recommendations](#5-governance-improvement-recommendations)
6. [Implementation Roadmap](#6-implementation-roadmap)
7. [Conclusion](#7-conclusion)
8. [References](#references)

---

## 1. Executive Summary

This report presents a cybersecurity risk and governance analysis for
**TransGo Global**, a fast-growing international logistics company
undergoing rapid digital transformation. The company has significantly
expanded its use of IoT sensors, cloud platforms, and remote operations
to support its global supply chain activities.

A recent internal audit revealed critical weaknesses in the company's
security governance structure, including:

- ❌ Unclear roles and responsibilities for cybersecurity decisions
- ❌ No formal escalation protocols for security incidents
- ❌ Legacy VPN protocols creating exploitable vulnerabilities
- ❌ Absence of a dedicated CISO function
- ❌ No formal risk register or risk treatment process

This report identifies the key risks associated with these governance
gaps, proposes a set of prioritised corrective measures, and presents
a simplified risk matrix to support decision-making by the
**Security Steering Committee**.

---

## 2. Organisational Context

### About TransGo Global

TransGo Global is an international logistics company operating across
**24 countries**, managing complex supply chains for manufacturing,
retail, and pharmaceutical clients. The company has undergone
significant digital transformation over the past three years:

|
 Capability 
|
 Current State 
|
|
-----------
|
---------------
|
|
**
IoT Sensors
**
|
 12,000+ connected devices across warehouses 
|
|
**
Cloud Platforms
**
|
 AWS and Azure — partially migrated 
|
|
**
Remote Operations
**
|
 60% of staff working remotely or hybrid 
|
|
**
Legacy Systems
**
|
 Multiple outdated VPN and on-premise systems 
|
|
**
Third-party Integrations
**
|
 80+ supplier and partner API connections 
|
|
**
Data Processed
**
|
 Client shipment data, financial records, personal data 
|

### Current Governance Structure

## 3. Current Governance Weaknesses

### 3.1 Absence of Clear Accountability

The most critical governance weakness identified is the
**absence of clearly defined cybersecurity accountability**.
Security responsibilities are informally distributed across
the IT Director, the Compliance Officer, and individual
business unit managers — with no single owner.

This creates a dangerous situation known as the
**"accountability gap"**: when an incident occurs,
no one has the authority or mandate to make rapid decisions,
slowing response times and amplifying damage.

> *"Organisations that lack a designated security leader
> take on average 74 days longer to identify and contain
> a data breach."*
> — IBM Cost of a Data Breach Report 2023

### 3.2 Legacy VPN Vulnerabilities

TransGo Global still operates **legacy VPN protocols**
(PPTP and L2TP without IPSec) for remote access to
operational systems. These protocols have known
cryptographic vulnerabilities:

- **PPTP**: Broken encryption — vulnerable to brute-force
  attacks in under 24 hours
- **L2TP without IPSec**: No encryption — traffic
  transmitted in plain text

With 60% of staff working remotely, these legacy protocols
represent the **primary attack surface** for threat actors
seeking to access internal logistics systems and client data.

### 3.3 No Formal Incident Escalation Protocol

No documented escalation procedure exists for cybersecurity
incidents. In the event of a ransomware attack or data breach:

- Who decides to isolate affected systems?
- Who notifies clients?
- Who contacts law enforcement?
- Who communicates to the Board?
- Who triggers the GDPR 72-hour notification to supervisory authorities?

These questions currently have no formal answers —
a situation that could transform a manageable incident
into a catastrophic one.

### 3.4 IoT Security Governance Gap

The rapid deployment of 12,000+ IoT sensors across
warehouse operations has not been accompanied by a
corresponding security governance framework:

- No inventory of connected devices
- No patch management process for IoT firmware
- Default factory credentials still active on multiple devices
- No network segmentation between IoT devices and
  core business systems

---

## 4. Risk Analysis & Risk Matrix

### 4.1 Risk Identification

| Risk ID | Risk Description | Source |
|---------|-----------------|--------|
| R-01 | Ransomware via legacy VPN exploitation | Threat actor |
| R-02 | Unauthorised access through IoT devices | External attacker |
| R-03 | Data breach due to governance accountability gap | Internal/External |
| R-04 | GDPR non-compliance due to absence of breach protocol | Regulatory |
| R-05 | Supply chain attack via third-party API | External attacker |
| R-06 | Operational disruption from unpatched systems | Technical failure |

### 4.2 Simplified Risk Matrix
text
     IMPACT
          Low        Medium       High      Critical
     ┌──────────┬────────────┬──────────┬──────────┐
High │          │    R-06    │   R-03   │   R-01   │
     ├──────────┼────────────┼──────────┼──────────┤

## 7. Conclusion

TransGo Global faces a critical governance inflection point.
The combination of rapid digital transformation, legacy
technical vulnerabilities, and structural accountability gaps
creates a risk profile that demands immediate executive action.

The recommendations presented in this report are prioritised
by risk severity and operational feasibility. The most urgent
actions — appointing a CISO, disabling legacy VPN protocols,
and establishing an incident response plan — can be initiated
within days and require minimal budget compared to the
potential cost of a major incident.

**To put the financial case in perspective:**

| Scenario | Estimated Cost |
|----------|---------------|
| Implementing all recommendations | €150,000 – €250,000 |
| Average ransomware incident (logistics sector) | €2.5M – €8M |
| GDPR fine (Article 83 — serious breach) | Up to 4% global turnover |
| Operational disruption (72h downtime) | €500,000 – €2M |

> **The cost of governance is a fraction of the cost
> of a governance failure.**

The Security Steering Committee is requested to approve
the immediate actions outlined in this report and to
schedule a follow-up governance review in **30 days**.

---

## References

- **ISO/IEC 27001:2022** — Information Security Management Systems
- **ISO/IEC 27002:2022** — Controls 5.15–5.26 (Governance & Access)
- **NIST Cybersecurity Framework 2.0** (2024)
- **ENISA Threat Landscape 2023** — European Union Agency for Cybersecurity
- **ENISA IoT Security Guidelines 2023**
- **GDPR (EU) 2016/679** — Articles 28, 32, 33
- **NIS2 Directive (EU) 2022/2555** — Article 21
- **IBM Cost of a Data Breach Report 2023**
- **Verizon DBIR 2023** — Data Breach Investigations Report

---

> **Author's note:** This report is an original academic deliverable
> produced as part of the Women4Cyber CyberAgents Programme (EQF Level 6).
> It demonstrates applied competencies in cybersecurity risk management,
> security governance, and professional report writing.

