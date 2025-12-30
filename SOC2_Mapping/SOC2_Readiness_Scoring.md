# SOC 2 Readiness Scoring (Based on ISO-Aligned Controls)

**Purpose:**  
Estimate SOC 2 readiness by evaluating the strength of existing ISO-aligned controls and identifying where additional evidence and operational consistency is required. This provides a realistic view of effort needed before a SOC 2 audit cycle.

**Scoring model:**  
Each control area is rated **0–3**, based on evidence maturity rather than documented intent.

| Score | Meaning |
|-------|---------|
| **0 — Not Present** | Control or evidence missing |
| **1 — Emerging** | Control exists, evidence limited or inconsistent |
| **2 — Developing** | Control operating, needs evidence discipline |
| **3 — Ready** | Control operating with consistent evidence |

This approach emphasizes practical audit readiness rather than theoretical framework coverage.

---

## 🔎 Readiness Scores by Domain

| Domain | Readiness Score (0–3) | Rationale |
|--------|-----------------------|----------|
| **Governance & Risk Management** | **3** | Policies and certification alignment indicate strong governance; main focus is review cadence documentation. |
| **Security Controls (Core)** | **2** | Controls exist and align with ISO; sampling evidence (access reviews, change tickets, incident records) determines readiness. |
| **Identity & Access Management** | **2** | Provisioning and RBAC requirements covered, but SOC 2 requires consistent review evidence and MFA proof. |
| **Availability & Continuity** | **2** | Capacity and continuity expectations align with ISO; readiness depends on change records and DR testing proof. |
| **Confidentiality Controls** | **3** | Encryption, key controls, and restricted access align well; key rotation evidence and logging depth strengthen confidence. |
| **Vendor Dependencies** | **2** | Transparency is strong, but subcontractor review cadence needs confirmation to satisfy SOC 2 expectations. |
| **Operational Evidence Discipline** | **1** | Common gap area: approvals, access reviews, incident summaries, and remediation timelines need consistent tracking. |

---

## 📊 Readiness Summary

| Category | Score | Notes |
|----------|-------|-------|
| Structural control coverage | **High** | ISO alignment gives solid coverage against SOC requirements |
| Operational evidence depth | **Medium** | Some controls lack consistent sampling evidence |
| Documentation completeness | **High** | Policies and governance practices align well |
| Audit sampling confidence | **Medium** | Gaps relate to review frequency and retention discipline |

### **Overall SOC 2 readiness:**  
> **2.2 / 3 — “Developing toward audit readiness”**

This indicates that the organization would not fail a SOC 2 audit due to control absence, but would likely receive remediation findings if **evidence discipline is not strengthened** before the audit window.

---

## 🎯 Key Remediation Priorities (Pre-Audit)

| Priority | Task | Reason |
|----------|------|--------|
| **High** | Track access review outcomes quarterly | Direct sampling requirement in SOC 2 |
| **High** | Capture change approvals systematically | Auditors request evidence during control testing |
| **High** | Record incident investigation summaries | Shows monitoring is not just alerting |
| **Medium** | Export training completion logs | Supports CC5.3 evidence requirements |
| **Medium** | Confirm MFA for privileged users | Often assumed but needs explicit validation |
| **Low** | Refresh subcontractor due diligence records | Supports transparency for dependencies |

---

## 📌 Interpretation Guidance

- **Readiness is not binary** — this scoring provides direction, not certification assurance
- **Evidence discipline** is usually the bottleneck, not missing controls
- **ISO maturity translates well** but does not replace operational sampling
- Organizations at this level typically need **1–2 quarters** to fully prepare for SOC 2 testing

---

## 🧭 Target State

> The path to “ready” status is primarily **operational** rather than **architectural**:
> - controls are in place
> - certifications align
> - but evidence needs consistency

Once quarterly reviews, approvals, and incident tracking are routine, readiness moves toward **2.8–3.0**, which is generally sufficient to enter a SOC 2 audit cycle with confidence.

