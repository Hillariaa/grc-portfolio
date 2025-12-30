# SIG Lite Vendor Questionnaire — Stripe

**Assessment Type:** Public documentation review  
**Vendor:** Stripe  
**Service:** Payment processing and financial data services  
**Primary Data Types:** Cardholder data, transaction details, PII  
**Risk Level:** High — vendor processes sensitive financial and personal data

---

## 1. Governance & Risk Management

| Question | Stripe Response | Evidence Source | Risk Rating (0–4) |
|----------|-----------------|----------------|-------------------|
| Does the vendor maintain formal security governance? | Yes — regular independent audits for SOC 1 & SOC 2 | https://docs.stripe.com/security | 4 |
| Does the vendor hold relevant certifications (e.g., ISO 27001 / SOC 2)? | Yes — SOC 1 and SOC 2 Type II compliance | https://docs.stripe.com/security | 4 |
| Does the vendor maintain an ISMS or equivalent? | Yes — scope implied by audit controls | https://docs.stripe.com/security | 4 |
| Are incident response processes documented and tested? | Likely — part of audit scope, though not public | https://docs.stripe.com/security | 3 |
| Does the vendor assess subcontractors or critical third parties? | Yes — sub-processor list and due diligence described | https://stripe.com/legal/service-providers | 3 |

---

## 2. Data Security & Privacy

| Question | Response | Evidence Source | Risk Rating |
|----------|----------|----------------|------------|
| Is customer data encrypted in transit? | Yes — TLS/SSL encryption enforced | https://docs.stripe.com/security | 4 |
| Is customer data encrypted at rest? | Yes — implied by PCI Level 1 requirements | https://docs.stripe.com/security | 4 |
| Does the vendor support data deletion requests? | Yes — privacy center outlines data rights | https://stripe.com/legal/privacy-center | 4 |
| Does the vendor comply with GDPR? | Yes — privacy policies & controls align with GDPR | https://stripe.com/legal/privacy-center | 4 |
| Are audit logs available to customers? | Likely available via API though not public | https://docs.stripe.com/security | 3 |

---

## 3. Identity, Access & Authentication

| Question | Response | Evidence Source | Risk Rating |
|----------|----------|----------------|------------|
| Does Stripe support SSO / API key controls? | Yes — API keys and managed access controls are standard | https://docs.stripe.com/security | 4 |
| Are internal authentication protections enforced (e.g., MFA)? | Yes — implied by SOC 2 scope | https://docs.stripe.com/security | 3 |
| Are privileged accounts monitored? | Likely yes — part of audit scope | https://docs.stripe.com/security | 3 |

---

## 4. Availability & Continuity

| Question | Response | Evidence Source | Risk Rating |
|----------|----------|----------------|-------------|
| Does the vendor provide uptime SLAs? | Yes — enterprise SLAs available for paying customers | https://docs.stripe.com/security | 3 |
| Is disaster recovery documented and tested? | Yes — implied by audit and PCI requirements | https://docs.stripe.com/security | 3 |
| Are RPO/RTO objectives defined? | Presumed defined internally for compliance | https://docs.stripe.com/security | 3 |

---

## 5. Vendor Dependencies

| Question | Response | Evidence Source | Risk Rating |
|----------|----------|----------------|-------------|
| Does the vendor disclose critical sub-processors? | Yes — list and due diligence process provided | https://stripe.com/legal/service-providers | 4 |
| Are subcontractor controls assessed? | Yes — due diligence required before engagement | https://stripe.com/legal/service-providers | 3 |

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

Stripe demonstrates strong controls with independent audits, PCI DSS Level 1 compliance, and privacy protections. Some internal practices are not fully public and may be confirmed during onboarding or contract discussions.

---

## 7. Follow-up Clarification Questions

| Area | Clarification Request |
|------|----------------------|
| Authentication | Confirm internal MFA enforcement for admin access |
| Logging | Clarify availability of audit log details for customers |

---

## 8. Decision

| Vendor | Final Determination |
|--------|--------------------|
| Stripe | **Approved — subject to clarifications during onboarding** |

**Assessor:** Hilary Azimoh 
**Date:** 28-02-2025

