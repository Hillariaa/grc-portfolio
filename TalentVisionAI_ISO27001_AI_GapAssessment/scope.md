# ISMS & AI Governance Scope – TalentVisionAI

## 1. Purpose

This document defines the scope of the ISO 27001:2022 and AI governance control gap assessment for TalentVisionAI, a fictional SaaS platform that uses machine learning models to score job applicants and recommend candidate shortlists to employers. 

The scope includes security, privacy, and AI-specific governance principles related to the design, development, deployment, and ongoing monitoring of the TalentVisionAI platform, aligned with ISO 27001:2022, ISO/IEC 42001 concepts, NIST AI RMF, GDPR profiling requirements and anticipated EU AI Act obligations.

---

## 2. Organization and Service Overview

**Organization:** TalentVisionAI (fictional)  
**Offering:** AI-driven HR screening and candidate ranking platform  
**Processing:** Personal data, employment history, CVs, candidate assessments, ranking recommendations, hiring scores

**Key characteristics:**
- The platform generates *automated ranking recommendations* that materially influence hiring decisions.
- The recommendation engine uses ML models trained on anonymized CV and hiring outcome datasets.
- Employers rely on ranking outputs to prioritize candidates, placing the system within **EU AI Act high-risk category** for employment.
- The system provides *explanations* of ranking decisions to hiring managers, partially satisfying transparency expectations.

---

## 3. ISMS Scope (ISO 27001)

The ISMS applies to:
- Design, development, deployment, and operation of TalentVisionAI’s SaaS platform
- Processing of personal and employment-related candidate data
- Storage, transmission, and confidentiality of training datasets and ranking outputs
- Internal systems used to administer production infrastructure
- Supporting operational workflows and incident handling
- Critical third-party services (cloud hosting, logging, messaging, model hosting middleware)

**In-scope components**
- SaaS application and APIs
- Model serving API layer
- AWS infrastructure (eu-west-1)
- Feature store and model registry
- Identity & access management
- CI/CD pipelines
- Internal developer workloads

**Out-of-scope for ISMS initial phase**
- Marketing website, CRM systems
- Experiments used for early research not deployed to production
- Legacy training pipelines no longer connected to live services

---

## 4. AI Governance Scope (ISO/IEC 42001 concepts, NIST AI RMF)

The AI governance scope applies to:
- ML and LLM-driven ranking models used in candidate scoring
- Training datasets, feature engineering, and model lifecycle controls
- Model monitoring related to performance drift, fairness, bias & adverse impact
- Explanation interfaces provided to hiring managers
- Decisions where recommendations materially influence hiring outcomes
- Profiling controls required under GDPR Articles 21 & 22

**Out-of-scope for AI governance initial phase**
- Experimental prototype models not connected to hiring decisions
- Synthetic data generation engines
- Benchmark/Pilot models used purely for research

---

## 5. Information Classification (high-level)

| Classification | Examples | Notes |
|----------------|---------|-------|
| Public | Marketing content | Release-ready content only |
| Internal | Non-sensitive docs, code comments | Shared internally |
| Confidential | Candidate identifiers, CVs, scoring outputs | **Primary risk category** |
| Restricted | Training datasets, lineage metadata, model artifacts | **High-risk; requires strongest controls** |

---

## 6. Assumptions

- The platform’s recommendation outputs **influence hiring decisions**, triggering GDPR & EU AI Act high-risk expectations.
- Bias, discrimination & fairness risks must be actively monitored and mitigated.
- ISO 27001 controls represent baseline security; AI-specific governance layers provide additional safeguards.
- Data processing locations remain in the EU unless cross-border transfers documented via SCCs.
- Final model decisions do not auto-reject applicants; humans retain decision authority.

---

## 7. Dependencies and Interfaces

| Dependency | Role |
|------------|------|
| AWS | Underlying infrastructure security (shared responsibility) |
| Model registry (e.g. MLflow) | Model versioning & metadata tracking |
| LLM summarization layer | CV parsing & transformation |
| HR applicant tracking systems | Integration targets & risk interfaces |
| Data labeling services | Potential source of embedded dataset bias |

---

## 8. Applicability Statement

All ISO 27001:2022 controls are considered for applicability.  
Additional AI controls are evaluated using:
- ISO/IEC 42001 concept alignment
- NIST AI RMF functions: Govern, Map, Measure, Manage
- GDPR profiling requirements for automated decision influence
- EU AI Act high-risk employment criteria

The combined control inventory feeds the **Annex A gap assessment**, **AI governance gap assessment**, and **remediation roadmap**.

---
