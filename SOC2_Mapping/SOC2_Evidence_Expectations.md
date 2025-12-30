# SOC 2 Evidence Expectations (ISO-Aligned Security Program)

**Purpose:**  
Translate ISO 27001-aligned control practices into the types of evidence a SOC 2 auditor typically samples. This supports planning for SOC 2 readiness rather than treating certification as a documentation-only exercise.

**Context:**  
While ISO defines required controls and risk management, SOC 2 validates whether those controls are **operating effectively** over time. Most gaps appear where ISO programs have controls in place, but **evidence is not consistently recorded or retained**.

---

## Evidence Mapping Key

| Evidence Type | Description |
|----------------|-------------|
| Documentary | Policy, procedure, standard |
| Operational | Tickets, logs, approvals, review outcomes |
| Technical | Tool output, scans, access lists |
| Attestation | Signed management assertions or confirmations |

---

## SOC 2 Evidence Needs Aligned to ISO Controls

| ISO Control | SOC 2 Need | Evidence Expected in SOC 2 | Gap Risk |
|-------------|------------|----------------------------|----------|
| **A.5.1 Information Security Policies** | CC1.2 | Published policies, version history, annual review sign-off | *Low* — ISO requires policies, SOC 2 requires **proof of review cadence** |
| **A.6.1 Roles & Responsibilities** | CC1.4 | Org chart, role definitions, onboarding docs | *Low* — as long as responsibilities are documented and assigned |
| **A.6.3 Awareness & Training** | CC5.3 | Training completion logs, reminders, % completion metrics | *Medium* — ISO doesn’t require proof of completion; SOC 2 samples **training records** |
| **A.7.2 Physical Entry Controls** | CC6.1, A1.1 | Visitor logs, badge reports, access reviews | *Low to Medium* — depends on availability of logs & retention |
| **A.8.14 Change Management** | A1.3 | Change tickets, approvals, rollback plans, post-change checks | *High* — most ISO programs lack **ticket-level approval evidence** |
| **A.8.22 Vulnerability Management** | CC7.1 | Scan results, remediation tracking, SLA adherence | *Medium* — SOC 2 verifies **closure within timelines** |
| **A.8.24 Logging** | CC7.2 | Log retention proof, investigation records, alert summaries | *Medium* — ISO requires logging; SOC 2 requires **analysis evidence** |
| **A.8.27 Secure System Architecture** | CC3.2 | Architecture diagrams, design reviews, dependency tracking | *Low* — usually aligned if architecture design reviews exist |
| **A.9.2 User Access Management** | CC6.2 | Access request tickets, terminations, quarterly access reviews | *High* — SOC 2 samples **approvals and revocation dates** |
| **A.9.3 Privileged Access Rights** | C1.1, CC6.2 | Admin access lists, MFA enforcement proof, review outcomes | *Medium to High* — MFA is often assumed but not evidenced |
| **A.10.1 Cryptographic Controls** | C1.1 | Encryption config screenshots, key rotation logs | *Medium* — SOC 2 needs rotation visibility |
| **A.11.1 Logging & Monitoring** | CC7.2 | Incident tickets, investigation summaries, closures | *High* — ISO doesn’t force **ticket-based investigation evidence** |

---

## Patterns Observed

1. **ISO supports the existence of controls; SOC 2 validates execution**
2. Evidence gaps appear when **actions are performed but not formally logged**
3. The most common blockers for SOC 2 readiness:
   - missing **approval tickets**
   - incomplete **access review records**
   - no **recorded incident summaries**
   - limited **remediation tracking**
4. **Policies rarely block SOC 2 — missing operational proof does**

---

## Practical Guidance for SOC 2 Readiness

| Area | Practical Step | Why It Helps |
|------|----------------|--------------|
| Access Reviews | Track quarterly reviews in ticketing or spreadsheet | SOC 2 will sample dates & reviewers |
| Training | Export completion report quarterly | Shows **operating effectiveness** |
| Incidents | Record investigation summaries even for low impact events | Demonstrates **traceability** |
| Changes | Require approval field in tickets or Git PRs | Auditors will pull samples |
| Vulnerabilities | Assign remediation deadlines | Aligns with **SOC timelines expectations** |

---

## High-Value Evidence Preparation (Pre-Audit)

**Before SOC 2:**
- Create a **review log** template (access, vendors, policy reviews)
- Export **training completion reports** quarterly
- Store **scan results + closure evidence**
- Ensure **change approvals** are consistently captured
- Track **incident investigations** beyond basic alerts

These practices **solve most partial mappings** from Phase 1 & 2.

---

## Readiness Summary

An ISO-driven program typically satisfies most SOC 2 control expectations conceptually.  
SOC 2 readiness depends primarily on **evidence discipline**, not missing controls.

Assuming consistent record-keeping, an ISO-aligned environment is generally **60–75% ready** before evidence gathering.

---

