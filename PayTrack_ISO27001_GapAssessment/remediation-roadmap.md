# Remediation Roadmap – PayTrack ISO 27001:2022

This roadmap outlines prioritized actions to address gaps identified through the ISO 27001:2022 control gap assessment and Statement of Applicability. Priorities reflect potential impact to confidentiality, integrity, and availability of payroll data, as well as readiness for future ISO 27001 certification and SOC 2 Type 1 attestation.

---

## 1. High Priority (0–3 months)

| Control ID | Control Name | Gap Summary | Remediation Action | Owner | Expected Outcome |
|------------|--------------|-------------|--------------------|-------|------------------|
| A.5.1 | Policies for information security | Policy lifecycle not formalized | Centralize policies in version-controlled repo; assign owners; define approval & annual review workflow | CTO / Sec Lead | Demonstrable policy governance with audit-ready evidence |
| A.5.17 | Authentication information | Conditional access & exception handling gaps | Extend MFA and conditional access to all privileged identities; track exceptions | Engineering Lead | Reduced credential compromise risk and consistent enforcement |
| A.8.16 | Monitoring activities | No logging alert thresholds or escalation | Create severity tiers & alert playbooks; integrate with SIEM or CloudWatch | Security Operations | Improved incident detection and reduced Mean Time to Detect (MTTD) |

---

## 2. Medium Priority (3–12 months)

| Control ID | Control Name | Gap Summary | Remediation Action | Owner | Expected Outcome |
|------------|--------------|-------------|--------------------|-------|------------------|
| A.6.3 | Information security awareness | Training untracked; no developer modules | Deploy tracked LMS training and quarterly phishing simulations | People Ops / Sec Lead | Increased security awareness; measurable reduction in human risks |
| A.7.2 | Physical entry | Visitor logs inconsistent; reviews missing | Enforce check-in process; quarterly badge reviews | Operations | Reduced risk of unauthorized physical access |
| A.8.28 | Secure coding | SSDLC informal; remediation SLAs absent | Add security gates to CI; define remediation timelines; require code review sign-off | Engineering Lead | Reduced vulnerabilities in production & improved audit evidence |
| A.8.18 | Use of cryptography | Rotation & validation not regularly monitored | Validate key rotation annually; monitor TLS deprecations | Engineering Lead | Strong crypto hygiene aligned with customer & audit expectations |

---

## 3. Long Term (12+ months)

| Control ID | Control Name | Gap Summary | Remediation Action | Owner | Expected Outcome |
|------------|--------------|-------------|--------------------|-------|------------------|
| A.5.7 | Threat intelligence | No structured process | Subscribe to ISAC feeds; quarterly threat review integrated into risk register | Sec Lead | Proactive threat alignment and risk anticipation |
| A.5.21 | Data leakage prevention | DLP controls absent | Deploy baseline endpoint & email DLP; classify high-risk data flows | Sec Lead / IT | Reduced risk of accidental payroll data disclosure |

---

## 4. Proposed Sequencing

1. **Stabilize foundations**
   - Policies, authentication hardening, monitoring workflows

2. **Increase control coverage**
   - Training, physical access, secure SDLC

3. **Enhance maturity**
   - Threat intelligence, DLP deployment

This sequence reduces **breach likelihood first**, then **audit risk**, then **strategic capabilities**.

---

## 5. Metrics for Leadership (recommended)

| Metric | Target | Purpose |
|--------|--------|---------|
| MFA coverage for privileged accounts | 100% | Credential protection |
| Time to revoke access after departure | < 24h | Reduce insider risk |
| Restoration test frequency | Quarterly | Validate continuity |
| Vulnerability remediation SLA | 30 days critical | Reduce exploit window |
| Phishing simulation failure | ↓ 20% per year | Improve staff resilience |

---

## 6. Certification Readiness Indicators

| Control Area | Status After Roadmap Completion |
|--------------|--------------------------------|
| Policy governance | Audit-ready |
| Access control | Fully enforced |
| Monitoring & alerting | Operational |
| Secure development | Evidenced |
| Risk treatment | Structured and traceable |

---

**Next step:** Integrate remediation items into backlog, assign milestones, and report monthly progress to leadership.
