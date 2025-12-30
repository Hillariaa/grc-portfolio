# Statement of Applicability (SoA)
## TalentVisionAI — ISO 27001:2022 + AI Governance (ISO/IEC 42001 Concepts & NIST AI RMF)

### Purpose
This Statement of Applicability identifies the applicability and implementation status of ISO 27001:2022 Annex A controls and AI-specific governance controls derived from ISO/IEC 42001 concepts, NIST AI RMF functions (Govern, Map, Measure, Manage), GDPR profiling obligations, and the forthcoming EU AI Act. It supports risk treatment planning and certification readiness for TalentVisionAI’s ISMS and emerging AI governance program.

### Scope reference
This SoA applies to components, data types, processes, and decisions defined within:
- `scope.md` (ISMS and AI governance scope)
- TalentVisionAI’s AI-enabled HR ranking platform deployed in AWS eu-west-1
- High-risk AI system characteristics as defined by EU AI Act draft text

---

## 1. ISO 27001 Annex A Control Applicability (Selected Controls)

| Control ID | Control Name | Applicable? | Justification | Current Status |
|------------|--------------|-------------|---------------|----------------|
| A.5.1 | Policies for information security | Yes | Required to establish foundational security governance and demonstrate commitment to customers and auditors | Partially Implemented |
| A.5.7 | Threat intelligence | Yes | HR and payroll data are targets for emerging threats; structured intelligence supports preventive controls | Not Implemented |
| A.5.17 | Authentication information | Yes | Protects access to sensitive candidate and hiring data; reduces credential abuse | Implemented |
| A.5.21 | Data leakage prevention | Yes | Prevents unintentional or malicious disclosure of CVs and candidate rankings | Not Implemented |
| A.6.3 | Information security awareness and training | Yes | Human error can expose sensitive candidate information; training reduces risk | Partially Implemented |
| A.7.2 | Physical entry | Yes | Office access may expose systems used to administer production workloads | Partially Implemented |
| A.8.16 | Monitoring activities | Yes | Monitoring required to detect unauthorized access, privilege escalation, or model tampering | Not Implemented |
| A.8.18 | Use of cryptography | Yes | Encryption required to protect personal and sensitive data in transit and at rest | Implemented |
| A.8.28 | Secure coding | Yes | Vulnerabilities in ranking logic or APIs could undermine confidentiality, integrity, or fairness | Partially Implemented |

**Non-applicable ISO examples**

| Control ID | Control Name | Applicable? | Justification | Current Status |
|------------|--------------|-------------|---------------|----------------|
| A.7.5 | Secure disposal | No | Physical media not used in production; AWS manages secure disposal | N/A |
| A.7.7 | Storage media | No | No removable media in use; AWS protections apply | N/A |

---

## 2. AI Governance Control Applicability

| Control ID | Control Name | Applicable? | Justification | Current Status |
|------------|--------------|-------------|---------------|----------------|
| AI-G1 | AI Risk Governance Roles | Yes | Defined accountability is required to manage risks of high-impact automated recommendations | Partially Implemented |
| AI-G2 | Model Lifecycle Documentation | Yes | Model lineage and documentation support transparency, reproducibility, and governance | Partially Implemented |
| AI-G3 | Human-in-the-Loop Oversight | Yes | Recommendations influence hiring processes; human oversight required for meaningful decision authority | Implemented |
| AI-G4 | Data Lineage & Provenance | Yes | Traceability is required for challenging outcomes and responding to appeals | Partially Implemented |
| AI-G5 | High-Risk System Registration | Yes | EU AI Act identifies employment-related AI as high-risk; registration supports conformity preparation | Not Implemented |
| AI-D1 | Dataset Quality Requirements | Yes | Data quality directly affects ranking fairness and accuracy | Partially Implemented |
| AI-D2 | Bias Identification & Mitigation | Yes | Automated ranking without bias controls may violate fairness expectations and GDPR Article 5 | Not Implemented |
| AI-D3 | Sensitive Attribute Handling | Yes | Direct or proxy bias must be limited to prevent discriminatory outcomes | Partially Implemented |
| AI-M1 | Explainability & Transparency | Yes | Hiring managers and candidates require understanding of automated recommendations | Partially Implemented |
| AI-M2 | Adverse Impact Monitoring | Yes | Unequal model impact may create systemic discrimination without detection | Not Implemented |
| AI-M3 | Model Drift Detection & Retraining | Yes | Accuracy and fairness degrade over time without drift monitoring; impacts hiring practices | Not Implemented |
| AI-M4 | Model Versioning & Approval Gates | Yes | Version control required for safety, reproducibility, and release accountability | Implemented |
| AI-M5 | Attack & Manipulation Resistance | Yes | Model manipulation or data poisoning could bias rankings or introduce fraud | Not Implemented |
| AI-U1 | User Dispute & Appeal Mechanisms | Yes | Candidates must be able to contest algorithmic outcomes under GDPR profiling expectations | Not Implemented |
| AI-U2 | Human Override Capability | Yes | Overrides required to ensure meaningful human control; prevents fully automated rejection | Implemented |

---

## 3. Non-Applicable AI Controls
*(optional for future expansion — none required at this stage)*

No AI controls are considered non-applicable, as all identified controls relate to current or anticipated risk, regulatory alignment, and operational expectations.

---

## 4. Relationship to Remediation
Controls with **Partially Implemented** and **Not Implemented** statuses drive remediation actions in the combined roadmap. High-priority actions align to:
- candidate fairness and non-discrimination risks
- ISO certification readiness
- EU AI Act conformity expectations
- reduction of security and privacy exposures

---

## 5. Approval (Portfolio Simulation)

| Role | Name | Date |
|------|------|------|
| Information Security & AI Governance Analyst | Hilary Azimoh | 11-02-2025 |
| CTO (Fictional) | Jane Doe | 11-02-2025 |

---
