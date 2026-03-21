# Exercise 03 — GDPR Violation & Ethical Analysis
## Real Case: Dedalus Biologie — CNIL Deliberation SAN-2022-012

> **Academic Context**
> Produced as part of the **Women4Cyber CyberAgents Programme (EQF Level 6)**
> [![Women4Cyber](https://img.shields.io/badge/Women4Cyber-CyberAgents_EQF6-purple)](https://platform.cyberagents.eu)
>
> Real case — Official CNIL sanction: **1,500,000 euros — April 12, 2022**

---

## 1. Case Overview

**Dedalus Biologie** is a French subsidiary of Dedalus Group,
Europe's leading healthcare software provider. It develops
Laboratory Information Management Systems (LIMS) used by
private medical laboratories across France.

In its capacity as a **data processor** (GDPR Article 28),
Dedalus handled sensitive health data on behalf of its
laboratory clients.

|
 Indicator 
|
 Data 
|
|
-----------
|
------
|
|
 Patients affected 
|
**
491,939
**
|
|
 GDPR Status 
|
 Data Processor — Article 28 
|
|
 Sanction 
|
**
1,500,000 euros
**
|
|
 Authority 
|
 CNIL (France) 
|
|
 Decision reference 
|
 SAN-2022-012 
|
|
 Date 
|
 April 12, 2022 
|

---

## 2. Timeline of Events

```
2015-2019 → Data migrations during software transitions
             in client laboratories

Feb 2021  → Security researchers discover a database
             containing sensitive medical data
             exposed on the internet — no authentication required

Feb 2021  → Alert reported by cybersecurity media "Zataz"
             and picked up by national press

Mar 2021  → CNIL opens formal investigation

Apr 2022  → CNIL issues 1,500,000 euros fine
             Decision made public
```

---

## 3. Established Facts

The CNIL investigation established the following:

- **491,939 patients** data freely accessible on the internet
- Data included: **full name, social security number,
  prescribing physician, laboratory name, pathologies,
  medications, medical comments**
- Data was stored **without any encryption** on the server
- The server required **no authentication** to access
- Data originated from migrations conducted **between 2015 and 2019**
  and had never been deleted
- Files contained data **beyond the scope** of what clients
  had instructed Dedalus to process

---

## 4. GDPR Violations Identified

### Article 5(1)(f) — Integrity and Confidentiality
Storing nearly 500,000 patient health records without
encryption or access controls constitutes a direct
violation of the fundamental principle of data security.

### Article 5(1)(e) — Storage Limitation
Data from migrations conducted between 2015 and 2019
was still present on the server in 2021 — years after
any legitimate purpose had expired.

### Article 5(1)(c) — Data Minimisation
Files contained information beyond what clients had
requested, violating the principle that data should be
limited to what is strictly necessary.

### Article 28 — Processor Obligations
As a data processor, Dedalus was required to act
**only on documented instructions** from its controller
clients. Processing data beyond those instructions,
and retaining it without authorisation, constitutes
a serious breach of processor obligations.

### Article 32 — Security of Processing

| Security Failure | Description |
|-----------------|-------------|
| No encryption | Data stored in plain text |
| No authentication | Server publicly accessible |
| No network segmentation | Migration data mixed with active data |
| No purge procedure | No automated deletion post-migration |
| Real data used in testing | Production data used for technical tests |

---

## 5. Ethical Analysis

### Betrayal of Medical Confidentiality
Medical confidentiality is one of the oldest ethical
principles in healthcare. Patients submitting to biological
analyses share their most intimate health information
in a context of absolute trust. Dedalus, as a technical
intermediary, held that trust by delegation — and
its negligence constituted a fundamental ethical breach.

### Absence of Privacy by Design Culture
Article 25 GDPR enshrines **Privacy by Design** —
security must be integrated from the outset, not added
as an afterthought. The accumulation of failures at
Dedalus (no encryption, no purge procedure, no security
audit) reflects a structural deficit in data protection
culture, not a single isolated error.

### Vulnerability of the Persons Concerned
The exposed data could identify patients with
potentially stigmatising conditions:
- HIV and sexually transmitted infections
- Mental health conditions
- Chronic diseases

Potential consequences for affected patients included
employment discrimination, insurance refusals,
and serious psychological harm — all irreversible.

---

## 6. CNIL Sanction Analysis

The 1,500,000 euros fine reflected the following factors:

| Aggravating Factor | Impact |
|-------------------|--------|
| Sensitive health data | Significant increase |
| Scale (491,939 persons) | Major increase |
| Duration of exposure | Increase |
| Multiple simultaneous violations | Increase |
| Absence of basic preventive measures | Increase |

| Mitigating Factor | Impact |
|------------------|--------|
| Cooperation with CNIL | Reduction |
| Corrective measures implemented | Reduction |

---

## 7. Corrective Recommendations

### 1. Automated Post-Migration Data Deletion
Deploy an automated deletion procedure for all
temporary migration files within **30 days** of
completion, with formal sign-off documentation.

### 2. Systematic Encryption
Implement **AES-256 encryption** for all health data
at rest and in transit, aligned with HDS certification
requirements and ANSSI guidelines.

### 3. Revise Subcontracting Contracts
Update all client contracts to precisely define:
- Authorised data categories
- Strict retention periods
- Audit clauses for compliance verification

### 4. Mandatory Staff Training
Deploy annual GDPR training for all technical staff
handling health data, covering processor obligations
under Article 28 and security requirements under Article 32.

---

## References

- **CNIL, Deliberation SAN-2022-012, April 12, 2022**
  https://www.legifrance.gouv.fr/cnil/id/CNILTEXT000045631355
- GDPR (EU) 2016/679 — Articles 5, 9, 25, 28, 32, 83
- French Public Health Code — Articles L1110-4, L1111-8
- ANSSI (2021). *Guide de securite des donnees de sante*
- EDPB (2021). *Guidelines on controller and processor concepts*
- Zataz.com (February 2021). *Fuite massive de donnees medicales francaises*
- Le Monde (March 2021). *Des donnees medicales de 491 000 Francais exposees*

