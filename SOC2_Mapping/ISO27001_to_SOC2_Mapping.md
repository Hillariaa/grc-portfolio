# ISO 27001:2022 → SOC 2 Trust Services Criteria Mapping
**Purpose:**  
This mapping shows how selected ISO 27001:2022 controls align to equivalent SOC 2 Trust Services Criteria (TSC). The goal is to demonstrate how an organization with an ISO-aligned security program can support SOC 2 readiness and external audit expectations.

---

## 🔎 Framework Notes

| Framework | Scope Focus | Notes |
|----------|------------|-------|
| ISO 27001:2022 | Information Security Management System (ISMS) | Structured around controls and risk-based management |
| SOC 2 | Controls for security, availability, confidentiality, processing integrity, privacy | Driven by attestation under AICPA criteria |

**Important:**  
ISO and SOC 2 do not map 1:1. SOC 2 tests *evidence of operation*, while ISO focuses on *management system + controls*. This mapping shows *coverage relationships*, not certification equivalence.

---

## 📂 Mapping Key

| Symbol | Meaning |
|--------|--------|
| **Full** | ISO control substantially supports SOC 2 requirement |
| **Partial** | ISO control contributes, but SOC requires additional evidence |
| **Gap** | ISO control does not cover SOC requirement; additional work needed |

---

## 🧩 ISO→SOC2 Mapping Table (Phase 1)

| ISO 27001:2022 Control | SOC 2 TSC Reference | Coverage | Notes |
|------------------------|--------------------|----------|-------|
| **A.5.1 Policies for Information Security** | CC1.2, CC1.3 | **Full** | ISO policy governance aligns to SOC 2 expectations for documented and approved policies. SOC 2 will require evidence of distribution & review. |
| **A.5.7 Threat Intelligence** | CC3.2 | **Partial** | ISO expects proactive threat awareness; SOC 2 expects threat considerations embedded into risk assessments. Evidence of *how* intel informs risk must be shown. |
| **A.6.1 Roles & Responsibilities** | CC1.4 | **Full** | Clear definition of responsibilities maps well. SOC 2 requires traceability into role assignments and approvals. |
| **A.6.3 Information Security Awareness & Training** | CC5.3 | **Full** | ISO requires training planning; SOC 2 validates completion records. Evidence depth is higher under SOC 2. |
| **A.7.2 Physical Entry Controls** | CC6.1 | **Full** | Physical access controls align closely; SOC 2 requires logs or supporting evidence for testing. |
| **A.8.1 Operational Planning & Control** | CC2.1 | **Partial** | ISO provides structure, SOC 2 needs operational consistency demonstrated through sampled evidence. |
| **A.8.16 Monitoring Activities** | CC4.1 | **Full** | Monitoring expectations support SOC 2 control evaluations. SOC 2 tests alerting and response handling in practice. |
| **A.8.28 Secure Coding** | CC3.2, CC6.6 | **Partial** | ISO control supports SOC 2 secure development expectations. SOC 2 typically requires code review evidence and dependency controls. |
| **A.9.1 Access Control Policy** | CC6.2, CC6.3 | **Full** | Alignment is strong. SOC 2 requires MFA & provisioning evidence, not just policy presence. |
| **A.9.2 User Access Management** | CC6.2 | **Full** | Access provisioning and review expectations overlap well. SOC 2 will sample user access reviews. |
| **A.9.4 System & Application Access Control** | CC6.1, CC6.2 | **Full** | ISO and SOC 2 alignment is high — both require defined controls and monitoring. |
| **A.10.1 Cryptographic Controls** | CC6.1, CC6.7 | **Full** | Encryption expectations align. SOC 2 requires proof of key management, rotation practices where applicable. |
| **A.11.1 Logging & Monitoring** | CC7.2 | **Full** | ISO logs + SOC alerting expectations complement each other. SOC 2 focuses on *investigation outcomes*. |
| **A.11.2 Security Event Handling** | CC7.3 | **Partial** | ISO requires processes; SOC 2 validates incidents with evidence. Retrospective testing fills gaps. |

