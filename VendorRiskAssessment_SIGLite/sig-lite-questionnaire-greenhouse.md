# SIG Lite Vendor Questionnaire — Greenhouse

**Assessment Type:** Public documentation review  
**Vendor:** Greenhouse  
**Service:** Applicant Tracking System (ATS) and recruitment platform  
**Primary Data Types:** Personal data, candidate profiles, employment history, contact information  
**Risk Level:** High — vendor handles PII and supports hiring operations  
**Scope of review:** Security posture, privacy handling, availability, and dependency risk based on publicly available material

---

## 1. Governance & Risk Management

| Question | Greenhouse Response | Evidence Source | Risk Rating (0–4) |
|----------|---------------------|----------------|-------------------|
| Does the vendor maintain formal security governance? | Yes — governance and control oversight are supported through recurring independent audits | https://www.greenhouse.com/security | 4 |
| Does the vendor hold relevant certifications (e.g., ISO 27001 / SOC 2)? | Yes — ISO 27001 and SOC 2 Type II certifications are maintained | https://www.greenhouse.com/security | 4 |
| Does the vendor maintain an ISMS or equivalent? | Yes — confirmed through ISO 27001 certification | https://www.greenhouse.com/security | 4 |
| Are incident response processes documented and tested? | Yes — these practices fall under audit scope, though operational specifics aren’t publicly detailed | https://www.greenhouse.com/security | 3 |
| Does the vendor perform employee background checks? | Yes — indicated as part of security expectations for handling sensitive data | https://www.greenhouse.com/security | 3 |
| Does the vendor assess subcontractors or critical third parties? | Yes — subprocessors are listed and monitored as part of compliance expectations | https://www.greenhouse.com/security | 3 |

---

## 2. Data Security & Privacy

| Question | Response | Evidence Source | Risk Rating |
|----------|---------|----------------|------------|
| Is customer data encrypted in transit? | Yes — TLS encryption in transit is standard | https://www.greenhouse.com/security | 4 |
| Is customer data encrypted at rest? | Yes — data-at-rest encryption confirmed | https://www.greenhouse.com/security | 4 |
| Does the vendor support data deletion requests? | Yes — deletion workflows available through GDPR tooling | https://support.greenhouse.io | 4 |
| Does the vendor support configurable data retention? | Yes — retention can be configured to support compliance needs | https://support.greenhouse.io | 4 |
| Does the vendor comply with GDPR? | Yes — guidance and controls are provided for customer compliance | https://support.greenhouse.io | 4 |
| Does the platform support EU data residency? | Yes — EU data storage support is available | https://www.greenhouse.com/security | 3 |
| Are audit logs available to customers? | Yes — audit log access is supported via API | https://www.greenhouse.com/security | 3 |

---

## 3. Identity, Access & Authentication

| Question | Response | Evidence Source | Risk Rating |
|----------|---------|----------------|------------|
| Does the platform support SSO / SAML / SCIM? | Yes — identity integrations are supported | https://www.greenhouse.com/security | 4 |
| Does the vendor enforce MFA internally? | Likely yes — implied through certification controls, but not explicitly stated | https://www.greenhouse.com/security | 3 |
| Are role-based access controls supported? | Yes — granular permission controls are available | https://www.greenhouse.com/security | 3 |
| Are privileged accounts monitored? | Monitoring is assumed under audit expectations, but not publicly described | https://www.greenhouse.com/security | 3 |

---

## 4. Availability & Continuity

| Question | Response | Evidence Source | Risk Rating |
|----------|---------|----------------|------------|
| Does the vendor provide uptime SLAs? | Yes — enterprise deployments include uptime commitments | https://desking.app/greenhouse-ats-review | 3 |
| Is disaster recovery documented and tested? | Expected as part of ISO alignment, though specific testing details aren’t publicly listed | https://www.greenhouse.com/security | 3 |
| Are RPO/RTO objectives defined? | Likely defined internally to support certification expectations | https://www.greenhouse.com/security | 3 |
| Does the vendor provide availability transparency? | Yes — status reporting is publicly available | https://status.greenhouse.io | 3 |

---

## 5. Vendor Dependencies

| Question | Response | Evidence Source | Risk Rating |
|----------|---------|----------------|------------|
| Does the vendor disclose critical sub-processors? | Yes — list provided online | https://www.greenhouse.com/security | 3 |
| Are subcontractor controls assessed? | Yes — covered under compliance expectations, though details are not public | https://www.greenhouse.com/security | 3 |
| Can the vendor provide an updated subprocessor list on request? | Yes — list is published and maintained | https://www.greenhouse.com/security | 4 |

---

## 6. Summary Risk Rating

| Risk Area | Score (0–4) |
|-----------|-------------|
| Governance & Risk | 4 |
| Data Security & Privacy | 4 |
| Identity & Access | 3 |
| Availability & Continuity | 3 |
| Vendor Dependencies | 3 |

### **Overall Vendor Risk Rating:** **3.4 / 4 — Low to Moderate Risk**

Greenhouse demonstrates a mature security and privacy posture supported by established certifications. Key internal practices such as MFA enforcement and privileged access controls are reasonably assumed but not explicitly detailed in public material. These gaps are typical for SaaS vendors and can be clarified during onboarding or contractual review.

---

## 7. Follow-up Questions / Clarifications

| Area | Clarification Request |
|------|-----------------------|
| Identity & Access | Confirm internal enforcement of MFA for privileged users |
| Availability | Obtain high-level disaster recovery testing frequency |
| Privileged Access | Request summary of privileged account monitoring approach |
| Vendor Dependencies | Ask whether subcontractor reviews are performed annually |

---

## 8. Decision

| Vendor | Final Determination |
|--------|--------------------|
| Greenhouse | **Approved — subject to onboarding clarifications being addressed** |

**Rationale:**  
The vendor meets expected controls for handling personal and operationally sensitive data. Certification coverage and GDPR-aligned features indicate a strong baseline. Follow-up questions focus on validation of internal practices rather than remediation.

---

**Assessor:** Hilary Azimoh 
**Date:** 28-02-2025 
