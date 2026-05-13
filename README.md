# ✈️ NELMMA Aviation — Data Governance Framework

<div align="center">

![Status](https://img.shields.io/badge/Status-Active%20Implementation-brightgreen)
![Framework](https://img.shields.io/badge/Framework-DAMA--DMBOK%20%7C%20ISO%2038505-blue)
![Compliance](https://img.shields.io/badge/Compliance-Act%20843%20%7C%20GDPR%20%7C%20ISO%2027001-orange)
![Industry](https://img.shields.io/badge/Industry-Aviation%20%26%20Logistics-purple)
![Scope](https://img.shields.io/badge/Scope-Ghana%20%7C%20West%20Africa%20%7C%20International-teal)

**Enterprise-Grade Data Governance Framework for a Ghana-Based Aviation & Logistics Operator**

*Developed by the OMIS 312 Group Two — Data Governance Consulting Engagement*

</div>

---

## 📋 Table of Contents

- [Executive Summary](#-executive-summary)
- [Business Problem](#-business-problem)
- [Project Objectives](#-project-objectives)
- [Governance Framework Overview](#-governance-framework-overview)
- [Architecture Overview](#%EF%B8%8F-architecture-overview)
- [Key Framework Components](#-key-framework-components)
- [Governance Lifecycle](#-governance-lifecycle)
- [Stakeholder Roles & RACI](#-stakeholder-roles--raci)
- [Policies & Standards](#-policies--standards)
- [Regulatory Compliance Alignment](#-regulatory-compliance-alignment)
- [Implementation Roadmap](#-implementation-roadmap)
- [KPIs & Success Metrics](#-kpis--success-metrics)
- [Tools & Technologies](#-tools--technologies)
- [Repository Structure](#-repository-structure)
- [Business Impact](#-business-impact)
- [Recommendations](#-recommendations)
- [Lessons Learned](#-lessons-learned)
- [Team](#-team)

---

## 🎯 Executive Summary

This repository documents the end-to-end design and implementation of a **Data Governance Framework** for **Nelmma Aviation**, a Ghana-based non-scheduled aviation and logistics company with over 20 years of operational experience. Nelmma operates across air and sea freight, cargo consolidation, ground handling, and executive aviation services, with active markets spanning **Nigeria, Liberia, Mali, China, and Belgium** and expansion plans targeting Central Africa and Europe.

Despite its strong market presence, Nelmma's internal data governance infrastructure was dormant — policies existed on paper but lacked enforcement, roles were undefined, and there were no ongoing training programs or compliance monitoring mechanisms. This engagement was structured as a **consulting-style academic project**, simulating a real enterprise governance redesign.

The resulting framework is aligned with **DAMA-DMBOK**, **ISO 38505**, **ISO 27001**, **ISO 8000**, and **Ghana's Data Protection Act (Act 843)**, making it both internationally credible and locally compliant.

> **Project Course:** OMIS 312 — Data Governance  
> **Project Theme:** *"Developing a Robust Data Governance Framework for Public and Private Sector Transformation in Ghana"*  
> **Organization Type:** Private-sector, family-run SME transitioning to structured enterprise governance  
> **Duration:** Phased implementation over 1–6 years (short-, medium-, and long-term horizons)

---

## 🔴 Business Problem

### The Governance Vacuum

Nelmma Aviation entered this engagement with a governance framework that existed in name only. A diagnostic assessment revealed five critical failure areas:

| Problem Area | Finding | Business Risk |
|---|---|---|
| **Role Ambiguity** | No Data Owners, Stewards, or Custodians formally assigned | Accountability gaps; unresolved data disputes |
| **Inactive Framework** | Existing policies not reviewed, enforced, or communicated | Regulatory non-compliance with Act 843 |
| **Training Deficit** | One-time onboarding only; no executive data training | Inconsistent data practices across departments |
| **Leadership Disengagement** | CEO not involved in data compliance oversight | Governance vacuum; no enforcement from top |
| **No Compliance Monitoring** | No audit trail, no reporting mechanisms, no KPIs | Hidden data risks with no early warning system |

### Engagement Discovery Process

Before reaching Nelmma, the team navigated real-world consulting challenges:

1. **Alpha Company** — Declined due to sensitivity about exposing internal data practices
2. **ISSER** — Existing governance structures were too rigid to accommodate a redesign
3. **Nelmma Aviation** — Identified as an ideal partner: willing, growth-oriented, and openly acknowledging governance gaps

This mirrors genuine enterprise consulting dynamics, where client selection, trust-building, and stakeholder alignment precede any technical work.

---

## 🎯 Project Objectives

1. **Assess** the current state of data governance at Nelmma Aviation using structured interviews, surveys, and document review
2. **Design** a governance framework tailored to aviation & logistics data — cargo manifests, passenger records, customs data, financial records, partner integrations
3. **Align** the framework to international standards (DAMA-DMBOK, ISO 38505, ISO 27001, ISO 8000) and Ghanaian law (Act 843)
4. **Define** governance roles, responsibilities, and decision rights across all operational layers
5. **Develop** enforceable data policies covering quality, access, classification, retention, and ethics
6. **Establish** a training curriculum for staff and executive leadership
7. **Create** an implementation roadmap spanning 1–6 years with phased milestones
8. **Build** monitoring and audit mechanisms for continuous governance improvement

---

## 🏛️ Governance Framework Overview

The NELMMA Data Governance Framework is built on three foundational pillars:

```
┌──────────────────────────────────────────────────────────────┐
│                 NELMMA GOVERNANCE FRAMEWORK                  │
├───────────────┬───────────────────┬──────────────────────────┤
│   PEOPLE      │     PROCESS       │      TECHNOLOGY          │
│               │                   │                          │
│ • Gov. Council│ • Data Lifecycle  │ • Central Repository     │
│ • Data Owners │ • Policy Cycle    │ • Access Control Tools   │
│ • Stewards    │ • Audit Schedule  │ • Data Lineage Tracking  │
│ • Custodians  │ • Training Plan   │ • Compliance Dashboard   │
│ • End Users   │ • Risk Reviews    │ • Cargo/Flight Systems   │
└───────────────┴───────────────────┴──────────────────────────┘
```

### Standards Alignment Summary

| Standard | Governance Element Covered |
|---|---|
| **DAMA-DMBOK** | Governance Council, Metadata, Data Quality, Retention, Steward Roles |
| **ISO 38505** | Data governance decision rights, accountability, assurance |
| **ISO 27001** | Security Controls, Access Reviews, Breach Response, Training (Clause 7.2) |
| **ISO 8000** | Data Quality Principles, Interoperability Standards |
| **Ghana Act 843** | Legal Compliance, Data Subject Rights, Retention, Consent, DPO Requirement |
| **GDPR** | Cross-border data transfers (EU operations in Belgium/Liège) |
| **PIPL (China)** | Data handling for China-corridor operations |

---

## 🏗️ Architecture Overview

```
                        ┌─────────────────────────────┐
                        │   DATA GOVERNANCE COUNCIL    │
                        │  (CEO + Business Unit Leads) │
                        └──────────────┬──────────────┘
                                       │ Strategic Oversight
                    ┌──────────────────▼──────────────────┐
                    │         DATA GOVERNANCE LEAD         │
                    │   (Policy, Audit, Compliance Hub)    │
                    └────────┬────────────────┬───────────┘
                             │                │
               ┌─────────────▼───┐    ┌───────▼─────────────┐
               │   DATA OWNERS   │    │   DATA CUSTODIANS    │
               │ (Dept. Managers)│    │   (IT / Systems)     │
               └─────────────────┘    └──────────────────────┘
                             │                │
               ┌─────────────▼───────────────▼───────────────┐
               │              DATA STEWARDS                    │
               │  (Operational Accountability Per Domain)      │
               │  • Cargo & Freight  • Passenger Records       │
               │  • Customs & Compliance  • Finance & Partners │
               └──────────────────────────────────────────────┘
                                       │
                    ┌──────────────────▼──────────────────┐
                    │           DATA DOMAINS               │
                    │  Flight Ops | Cargo | Customs |      │
                    │  Passenger | Finance | HR | Partners │
                    └─────────────────────────────────────┘
```

---

## 🔧 Key Framework Components

### 1. Data Governance Committee
A cross-functional body comprising the CEO, department heads, and the Data Governance Lead. Responsible for approving policies, resolving disputes, and setting the data strategy.

### 2. Role Definitions
Clearly documented responsibilities for:
- **Data Owners** — Accountable for data within their business domain
- **Data Stewards** — Responsible for data quality and day-to-day governance
- **Data Custodians** — Technical managers of data storage and security systems
- **Data Protection Officer (DPO)** — Required under Ghana Act 843 and GDPR
- **End Users** — Trained on permissible data access and usage

### 3. Policy Suite
Comprehensive policies covering:
- Data Classification & Sensitivity Levels
- Access Control & Role-Based Permissions (RBAC)
- Data Retention & Disposal Schedules
- Privacy & Consent Management
- Breach Response & Notification Protocols
- Cross-Border Data Transfer (EU/China corridors)

### 4. Data Quality Standards (ISO 8000)
Dimensions tracked: **Accuracy, Completeness, Consistency, Timeliness, Validity, Uniqueness**

Applied across all data domains: cargo manifests, passenger records, customs filings, flight schedules, financial transactions.

### 5. Metadata & Master Data Management
Centralized metadata repository covering:
- Client master records
- Airport and route data
- Shipment tracking identifiers
- Aircraft and ground equipment data

### 6. Data Lineage
Tracks data flow end-to-end — from collection, through processing, to storage and disposal — enabling full audit traceability and error investigation.

### 7. Training & Awareness Program (ISO 27001 Clause 7.2)
- Role-specific training modules
- Executive governance awareness sessions
- Mandatory onboarding + quarterly refresher workshops
- E-learning modules on data ethics and privacy law

---

## 🔄 Governance Lifecycle

```
  ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
  │  DEFINE  │ ── │  ENABLE  │ ── │ ENFORCE  │ ── │ MONITOR  │
  │          │    │          │    │          │    │          │
  │ Policies │    │ Training │    │  Audits  │    │  KPIs &  │
  │  Roles   │    │  Tools   │    │  Access  │    │ Reviews  │
  │Standards │    │Workflows │    │ Controls │    │ Reports  │
  └──────────┘    └──────────┘    └──────────┘    └──────────┘
       │               │               │               │
       └───────────────┴───────────────┴───────────────┘
                              │
                    ┌─────────▼─────────┐
                    │   CONTINUOUS       │
                    │   IMPROVEMENT      │
                    │  (Annual Review)   │
                    └───────────────────┘
```

---

## 👥 Stakeholder Roles & RACI

| Activity | CEO | DG Lead | Data Owner | Data Steward | IT Custodian | HR/Training | End Users |
|---|---|---|---|---|---|---|---|
| Approve Governance Policies | **A** | R | C | I | I | I | I |
| Define Data Domains & Ownership | **A** | R | R | C | I | I | I |
| Monitor Data Quality | I | **A** | R | R | C | I | I |
| Conduct Compliance Audits | I | **A/R** | C | C | R | I | I |
| Manage Access Controls | I | A | C | I | **R** | I | I |
| Deliver Training Programs | C | A | I | I | I | **R** | I |
| Report Data Incidents | **A** | R | R | R | R | I | C |
| Review Framework Annually | **A** | R | C | C | C | C | I |

> **R** = Responsible | **A** = Accountable | **C** = Consulted | **I** = Informed

---

## 📜 Policies & Standards

### Policy Framework Structure

```
nelmma-dg-repo/
└── policies/
    ├── DG-POL-001_Data-Classification-Policy.md
    ├── DG-POL-002_Access-Control-Policy.md
    ├── DG-POL-003_Data-Retention-and-Disposal-Policy.md
    ├── DG-POL-004_Privacy-and-Consent-Policy.md
    ├── DG-POL-005_Data-Quality-Policy.md
    ├── DG-POL-006_Breach-Response-Policy.md
    ├── DG-POL-007_Cross-Border-Data-Transfer-Policy.md
    └── DG-POL-008_Metadata-Management-Policy.md
```

### Data Classification Matrix

| Classification Level | Description | Examples | Access |
|---|---|---|---|
| 🔴 **Confidential** | Highly sensitive, legal risk if exposed | Passport data, financial records, GSSA contracts | Executive + DPO only |
| 🟠 **Restricted** | Internal use; limited sharing | Cargo manifests, customer PII, employee HR records | Role-based (need-to-know) |
| 🟡 **Internal** | General business operations data | Flight schedules, route data, internal reports | All staff |
| 🟢 **Public** | Approved for external publication | Service descriptions, market presence, press releases | Anyone |

---

## 🌍 Regulatory Compliance Alignment

| Regulation | Jurisdiction | Key Requirements | Nelmma Application |
|---|---|---|---|
| **Ghana Data Protection Act (Act 843)** | Ghana | DPO appointment, consent, data subject rights | Primary compliance baseline |
| **GDPR** | EU / Belgium | Cross-border transfers, right to erasure, breach notification | Belgium & Liège corridor operations |
| **PIPL** | China | Localization, consent, data export restrictions | China warehouse & freight operations |
| **GCAA Regulations** | Ghana | Operational data standards for aviation | Flight operations & ground handling |
| **Customs Regulations** | Multi-market | Cargo documentation integrity | Freight forwarding & customs clearance |

---

## 🗺️ Implementation Roadmap

### Phase Overview

| Phase | Timeline | Focus | Key Deliverables |
|---|---|---|---|
| **Phase 1: Foundation** | Months 1–2 | Governance Structure | Committee formation, role assignments, governance charter |
| **Phase 2: Policy Development** | Months 3–4 | Policy Suite | All 8 data governance policies, data classification matrix |
| **Phase 3: Training Rollout** | Months 4–6 | Capability Building | Role-specific training, executive sessions, onboarding update |
| **Phase 4: System Integration** | Months 6–9 | Technology Enablement | Central repository, access controls, data lineage tracking |
| **Phase 5: Monitoring & Audit** | Months 9–12 | Ongoing Governance | Quarterly audits, KPI dashboard, first annual review |
| **Phase 6: Scale & Optimize** | Years 2–6 | Regional Expansion | Framework extension to new markets (Central Africa, UK, EU) |

### Detailed Roadmap by Year

**Year 1–2 (Setup & Enablement)**
- ✅ Appoint Data Governance Lead and establish committee
- ✅ Define and document all data domains and ownership
- ✅ Draft, review, and publish all core data policies
- ✅ Deploy RBAC-based access control system
- ✅ Launch first training cohort for all staff

**Year 2–3 (Integration)**
- 📋 Implement centralized metadata repository
- 📋 Integrate governance tools with cargo and flight management systems
- 📋 Establish data lineage tracking for all critical data flows
- 📋 First full compliance audit under Act 843

**Year 3–4 (Governance)**
- 📋 Begin quarterly audit cycle and stakeholder reporting
- 📋 Introduce data governance maturity assessments
- 📋 Expand training to include regulatory changes and emerging risks

**Year 4–6 (Optimization & Scale)**
- 📋 Extend framework to new markets: UK, Central Africa, China hub
- 📋 Automate compliance monitoring and reporting
- 📋 Pursue formal ISO 27001 certification
- 📋 Build data governance playbook for international subsidiaries

---

## 📊 KPIs & Success Metrics

| KPI Category | Metric | Target | Measurement Frequency |
|---|---|---|---|
| **Policy Adoption** | % of staff completing governance training | ≥ 95% | Quarterly |
| **Data Quality** | Data accuracy rate across core domains | ≥ 98% | Monthly |
| **Compliance** | % of data requests fulfilled within SLA | ≥ 90% | Monthly |
| **Incident Response** | Mean time to report data breach | < 24 hours | Per incident |
| **Audit Performance** | % of audit findings resolved within 30 days | ≥ 85% | Quarterly |
| **Role Coverage** | % of data assets with assigned Data Owner | 100% | Bi-annually |
| **Access Control** | % of data assets with enforced RBAC | 100% | Quarterly |
| **Stakeholder Confidence** | Internal governance satisfaction score | ≥ 4.0 / 5.0 | Annually |

---

## 🛠️ Tools & Technologies

| Category | Tool / System | Purpose |
|---|---|---|
| **Governance Standards** | DAMA-DMBOK, ISO 38505 | Framework methodology |
| **Security Standards** | ISO 27001, ISO 8000 | Security controls and data quality |
| **Data Repository** | Centralized Secure Storage (TBD cloud/on-prem) | Single source of truth |
| **Access Management** | RBAC System | Role-based access enforcement |
| **Data Lineage** | Data lineage tracking tool | Audit trail and traceability |
| **Compliance Monitoring** | Audit dashboard | Policy adherence monitoring |
| **Operations** | Cargo tracking, passenger management systems | Operational data sources |
| **Training Delivery** | LMS (e-learning platform) | Staff and executive training |
| **Documentation** | GitHub + Markdown | Version-controlled governance documentation |

---

## 📁 Repository Structure

```
nelmma-aviation-data-governance/
│
├── README.md                           # This file — project overview
├── BUSINESS_CASE.md                    # Full business justification and ROI analysis
├── GOVERNANCE_CHARTER.md               # Official governance charter document
├── CHANGELOG.md                        # Version history of framework updates
├── .gitignore                          # Ignore rules for sensitive data
│
├── documentation/
│   ├── executive-summary.md
│   ├── background-and-context.md
│   ├── governance-challenges.md
│   ├── stakeholder-analysis.md
│   └── framework-overview.md
│
├── policies/
│   ├── DG-POL-001_Data-Classification-Policy.md
│   ├── DG-POL-002_Access-Control-Policy.md
│   ├── DG-POL-003_Data-Retention-and-Disposal-Policy.md
│   ├── DG-POL-004_Privacy-and-Consent-Policy.md
│   ├── DG-POL-005_Data-Quality-Policy.md
│   ├── DG-POL-006_Breach-Response-Policy.md
│   ├── DG-POL-007_Cross-Border-Data-Transfer-Policy.md
│   └── DG-POL-008_Metadata-Management-Policy.md
│
├── governance-model/
│   ├── RACI-Matrix.md
│   ├── Data-Ownership-Matrix.md
│   ├── Governance-Committee-Charter.md
│   ├── Escalation-Process.md
│   └── Role-Definitions.md
│
├── architecture/
│   ├── framework-architecture.md
│   ├── data-domains.md
│   ├── governance-hierarchy.md
│   └── technology-stack.md
│
├── diagrams/
│   ├── governance-hierarchy-diagram.png
│   ├── data-lifecycle-flow.png
│   ├── compliance-heatmap.png
│   ├── maturity-model.png
│   └── implementation-roadmap-visual.png
│
├── compliance/
│   ├── Act-843-Alignment.md
│   ├── GDPR-Alignment.md
│   ├── PIPL-Alignment.md
│   ├── ISO-27001-Controls.md
│   └── Regulatory-Matrix.md
│
├── data-quality/
│   ├── Data-Quality-Framework.md
│   ├── Quality-Dimensions.md
│   ├── Quality-KPI-Tracker.md
│   └── Quality-Audit-Template.md
│
├── metadata-management/
│   ├── Metadata-Standards.md
│   ├── Master-Data-Domains.md
│   └── Data-Dictionary-Template.md
│
├── security/
│   ├── Access-Control-Framework.md
│   ├── Data-Classification-Matrix.md
│   ├── Breach-Response-Runbook.md
│   └── Encryption-Standards.md
│
├── workflows/
│   ├── Data-Request-Workflow.md
│   ├── Incident-Response-Workflow.md
│   ├── Policy-Review-Workflow.md
│   └── Audit-Workflow.md
│
├── templates/
│   ├── Data-Governance-Policy-Template.md
│   ├── Data-Stewardship-Roles-Template.md
│   ├── Risk-Assessment-Template.md
│   ├── KPI-Tracking-Template.md
│   ├── Governance-Charter-Template.md
│   └── Training-Plan-Template.md
│
├── reports/
│   ├── Phase-1-Assessment-Report.md
│   ├── Governance-Gap-Analysis.md
│   └── Stakeholder-Engagement-Summary.md
│
├── presentations/
│   └── NELMMA_Framework_Presentation.pptx
│
└── portfolio/
    ├── PORTFOLIO_CASE_STUDY.md
    ├── LINKEDIN_DESCRIPTION.md
    └── RESUME_BULLETS.md
```

---

## 💼 Business Impact

### Operational Efficiency
A structured governance framework eliminates the data ambiguity that slows operations. When cargo, flight, and customs teams work from a single source of truth, scheduling errors decrease, handoffs improve, and delays are reduced.

### Regulatory Risk Reduction
Without governance, Nelmma faces material risk of fines under Ghana's Data Protection Act (Act 843) and GDPR for its Belgium corridor. The framework provides the audit trail, consent mechanisms, and breach notification protocols required by law.

### Stakeholder & Partner Confidence
Airlines, GSSA partners, customs authorities, and international logistics partners increasingly require demonstrated data governance maturity before entering agreements. This framework positions Nelmma as a trustworthy, enterprise-grade partner.

### Competitive Differentiation
In West Africa's aviation sector, few SMEs have a formalized, standards-aligned governance framework. Nelmma's implementation creates a genuine differentiator — particularly valuable as it pursues ISO certification and international expansion.

### Scalability
The framework is designed to scale with the business — from a Ghana-centric operation today to a multi-country, multi-corridor logistics network across Central Africa, UK, Europe, and China.

---

## ✅ Recommendations

1. **Appoint a Dedicated Data Governance Lead** — A full-time role responsible for day-to-day policy enforcement, training coordination, and audit management
2. **Establish the Data Governance Committee** within Month 1 — With CEO endorsement and cross-departmental representation
3. **Prioritize Act 843 Compliance** — Appoint a DPO, complete a data mapping exercise, and implement consent mechanisms before any system integrations
4. **Invest in Training as Infrastructure** — Move from one-time onboarding to a continuous learning culture with quarterly data governance touchpoints
5. **Adopt Data Lineage from Day One** — Tracking data flow from source to use enables faster error diagnosis and more credible audits
6. **Use Phased Technology Adoption** — Avoid over-investing in tools before governance processes are stable; let process maturity drive tool selection
7. **Engage External Regulators Early** — Proactive engagement with the Data Protection Commission and GCAA builds trust and reduces enforcement risk

---

## 🎓 Lessons Learned

| Lesson | Context | Takeaway |
|---|---|---|
| **Governance buy-in precedes design** | CEO and leadership must champion the framework before implementation begins | Without executive sponsorship, policies go unenforced |
| **Tailoring beats templating** | Generic frameworks don't fit Nelmma's non-scheduled, multi-market model | Aviation-specific data domains required custom role design |
| **Partner selection is governance work** | Rejections from Alpha Company and ISSER shaped the engagement | Client fit analysis is as critical as framework design |
| **Training is underestimated** | One-time onboarding created false confidence at Nelmma | Continuous training is a governance pillar, not an afterthought |
| **Compliance is multi-jurisdictional** | Nelmma's markets span 5+ regulatory environments | Governance frameworks must map every applicable law |

---

## 👨‍💼 Team

| Name | Student ID |
|---|---|
| Samson Awinsone Ayamga | 11219536 |
| Abraham Yartey | 11019809 |
| Roderick Faakye Mireku | 11297176 |
| Nana Kane Bruce Eshun | 11117122 |
| Clifford Mante Yeboah | 11235040 |
| Lamidi Okyere | 11209186 |
| Hans Nmashie | 11294210 |
| Addo Mariam Pokuaa | 11016054 |
| Kelvin Larbi Yeboah | 11169462 |
| Hajara Abdul Mumin | 11333351 |
| Nketsiah Obed Anthony | 11296843 |

**Course:** OMIS 312 — Data Governance  
**Institution:** University of Ghana Business School (UGBS)  
**Project Theme:** *Developing a Robust Data Governance Framework for Public and Private Sector Transformation in Ghana*

---

## 📚 References

- DAMA International. (2017). *DAMA-DMBOK: Data Management Body of Knowledge* (2nd ed.). Technics Publications.
- Ghana Data Protection Commission. (2012). *Data Protection Act, 2012 (Act 843)*. Government of Ghana.
- ISO/IEC 27001:2013 — Information Security Management Systems
- ISO 8000 — Data Quality Principles
- ISO 38505 — Governance of Data
- Khatri, V., & Brown, C. V. (2010). Designing data governance. *Communications of the ACM*, 53(1), 148–152.
- Smallwood, R. F. (2019). *Information Governance: Concepts, Strategies, and Best Practices* (2nd ed.). Wiley.

---

<div align="center">

*This project represents a real-world consulting engagement conducted as part of OMIS 312 coursework.*  
*All framework content is based on primary stakeholder data collected from Nelmma Aviation.*

**⭐ If this framework helped your understanding of data governance, please star this repository.**

</div>
