# 📋 NELMMA Aviation — Data Governance Policy Templates

> **Usage Note:** Each section below represents a standalone policy document.  
> Copy each section into its own file using the naming convention: `DG-POL-00X_[Policy-Name].md`

---

# DG-POL-001: Data Classification Policy

**Version:** 1.0 | **Owner:** Data Governance Lead | **Classification:** Internal

## Purpose
To define how Nelmma Aviation classifies its data assets according to sensitivity, enabling appropriate protection, access control, and handling procedures.

## Classification Levels

| Level | Label | Definition | Examples |
|---|---|---|---|
| Level 4 | 🔴 CONFIDENTIAL | Highest sensitivity; exposure causes severe harm | Passport/ID data, GSSA contract terms, financial statements, executive decisions |
| Level 3 | 🟠 RESTRICTED | Sensitive; exposure causes significant harm | Customer PII, cargo manifests with shipper details, employee records, partner agreements |
| Level 2 | 🟡 INTERNAL | Business use only; not for public release | Flight schedules, route data, internal reports, operational procedures |
| Level 1 | 🟢 PUBLIC | Approved for external publication | Service descriptions, marketing materials, press releases |

## Responsibilities
- **Data Owners** classify all assets within their domain
- **DG Lead** reviews and approves classifications for Confidential/Restricted assets
- **All staff** handle data according to its assigned classification level

## Review
Classification is reviewed annually or upon material change in business context.

---

# DG-POL-002: Access Control Policy

**Version:** 1.0 | **Owner:** IT Data Custodian | **Classification:** Internal

## Purpose
To ensure that access to Nelmma data assets is granted only to authorized individuals, at the minimum level necessary for their role.

## Principles
- **Least Privilege:** Access is granted at the minimum level required for job function
- **Need to Know:** Access is restricted to those with a documented business need
- **Separation of Duties:** No individual has unrestricted access to modify and approve data
- **Role-Based Access Control (RBAC):** Permissions are assigned to roles, not individuals

## Access Levels

| Access Level | Permissions | Assigned To |
|---|---|---|
| Read-Only | View data; no modification | Auditors, external partners (limited) |
| Read-Write | View and modify data within domain | Operational staff, stewards |
| Administrative | Full access including deletion | Data Custodians (IT), DG Lead |
| Super-Admin | System-level access | IT Manager + DG Lead jointly |

## Access Lifecycle
1. **Request:** Submit Access Request Form (ARF-001) to DG Lead
2. **Approval:** Data Owner approves; IT Custodian provisions
3. **Review:** Quarterly access reviews by DG Lead
4. **Revocation:** Immediate revocation upon role change or departure

## Breach of Access Policy
Unauthorized access attempts are logged, investigated, and reported per DG-POL-006.

---

# DG-POL-003: Data Retention and Disposal Policy

**Version:** 1.0 | **Owner:** Data Governance Lead | **Classification:** Internal

## Purpose
To define how long Nelmma retains different categories of data and how data is securely disposed of at end-of-life.

## Retention Schedule

| Data Category | Retention Period | Legal Basis | Disposal Method |
|---|---|---|---|
| Passenger PII | 7 years | Act 843, GCAA | Secure deletion + certificate |
| Cargo Manifests | 10 years | Customs law | Secure archival then deletion |
| Financial Records | 10 years | Ghana Companies Act | Encrypted archive then destruction |
| Employee Records | 7 years post-departure | Labour Act | Secure deletion |
| Partner Contracts | Duration + 7 years | Contract law | Legal hold then secure deletion |
| Marketing Data | Until consent withdrawn | GDPR, Act 843 | Deletion upon request |
| Audit Logs | 5 years | Governance policy | Immutable archive |

## Disposal Standards
- Electronic data: Cryptographic erasure or NIST 800-88 compliant wiping
- Physical documents: Cross-cut shredding by certified provider
- Disposal must be documented with date, method, and authorizing officer

---

# DG-POL-004: Privacy and Consent Policy

**Version:** 1.0 | **Owner:** Data Protection Officer | **Classification:** Internal

## Purpose
To ensure Nelmma collects and processes personal data only with valid consent and in compliance with applicable privacy laws.

## Consent Requirements
- Consent must be **freely given, specific, informed, and unambiguous**
- Consent is obtained before or at the point of data collection
- Records of consent are maintained and auditable
- Individuals may withdraw consent at any time

## Individual Rights (Act 843 / GDPR)

| Right | Description | Response Time |
|---|---|---|
| Access | Individuals may request a copy of their data | 30 days |
| Correction | Individuals may request correction of inaccurate data | 14 days |
| Erasure | Individuals may request deletion of their data | 30 days |
| Restriction | Individuals may restrict processing of their data | 14 days |
| Portability | Individuals may request data in machine-readable format | 30 days |
| Objection | Individuals may object to data processing | Immediate assessment |

## Cross-Border Transfers
- Data transferred to EU (Belgium): GDPR Standard Contractual Clauses required
- Data transferred to China: PIPL compliance checks and transfer impact assessment required
- All cross-border transfers are logged and reviewed quarterly

---

# DG-POL-005: Data Quality Policy

