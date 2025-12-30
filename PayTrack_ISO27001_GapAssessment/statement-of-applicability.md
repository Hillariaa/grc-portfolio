# Statement of Applicability (SoA)
## PayTrack – ISO 27001:2022 (Annex A Controls)

### Purpose
This Statement of Applicability identifies which ISO 27001:2022 Annex A controls are applicable to PayTrack’s ISMS scope and explains the justification for their applicability based on legal, regulatory, contractual, risk, and operational requirements. It also records the current implementation status for audit and planning purposes.

### Applicable Controls

| Control ID | Control Name | Applicable? | Justification | Current Status |
|------------|--------------|-------------|---------------|----------------|
| A.5.1 | Policies for information security | Yes | Formal governance of information security is required to define expectations, guide implementation of controls, and demonstrate commitment to customers and auditors. | Partially Implemented |
| A.5.7 | Threat intelligence | Yes | Payroll and financial platforms are targeted by credential theft, fraud, and phishing; structured threat intelligence is needed to identify emerging risks and support incident response. | Not Implemented |
| A.5.17 | Authentication information | Yes | Protects authentication credentials for customer and internal accounts; required to reduce credential-based attack risks and protect payroll data integrity. | Implemented |
| A.5.21 | Data leakage prevention | Yes | Processing of personal and financial data creates risk of accidental or malicious data leakage; controls needed to prevent unauthorized transmission of payroll data. | Not Implemented |
| A.6.3 | Information security awareness, education, and training | Yes | Human error remains a major source of breaches; staff require training to safely handle payroll data and recognize fraud attempts. | Partially Implemented |
| A.7.2 | Physical entry | Yes | Unauthorized physical access to operational or support areas could expose credentials or devices used to administer the SaaS platform; required for defense in depth. | Partially Implemented |
| A.6.9 | Physical security monitoring | Yes | Monitoring entry points supports incident investigations and deters unauthorized access attempts that could indirectly affect platform security. | Implemented |
| A.8.16 | Monitoring activities | Yes | Continuous monitoring and alerting are required to detect unauthorized access, privilege escalation, payroll manipulation, and fraudulent activity. | Not Implemented |
| A.8.18 | Use of cryptography | Yes | Encryption is required to protect payroll and bank account information at rest and in transit and to meet regulatory and customer expectations. | Implemented |
| A.8.28 | Secure coding | Yes | Software vulnerabilities in payroll calculation logic or API endpoints could compromise confidentiality or integrity of salary data; secure coding is required. | Partially Implemented |

### Non-Applicable Controls

| Control ID | Control Name | Applicable? | Justification | Current Status |
|------------|--------------|-------------|---------------|----------------|
| A.7.5 | Secure disposal | No | PayTrack does not process or store sensitive information on physical media; secure data disposal is managed through AWS encryption and decommissioning processes. | N/A |
| A.7.7 | Storage media | No | The platform operates as a cloud-native SaaS with no removable physical media in production environments; AWS manages physical storage security. | N/A |
| A.5.10 | Acceptable use of information and assets | No | Employee use of devices for non-production workload is out of current ISMS scope; BYOD usage is restricted from access to confidential customer data. | N/A |

### Relationship to remediation
Controls marked **Partially Implemented** or **Not Implemented** generate remediation actions in the PayTrack roadmap to support certification preparation and risk reduction.

### Approval (Portfolio Simulation)

| Role | Name | Date |
|------|------|------|
| Information Security Analyst | Hilary Azimoh | 11-02-2002 |
| CTO | Jane Doe | 11-02-2002 |