---

## 📌 Early Observations (Phase 1)

- ISO controls **cover most SOC 2 security criteria** at a conceptual level.
- SOC 2 testing requires **operational evidence**, not only documented controls.
- Most “partial” cases are gaps in **recorded evidence, retention, and samples**, rather than missing controls.

In practice, an ISO-aligned organization is usually **60–75% prepared for SOC 2** before evidence gathering.

---

## 🧭 Next Steps – Phase 2 Mapping

| Task | Status |
|------|--------|
| Expand mapping to Availability, Confidentiality, PI, Privacy | Not started |
| Identify evidence needed for “partials” before SOC audit | Pending |
| Create SOC 2 evidence register template | Scheduled |
| Link mapping to your Project 1D controls | Scheduled |

---

## 📂 ISO→SOC2 Mapping Table (Phase 2 — Availability & Confidentiality)

| ISO 27001:2022 Control | SOC 2 TSC Reference | Coverage | Notes |
|------------------------|--------------------|----------|-------|
| **A.7.4 Securing Offices, Rooms and Facilities** | CC6.1, A1.1 | Full | Physical protections support both Security and Availability criteria. SOC 2 requires logs or physical review evidence during testing. |
| **A.8.3 Capacity Management** | A1.2 | Full | ISO’s expectation for capacity planning aligns with SOC 2 availability controls. Evidence typically includes monitoring thresholds and capacity plans. |
| **A.8.14 Change Management** | A1.3, CC7.2 | Partial | Change controls support Availability, but SOC 2 requires audited change tickets and approval workflows. Gaps usually relate to operational proof rather than missing processes. |
| **A.8.15 Test Management** | PI1.2, PI1.3 | Partial | Test processes contribute to service reliability. SOC 2 looks for consistent execution and evidence retention. |
| **A.8.22 Management of Technical Vulnerabilities** | CC7.1, A1.1 | Full | Vulnerability handling supports Availability through proactive remediation. SOC 2 sampling commonly tests remediation timelines. |
| **A.8.24 Logging** | CC7.2, A1.3 | Full | Logging contributes to understanding service impact and incident diagnosis. SOC 2 requires logs tied to investigations. |
| **A.8.27 Secure System Architecture and Engineering Principles** | CC3.2, A1.1 | Full | Architecture considerations support ongoing maintainability and reliability required by Availability criteria. |
| **A.9.3 Privileged Access Rights** | CC6.2, C1.1 | Partial | Privileged controls protect Confidentiality. SOC 2 requires evidence of reviews and confirmations. |
| **A.9.5 Access to Source Code** | CC6.6, PI1.1 | Full | Restricting code access protects confidentiality and integrity of internal systems. SOC 2 typically samples access lists. |
| **A.10.1 Cryptographic Controls** | C1.1 | Full | Encryption provides direct support for Confidentiality criteria. SOC 2 looks for key lifecycle evidence. |
| **A.10.2 Key Management** | C1.1 | Full | Key management practices are directly relevant to confidentiality. SOC 2 requires verification of enforcement and rotation procedures. |
| **A.11.1 Logging and Monitoring of Activities** | C1.1, CC7.2 | Full | Monitoring user actions is relevant to confidentiality protections. Evidence depth is the differentiator under SOC 2. |
| **A.11.3 Assessment for Technical Compliance** | CC7.1 | Full | Ongoing assessments support evaluation of confidentiality controls. SOC 2 will verify assessment records or tool output. |


### Observations (Phase 2)

- ISO confidentiality and availability controls generally align well to SOC 2 expectations, but SOC 2 requires **operational proof** that controls are consistently applied.
- Gaps tend to appear where **evidence retention** or **ticket sampling** is required rather than missing processes.
- ISO-driven programs are often **structured enough** for SOC 2 readiness, but require **evidence mapping** before audit timing.
- Availability alignment depends heavily on whether **change management and capacity planning** are documented and reproducible.