**Version:** 1.0 | **Owner:** Data Governance Lead | **Classification:** Internal

## Purpose
To define the data quality standards Nelmma must maintain across all operational data assets.

## Quality Dimensions (ISO 8000)

| Dimension | Definition | Measurement |
|---|---|---|
| **Accuracy** | Data correctly represents reality | Error rate per domain |
| **Completeness** | Required fields are populated | % of complete records |
| **Consistency** | Data is uniform across systems | Cross-system match rate |
| **Timeliness** | Data is current and up-to-date | Lag from event to record |
| **Validity** | Data conforms to defined formats and rules | % format compliance |
| **Uniqueness** | No unintended duplicate records exist | Duplicate rate |

## Target Standards

| Domain | Accuracy Target | Completeness Target | Review Frequency |
|---|---|---|---|
| Cargo Manifests | ≥ 99% | ≥ 98% | Weekly |
| Passenger Records | ≥ 99.5% | 100% | Per-flight |
| Financial Data | 100% | 100% | Monthly |
| Customer Master Data | ≥ 97% | ≥ 95% | Monthly |
| Compliance Records | 100% | 100% | Quarterly |

## Quality Issue Resolution
- **Minor issues (< 5% error rate):** Steward corrects within 5 business days
- **Moderate issues (5–15%):** Data Owner involved; root cause analysis required
- **Critical issues (> 15% or compliance-critical):** Escalate to DG Lead; operational hold on affected data

---

# DG-POL-006: Data Breach Response Policy

**Version:** 1.0 | **Owner:** Data Protection Officer | **Classification:** Internal

## Purpose
To define the process for identifying, containing, reporting, and recovering from data breaches.

## Breach Definition
A data breach is any confirmed or suspected incident resulting in unauthorized access to, disclosure of, alteration of, or destruction of Nelmma data assets.

## Response Procedure

| Step | Action | Timeframe | Owner |
|---|---|---|---|
| 1. **Detect** | Identify and confirm the breach | Immediate | Any staff |
| 2. **Report** | Notify DG Lead and DPO | Within 2 hours | Discovering staff |
| 3. **Contain** | Isolate affected systems; revoke compromised access | Within 4 hours | IT Custodian |
| 4. **Assess** | Determine scope, data affected, and individuals impacted | Within 24 hours | DPO + DG Lead |
| 5. **Notify Authorities** | Report to Data Protection Commission (Act 843) | Within 72 hours | DPO |
| 6. **Notify Individuals** | Inform affected data subjects | Within 7 days | DPO |
| 7. **Remediate** | Fix root cause; implement controls | Within 30 days | IT + DG Lead |
| 8. **Review** | Post-incident review and lessons learned | Within 45 days | Governance Council |

## Breach Log
All incidents (confirmed and suspected) must be logged in the Breach Register (maintained by DPO).

---

# DG-POL-007: Cross-Border Data Transfer Policy

**Version:** 1.0 | **Owner:** Data Protection Officer | **Classification:** Restricted

## Purpose
To govern the transfer of personal and operational data across international borders in compliance with applicable laws.

## Transfer Corridors

| Corridor | Regulation | Mechanism Required |
|---|---|---|
| Ghana → EU / Belgium | GDPR Article 46 | Standard Contractual Clauses (SCCs) |
| Ghana → China | PIPL Chapter 4 | Transfer Impact Assessment + PRC authority notification |
| Ghana → Nigeria / Liberia / Mali | ECOWAS + local laws | Data-sharing agreement with privacy provisions |
| Ghana → USA (NJ Warehouse) | Sectoral US law | Binding Corporate Rules or SCCs |

## Requirements for All Cross-Border Transfers
1. Transfer is documented in the Cross-Border Transfer Register
2. Receiving party has agreed to data protection terms in writing
3. Adequacy assessment confirms receiving country's legal protections
4. DPO has reviewed and approved the transfer arrangement

---

# DG-POL-008: Metadata Management Policy

**Version:** 1.0 | **Owner:** Data Governance Lead | **Classification:** Internal

## Purpose
To ensure that all Nelmma data assets are consistently described through standardized metadata, enabling discoverability, traceability, and governance.

## Mandatory Metadata Fields

| Field | Description | Example |
|---|---|---|
| Asset Name | Business name of the data asset | "Cargo Manifest — Inbound" |
| Domain | Business domain owning the asset | Cargo Operations |
| Data Owner | Named accountable individual | Head of Cargo |
| Data Steward | Named operational responsible | Cargo Data Steward |
| Classification | Sensitivity level per DG-POL-001 | Restricted |
| Retention Period | Per DG-POL-003 | 10 years |
| Source System | System of record | Cargo Management System (CMS) |
| Last Updated | Date of last metadata review | 2025-01-15 |
| Data Quality Score | Most recent quality assessment | 97.3% |
| Regulatory Tags | Applicable regulations | Act 843, Customs Law |

## Metadata Repository
All metadata is stored in the central Nelmma Data Catalog, accessible to Data Owners, Stewards, and the DG Lead.

---

*All policies are effective upon approval by the Data Governance Council and CEO signature.*  
*Review cycle: Annual, or upon material business change.*
