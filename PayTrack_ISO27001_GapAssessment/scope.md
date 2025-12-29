# ISMS Scope – PayTrack ISO 27001:2022 Control Gap Assessment

## 1. Purpose

This document defines the scope of the ISO 27001:2022 control gap assessment for PayTrack, a SaaS payroll provider operating primarily in the European Union.

The goal of the assessment is to:

- Identify gaps against ISO 27001:2022 Annex A controls
- Provide inputs for a future Statement of Applicability (SoA)
- Support ISO 27001 certification and SOC 2 Type 1 readiness

---

## 2. Organization and Service Overview

**Organization name:** PayTrack (fictional)  
**Service:** Cloud-based payroll platform for small and medium businesses  

PayTrack provides:

- Employee onboarding and payroll processing
- Salary calculation, tax calculations, and statutory deductions
- Bank payment file generation and payment execution through integrated payment providers
- Payslip generation and delivery to employees

The platform is multi-tenant and primarily serves EU-based customers, with **planned expansion to US customers**, creating additional regulatory and cross-border data transfer considerations.

---

## 3. Scope of the ISMS (Target State)

The Information Security Management System (ISMS) is intended to cover:

- Design, development, operation, and maintenance of the PayTrack SaaS platform
- Information systems, infrastructure, and processes used to store, process, or transmit customer payroll data
- Supporting activities performed by PayTrack staff and key third parties

### In-scope components

- PayTrack SaaS web application and APIs
- Production environment hosted in **AWS eu-west-1 (Ireland)**:
  - VPC, EC2, RDS, S3, Load Balancers, Security Groups, IAM
- Identity and access management:
  - SSO / SAML (e.g., via Okta or Azure AD)
  - Role-based access control for internal staff
- CI/CD and code repositories:
  - Source control (e.g., GitHub)
  - Build and deployment workflows
- Endpoint devices used to administer and support the platform:
  - Company-managed laptops for engineering and support staff
- Logging, monitoring, and alerting tooling
- Third-party critical services:
  - Payment processor (e.g., Stripe)
  - Email/SMS provider (e.g., Twilio)
  - Error tracking and monitoring (e.g., Sentry, Datadog)

### Out-of-scope (initial phase)

- Employee personal devices (BYOD) used for non-administrative functions
- Corporate HR systems unrelated to PayTrack’s service
- Marketing website and CRM platform
- Non-production sandbox environments used for experimentation

These may be brought into scope in later ISMS maturity phases.

---

## 4. Information Types and Classification (High Level)

PayTrack processes and stores the following key information types:

- **Customer business data** – company details, billing info
- **Employee personal data (PII)** – name, address, contact information
- **Sensitive financial data** – salary information, bank account numbers
- **Authentication data** – credentials, access tokens
- **System and security logs**

A simple three-level classification model is assumed:

- **Public** – information approved for public release
- **Internal** – low-sensitivity internal operational information
- **Confidential** – customer data, employee data, and any information that could cause harm if disclosed, modified, or destroyed

---

## 5. Assumptions

- PayTrack intends to pursue **ISO 27001 certification within 12–18 months**.
- SOC 2 Type 1 readiness is targeted within the next 6–9 months.
- Existing controls are partially implemented and not consistently documented.
- The AWS Shared Responsibility Model applies for all cloud services.
- Third-party vendors will supply security documentation (e.g., SOC 2 reports, security whitepapers) to support due diligence.

---

## 6. Dependencies and Interfaces

- **Cloud provider (AWS)** – physical security, underlying infrastructure controls.
- **Payment provider** – secure payment processing and PCI-DSS-aligned controls.
- **Identity provider** – SSO, MFA, authentication policies.
- **Internal teams**:
  - Engineering (secure development and deployment)
  - Operations (incident handling, change management)
  - Customer support (secure handling of tickets and data)

This scope will be used as the basis for the Annex A control gap analysis and the draft Statement of Applicability.
