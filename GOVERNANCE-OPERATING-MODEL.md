# 🏛️ NELMMA Aviation — Governance Operating Model

**Document ID:** DG-OPS-001  
**Version:** 1.0  
**Owner:** Data Governance Lead

---

## 1. Governance Hierarchy

```
┌─────────────────────────────────────────────────────┐
│              STRATEGIC LAYER                         │
│                                                      │
│   DATA GOVERNANCE COUNCIL                            │
│   Chair: CEO | Members: Business Unit Heads          │
│   Authority: Policy approval, strategy, disputes     │
└──────────────────────┬──────────────────────────────┘
                       │ Reports to Council
┌──────────────────────▼──────────────────────────────┐
│              MANAGEMENT LAYER                        │
│                                                      │
│   DATA GOVERNANCE LEAD                               │
│   + DATA PROTECTION OFFICER (DPO)                    │
│   Authority: Daily operations, compliance, training  │
└──────────┬─────────────────────────┬────────────────┘
           │                         │
┌──────────▼──────────┐   ┌─────────▼──────────────┐
│   DOMAIN LAYER      │   │   TECHNICAL LAYER       │
│                     │   │                         │
│   DATA OWNERS       │   │   DATA CUSTODIANS (IT)  │
│   (per domain)      │   │   Storage, Security,    │
│   + DATA STEWARDS   │   │   Access Provisioning   │
└─────────────────────┘   └─────────────────────────┘
           │
┌──────────▼──────────────────────────────────────────┐
│              OPERATIONAL LAYER                       │
│                                                      │
│   END USERS — Cargo, Passenger, Customs, Finance,   │
│   HR, Partner Management                             │
└─────────────────────────────────────────────────────┘
```

---

## 2. Decision-Making Structure

### 2.1 Strategic Decisions (Governance Council)
Decisions requiring full council vote (simple majority):
- Adoption of new or revised governance policies
- Appointment of Data Owners and Data Governance Lead
- Approval of cross-border data-sharing agreements
- Response to regulatory enforcement actions
- Annual framework review and approval

**Meeting cadence:** Quarterly (mandatory); extraordinary as needed

### 2.2 Operational Decisions (DG Lead + DPO)
Decisions within delegated authority:
- Approval of individual data access requests
- Classification of new data assets
- Incident escalation and initial response
- Training content and scheduling
- Routine audit findings and remediation tracking

**Escalation trigger:** Any decision with regulatory, financial, or reputational implications > GHS 10,000

### 2.3 Domain Decisions (Data Owners)
Decisions within data domain:
- Data quality issue resolution
- Steward assignment and tasking
- Domain-specific standards and procedures
- Metadata updates and data catalog maintenance

---

## 3. Escalation Process

```
LEVEL 1 — Data User
   Issue: Identified data quality error or access problem
   Action: Report to Data Steward within 1 business day
   Resolution target: 3 business days

LEVEL 2 — Data Steward
   Issue: Cannot resolve; pattern identified; policy unclear
   Action: Escalate to Data Owner with documented evidence
   Resolution target: 5 business days

LEVEL 3 — Data Owner
   Issue: Cross-domain impact; policy conflict; resource constraint
   Action: Escalate to DG Lead with impact assessment
   Resolution target: 10 business days

LEVEL 4 — Data Governance Lead / DPO
   Issue: Legal/regulatory risk; unresolved cross-domain conflict
   Action: Escalate to Governance Council
   Resolution target: Next Council meeting (maximum 45 days)

LEVEL 5 — Governance Council
   Issue: Strategic policy decision; regulatory enforcement action
   Action: Extraordinary Council meeting; external legal advice if required
   Resolution target: 15 business days (extraordinary)
```

---

## 4. RACI Matrix — Core Governance Activities

**R** = Responsible (does the work) | **A** = Accountable (answerable for outcome) | **C** = Consulted | **I** = Informed

