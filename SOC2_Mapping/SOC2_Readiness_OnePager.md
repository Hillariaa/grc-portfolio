# SOC 2 Readiness Summary (Based on ISO-Aligned Controls)

**Objective:**  
Provide a high-level assessment of SOC 2 readiness based on existing ISO 27001–aligned controls and current operational practices. This summary is intended to support planning for a first SOC 2 audit cycle and highlight areas where evidence discipline is required to avoid remediation findings.

---

## Overall Readiness

| Category | Assessment | Confidence |
|----------|------------|------------|
| Control Coverage (Security, Availability, Confidentiality) | Strong conceptual alignment via ISO controls | High |
| Operational Evidence Depth | Inconsistent across domains | Medium |
| Audit Sampling Preparedness | Developing | Medium |
| Expected Audit Effort | Moderate | — |

### Readiness Rating  
> **2.2 / 3 — Developing toward audit readiness**

**Interpretation:**  
Controls largely exist and align to SOC 2 expectations, but readiness depends on establishing consistent and traceable evidence for access reviews, change approvals, and incident investigation summaries. These evidence practices usually require one to two quarters to mature.

---

## Key Strengths

- Policies, governance, and certification alignment form a solid baseline
- Encryption and key management practices meet Confidentiality expectations
- Access restrictions and RBAC controls are established across systems
- Logging and monitoring are implemented and support incident detection
- Vendor dependencies are documented with transparency into subprocessors

---

## Areas Requiring Evidence Discipline

| Control Area | Needed Evidence | Reason |
|--------------|----------------|-------|
| Access Reviews | Documented quarterly reviews | SOC 2 samples review outcomes |
| Change Management | Approval workflow and rollback plans | Operational consistency must be proven |
| Incident Handling | Investigation summaries per event | Shows monitoring leads to action |
| Training Completion | Exported completion logs | Supports CC5.3 validation |
| Privileged Access | MFA enforcement verification | Common SOC 2 clarification request |

---

## Priority Actions Before Audit

1. Formalize quarterly access and permissions review recordings  
2. Require approval or justification for changes in tickets or PRs  
3. Log investigation summaries for all security events, not only major incidents  
4. Export and store training completion records per quarter  
5. Confirm MFA enforcement for admin or privileged roles platform-wide

These steps improve **audit sampling outcomes** without increasing operational overhead.

---

## Recommended Readiness Timeline

| Quarter | Focus | Outcome |
|---------|-------|---------|
| Q1 | Establish evidence tracking for access, changes, incidents | Evidence baseline |
| Q2 | Maintain cadence and close minor gaps | Audit-ready sampling |
| Q3 | Optional internal audit or mock sampling | Confidence before external audit |

---

## Summary

The organization is structurally well-positioned for SOC 2 due to ISO alignment, but audit readiness depends on **evidence consistency and sampling maturity** rather than adding new controls. The most effective path forward is to treat SOC 2 preparation as an **evidence lifecycle project**, not a policy rewrite.

With steady evidence discipline over 1–2 quarters, the organization should be prepared to enter a SOC 2 audit cycle with reasonable confidence.

---

**Assessor:** Hilary Azimoh  
**Updated:** 11-03-2025
