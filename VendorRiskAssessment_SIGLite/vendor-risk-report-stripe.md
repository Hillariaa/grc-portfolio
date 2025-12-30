# Vendor Risk Report — Stripe

**Vendor:** Stripe  
**Service:** Payment processing and financial data services  
**Assessment Type:** Public documentation review  
**Assessed By:** Hilary Azimoh  
**Date:** 28-02-2025 
**Overall Risk Rating:** Low to Moderate Risk (3.4 / 4)

---

## 1. Executive Summary

Stripe is a well-established payment processor with a mature security posture supported by independent audits and PCI DSS Level 1 certification. The vendor processes sensitive personal and financial data, which drives a higher baseline risk, but available evidence indicates strong security, privacy, and operational controls.

Not all internal access-control practices are publicly detailed, which is common for regulated financial services. These gaps should be clarified during onboarding but do not indicate material weaknesses.

At this stage, Stripe is suitable for use as a third-party vendor, assuming standard contractual and risk acceptance steps are followed.

---

## 2. Scope & Context

| Category | Details |
|----------|---------|
| Data handled | Payment card data, PII, transaction data |
| Business impact | High — financial processing and revenue handling |
| Geographic considerations | Global operations with privacy alignment |
| Assessment scope | Security, privacy, availability, vendor dependencies |
| Documentation basis | Publicly available compliance material |

The review focused on whether Stripe’s publicly stated controls align with expectations for a payment processor with access to sensitive data.

---

## 3. Summary of Findings

| Control Area | Strengths | Considerations | Rating (0–4) |
|--------------|----------|----------------|--------------|
| Governance & Risk | Independent audits (SOC 1 & SOC 2), established governance | Operational detail not publicly available | 4 |
| Data Security & Privacy | PCI DSS Level 1, encryption, tokenization, GDPR alignment | Limited visibility into tokenization internals | 4 |
| Identity & Access | Assumed MFA & privileged access controls from audit scope | Internal MFA enforcement not explicitly stated | 3 |
| Availability & Continuity | Enterprise-grade expectations validated via compliance standards | No detailed RPO/RTO published | 3 |
| Vendor Dependencies | Sub-processor transparency and due diligence | Limited detail on subcontractor frequency | 3 |

---

## 4. Key Observations

1. **Stripe’s certification and audit posture is strong.**  
   SOC and PCI certifications reflect well-defined internal processes and control structures.

2. **Financial data handling is aligned with industry standards.**  
   Tokenization and encryption significantly reduce direct exposure to card data.

3. **Identity protections are implied rather than explicitly documented.**  
   This is typical for PCI environments but should be confirmed through due diligence.

4. **Continuity expectations are reasonable but not transparent.**  
   Customers usually obtain continuity specifics under NDA during onboarding.

5. **Data subject rights are supported via the privacy framework.**  
   GDPR controls appear well implemented and documented.

---

## 5. Residual Risk Statement

Stripe’s residual risk is **Low to Moderate**, driven primarily by:

- lack of public detail on internal authentication and privileged access practices  
- limited visibility on disaster recovery cadence  
- high risk category of data handled (financial + personal)

These items represent **visibility gaps rather than control gaps**, and can typically be addressed through onboarding clarifications.

---

## 6. Questions to Clarify During Onboarding

| Area | Clarification Request |
|------|----------------------|
| Authentication | Confirm internal MFA enforcement for privileged access |
| Logging | Confirm customer access to audit logs or log exports |
| Continuity | Confirm frequency of DR testing and high-level RPO/RTO targets |
| Vendor Dependencies | Confirm subcontractor review cadence |

---

## 7. Recommended Actions

| Action Category | Recommendation | Owner |
|-----------------|----------------|-------|
| Contractual | Ensure contractual references to PCI DSS & audit rights | Procurement / Legal |
| Due Diligence | Request onboarding package including SOC 2 report | Security / VRM |
| Access Assurance | Validate MFA and privileged access controls | Security |
| Logging | Ask whether logs or events can be exported or integrated | Engineering / Security |

---

## 8. Final Determination

| Vendor | Risk Decision | Conditions |
|--------|--------------|------------|
| Stripe | **Approved for use** | Follow-up questions to be confirmed during onboarding |

**Rationale:**  
Stripe meets industry expectations for financial services security and privacy. Remaining questions relate to verification of internal controls rather than remediation. These are reasonable to resolve contractually.

---

## 9. Review Cycle Recommendation

| Cycle | Justification |
|-------|--------------|
| **Annual review** | Payment processor; compliance cycles align to annual audit reporting |