| Governance Activity | CEO | Gov. Council | DG Lead | DPO | Data Owner | Data Steward | IT Custodian | HR/Training | End User |
|---|---|---|---|---|---|---|---|---|---|
| **POLICY & STRATEGY** |||||||||
| Approve governance charter | **A** | R | C | C | I | I | I | I | I |
| Develop data policies | I | A | **R** | C | C | I | C | I | I |
| Approve data policies | C | **A** | R | C | I | I | I | I | I |
| Annual framework review | **A** | R | R | C | C | I | I | I | I |
| **ROLES & ACCOUNTABILITY** |||||||||
| Appoint Data Governance Lead | **A** | R | — | I | I | I | I | I | I |
| Appoint Data Owners | C | **A** | R | I | — | I | I | I | I |
| Appoint Data Stewards | I | I | C | I | **A/R** | — | I | I | I |
| Define role responsibilities | I | A | **R** | C | C | I | I | C | I |
| **DATA QUALITY** |||||||||
| Set quality standards | I | A | **R** | I | C | I | I | I | I |
| Monitor data quality | I | I | **A** | I | R | R | C | I | I |
| Resolve quality issues (domain) | I | I | C | I | **A** | R | I | I | I |
| Escalate critical quality issues | I | A | **R** | I | C | C | I | I | I |
| **COMPLIANCE** |||||||||
| Monitor regulatory changes | I | I | C | **R** | I | I | I | I | I |
| Conduct compliance audits | I | A | **R** | R | C | C | I | I | I |
| Respond to regulatory inquiries | C | A | C | **R** | I | I | I | I | I |
| Handle data subject requests | I | I | C | **R** | C | I | I | I | I |
| **ACCESS CONTROL** |||||||||
| Approve access requests | I | I | **A** | C | R | I | R | I | I |
| Provision / revoke access | I | I | C | I | I | I | **R** | I | I |
| Conduct quarterly access reviews | I | I | **A** | C | R | I | R | I | I |
| **TRAINING** |||||||||
| Design training curriculum | I | I | **A** | C | C | I | I | R | I |
| Deliver training | I | I | A | C | I | I | I | **R** | I |
| Track training completion | I | I | **R** | C | I | I | I | R | I |
| **INCIDENT MANAGEMENT** |||||||||
| Detect and report incident | I | I | I | I | I | I | I | I | **R** |
| Contain and assess incident | I | I | **A** | R | R | C | R | I | I |
| Notify regulatory authorities | C | **A** | C | **R** | I | I | I | I | I |
| Post-incident review | I | **A** | R | R | C | C | C | I | I |

---

## 5. Stakeholder Responsibilities Summary

### Data Governance Council
- Set the strategic direction for data governance at Nelmma
- Approve all governance policies and major framework changes
- Provide executive sponsorship and resource allocation
- Review quarterly governance reports and KPIs
- Resolve cross-functional data disputes

### Data Governance Lead
- Manage the day-to-day governance program
- Develop, maintain, and communicate governance policies
- Coordinate audit schedules and track remediation
- Maintain the governance documentation repository
- Report program status to the Council quarterly

### Data Protection Officer (DPO)
- Monitor compliance with Act 843, GDPR, and PIPL
- Handle all data subject access requests and complaints
- Lead breach response and regulatory notification
- Conduct data protection impact assessments
- Liaise with the Data Protection Commission of Ghana

### Data Owners
- Accept accountability for data quality within their domain
- Classify all data assets in their domain
- Approve access requests for domain data
- Assign and support Data Stewards
- Participate in governance meetings and audits

### Data Stewards
- Execute data quality checks and resolve issues
- Maintain metadata accuracy in the data catalog
- Monitor access usage within their domain
- Support training of end users on data standards
- Report quality and compliance issues to Data Owner

### Data Custodians (IT)
- Implement and maintain technical access controls (RBAC)
- Ensure secure storage, backup, and disaster recovery
- Maintain data lineage tracking systems
- Provision and revoke access per approved requests
- Support data breach containment and forensics

### End Users
- Handle data in accordance with their classification level
- Complete all mandatory governance training
- Report suspected data quality issues or breaches
- Comply with access control and data handling procedures
- Do not share access credentials or data outside approved channels

---

## 6. Governance Meeting Schedule

| Meeting | Participants | Frequency | Purpose |
|---|---|---|---|
| Governance Council Meeting | Council members + DG Lead | Quarterly | Strategy, policy approval, KPI review |
| Data Owner Sync | DG Lead + All Data Owners | Monthly | Quality issues, domain updates, escalations |
| Data Quality Review | DG Lead + Stewards | Monthly | Quality KPIs, data health dashboard review |
| Compliance Check-In | DG Lead + DPO | Monthly | Regulatory updates, incident review, audit prep |
| IT Governance Sync | DG Lead + IT Custodians | Monthly | Access reviews, system updates, security events |
| Training Review | DG Lead + HR | Quarterly | Training completion, curriculum updates |
| Annual Framework Review | Governance Council | Annually | Full framework assessment and update |
