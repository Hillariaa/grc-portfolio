# Combined Remediation Roadmap – TalentVisionAI
## ISO 27001:2022 + AI Governance (ISO/IEC 42001 Concepts & NIST AI RMF)

This roadmap prioritizes remediation activities based on security, privacy, fairness, explainability, and regulatory requirements for a high-risk AI platform used in candidate screening and ranking. Actions are sequenced to reduce immediate risk, establish measurement and governance, and prepare for emerging regulation.

---

## 1. High Priority (0–3 months) — Foundations & Fairness

| Control ID | Standard | Gap Summary | Remediation Action | Owner | Expected Outcome |
|------------|----------|-------------|--------------------|-------|------------------|
| A.5.1 | ISO27001 | Policy governance informal | Move policies to GitHub; define ownership, approvals, and annual review cadence | CTO / Sec Lead | Clear policy governance and audit-ready evidence |
| A.8.16 | ISO27001 | No alert triage or thresholds | Define severity tiers; configure alerting via SIEM/CloudWatch; create on-call rotation | Security Ops | Reduced time to detect and respond to security events |
| AI-D2 | AI Govern | No bias identification or mitigation | Implement quarterly bias tests; document mitigation techniques | AI Lead | Reduced discriminatory outcomes; GDPR fairness alignment |
| AI-M1 | AI Govern | Limited transparency & explainability | Produce rationale summaries aligned to GDPR transparency expectations | AI Lead | Improved trust in recommendations and human review quality |
| AI-U1 | AI Govern | No contestability or appeal mechanism | Create applicant challenge workflow; publish process; track disputes | HR Ops / AI Lead | Demonstrable meaningful human oversight; EU AI Act readiness |
| AI-G1 | AI Govern | Roles unclear; no RACI | Define RACI for model lifecycle & AI risk governance; assign owners | CTO / AI Lead | Traceable responsibility and accountability for AI control decisions |

---

## 2. Medium Priority (3–12 months) — Measurement & Control

| Control ID | Standard | Gap Summary | Remediation Action | Owner | Expected Outcome |
|------------|----------|-------------|--------------------|-------|------------------|
| A.6.3 | ISO27001 | Training untracked | Deploy LMS; introduce developer training; run phishing simulations | People Ops | Measurable human risk reduction and improved compliance |
| A.7.2 | ISO27001 | Physical access logging inconsistent | Enforce visitor logging; quarterly badge reviews | Ops | Secure physical access to environments and support areas |
| AI-G4 | AI Govern | Dataset lineage limited | Automate lineage metadata in feature store | Data Eng | Traceable models and improved audit posture |
| AI-M2 | AI Govern | No adverse impact monitoring | Track impact metrics quarterly; escalate threshold breaches | AI Lead | Early detection of discriminatory model outcomes |
| AI-M3 | AI Govern | No drift monitoring | Deploy drift detection alerts and retraining workflow | AI Lead | Prevent model degradation and fairness drift |
| AI-M4 | AI Govern | Approval gates informal | Add security + fairness checks to deployment gates | AI Lead | Controlled and auditable model releases |
| A.8.28 | ISO27001 | SSDLC informal | Add security scanning & approvals into CI/CD; set remediation SLAs | Eng Lead | Reduced production vulnerabilities and more secure releases |

---

## 3. Long-Term (12+ months) — Strategic & Regulatory Alignment

| Control ID | Standard | Gap Summary | Remediation Action | Owner | Expected Outcome |
|------------|----------|-------------|--------------------|-------|------------------|
| AI-G5 | AI Govern | High-risk registration absent | Register system as high-risk under EU AI Act when applicable | Legal / Sec Lead | Regulatory conformity readiness without disruption |
| A.5.7 | ISO27001 | No threat intelligence | Subscribe to ISAC feeds; conduct quarterly threat reviews | Sec Lead | Proactive anticipation of new threats relevant to HR/AI systems |
| A.5.21 | ISO27001 | No DLP controls | Deploy DLP across endpoints and email; classify high-risk flows | Sec Lead / IT | Reduced risk of unintentional data leakage |
| AI-M5 | AI Govern | No adversarial robustness testing | Add adversarial testing and poisoning/evasion defense checks | AI Lead / Sec Lead | Protection against ranking manipulation and candidate fraud |
| AI-D3 | AI Govern | Proxy attributes unchecked | Identify and mitigate proxy variables correlated to sensitive traits | Data Eng | Reduced indirect discrimination risk and accountability on fairness |

---

## 4. Proposed Sequencing

### Phase 1 — Foundations & Fairness (0–3 months)
- Policy governance formalization
- Bias identification & mitigation
- Explainability & rationale summaries
- Alerting & escalation workflows
- Contestability & appeal mechanisms
- AI governance roles established

### Phase 2 — Measurement & Control (3–12 months)
- Model drift detection & retraining workflows
- Adverse impact monitoring & escalation
- Dataset lineage and provenance reporting
- SSDLC integration within CI/CD
- Measurable security & awareness training

### Phase 3 — Strategic & Regulatory Alignment (12+ months)
- High-risk AI system registration (EU AI Act)
- DLP deployment across data channels
- Adversarial robustness & model attack testing
- Proactive industry-aligned threat intelligence

---

## 5. Success Metrics (Reporting to Leadership)

| Metric | Target | Domain | Signal |
|--------|--------|--------|--------|
| Bias reduction trend | ↓ year-over-year | AI | Fairness maturity |
| Adverse impact alerts | Captured & escalated | AI | Harm detection |
| MFA coverage | 100% privileged | ISO | Credential protection |
| Incident triage SLA | < 1 hour | ISO | Operational readiness |
| Override justification rate | 100% logged | AI | Meaningful human oversight |
| Drift alerts | Monthly review | AI | Model trustworthiness & lifecycle control |
| Training completion | 95% within 30 days | ISO | Human risk reduction |

---

## 6. Certification & Regulatory Readiness

| Requirement | Alignment |
|------------|----------|
| ISO 27001 certification | Target-ready in 12–18 months |
| SOC 2 Type 1 readiness | Aligned with remediation tasks |
| EU AI Act (high-risk) | Foundational alignment & phased preparation |
| GDPR profiling expectations | Partially aligned; transparency & appeals improving |

---

**Next step:** Integrate roadmap actions into delivery backlogs and report progress monthly to stakeholders.
