# Awesome-Dependency-Update-Automation

Markdown
# 🚀 Awesome-Account-Reconciliation-Platforms


## 🌟 Top Account Reconciliation Platforms Ecosystem


Curated List of SaaS Products & Open-Source GitHub Projects  
Focused on **Account Reconciliation, Transaction Matching, Bank Reconciliation, Balance-Sheet Reconciliation, Financial Close, Exception Management & Accounting Automation**


**Last updated: August 2026**


This repository tracks notable **SaaS/Hosted Platforms** and **Open-Source Projects** for Account Reconciliation.


Account reconciliation platforms help finance and accounting teams reconcile balance-sheet accounts, bank accounts, subledgers, payments, intercompany balances and other financial data sources; automate matching; identify exceptions; maintain audit trails; and accelerate the financial close.


**Examples** include BlackLine, Trintech, AutoRek, ReconArt, FloQast, OneStream, Cadency, Fiserv Frontier, Duco and SmartStream.


> **Open-source emphasis:** There are considerably fewer mature open-source equivalents to enterprise platforms such as BlackLine, Cadency and SmartStream than there are commercial products. Therefore, the Open-Source section includes both dedicated reconciliation engines and open-source accounting, ledger, bank-reconciliation, record-linkage and transaction-matching projects that can be combined into a self-hosted reconciliation stack.


---


## 📋 Table of Contents


- [☁️ SaaS/Hosted Platforms](#️-saashosted-platforms)
- [💻 Open-Source GitHub Projects](#-open-source-github-projects)
- [🧩 Open-Source Accounting & Reconciliation Platforms](#-open-source-accounting--reconciliation-platforms)
- [🔧 Open-Source Matching & Reconciliation Engines](#-open-source-matching--reconciliation-engines)
- [📊 Open-Source Financial Infrastructure](#-open-source-financial-infrastructure)
- [🏗️ Building an Open-Source Reconciliation Stack](#️-building-an-open-source-reconciliation-stack)
- [🔍 Commercial vs Open-Source](#-commercial-vs-open-source)
- [🤝 How to Contribute](#-how-to-contribute)
- [⚠️ Disclaimer](#️-disclaimer)


---


# ☁️ SaaS/Hosted Platforms


| Platform | Description | Pricing | Free Tier |
|---|---|---|---|
| **BlackLine** | Enterprise financial-close and accounting automation platform covering account reconciliation, transaction matching, journal entries, intercompany accounting and close management. | Custom / Contact Sales | N/A |
| **Trintech** | Financial-close automation platform covering account reconciliation, transaction matching, journal entries, intercompany accounting and close management through its Cadency and Adra product families. | Custom / Contact Sales | N/A |
| **AutoRek** | Financial-data management and reconciliation platform used by banks, asset managers, insurers and other financial institutions for complex reconciliation, data transformation and regulatory workflows. | Custom / Contact Sales | N/A |
| **ReconArt** | Enterprise reconciliation platform supporting account reconciliation, transaction matching, exception management, certification and financial-close processes. | Custom / Contact Sales | N/A |
| **FloQast** | Financial-close management platform with account reconciliations, close checklists, workflow, documentation and accounting automation. | Custom / Contact Sales | N/A |
| **OneStream** | Corporate performance management platform with financial-close, consolidation and account-reconciliation capabilities. | Custom / Contact Sales | N/A |
| **Cadency** | Trintech's enterprise financial-close platform for reconciliation, transaction matching, journal-entry management, intercompany accounting and controls. | Custom / Contact Sales | N/A |
| **Fiserv Frontier Reconciliation** | Enterprise reconciliation and certification platform designed for high-volume banking, payment and inter-system reconciliation. | Custom / Contact Sales | N/A |
| **Duco** | Cloud-native data reconciliation platform focused on complex, high-volume financial-data matching, automation and exception management. | Custom / Contact Sales | N/A |
| **SmartStream TLM Reconciliation** | Enterprise transaction-lifecycle management platform specializing in high-volume cash, securities, trade and financial-data reconciliation. | Custom / Contact Sales | N/A |
| **Trintech Adra** | Financial-close suite aimed particularly at mid-market organizations, providing account reconciliation, transaction matching, close management and journal automation. | Custom / Contact Sales | N/A |
| **BlackLine Account Reconciliations** | Dedicated account-reconciliation capability for standardizing, automating and controlling balance-sheet account substantiation. | Custom / Contact Sales | N/A |
| **BlackLine Transaction Matching** | High-volume transaction-matching solution for matching financial records, identifying exceptions and automating reconciliation. | Custom / Contact Sales | N/A |
| **Trintech CadencyDirect** | Financial-close and reconciliation capabilities integrated into enterprise workflow environments, including reconciliation, matching and close processes. | Custom / Contact Sales | N/A |
| **OneStream Account Reconciliations** | Account-reconciliation functionality embedded within OneStream's broader CPM, consolidation and financial-close environment. | Custom / Contact Sales | N/A |
| **FloQast Reconciliation Management** | Reconciliation capabilities integrated into FloQast's broader close-management environment. | Custom / Contact Sales | N/A |
| **SolveXia** | No-code automation platform used for financial-data processing, reconciliation, variance analysis and accounting workflows. | Custom / Contact Sales | Varies |
| **HighRadius Account Reconciliation** | Finance automation platform providing reconciliation, matching, close management and accounting automation capabilities. | Custom / Contact Sales | N/A |
| **Numeric** | Modern financial-close platform providing account reconciliation, close management and accounting workflows. | Custom / Contact Sales | Varies |
| **Adra Matcher** | Transaction-matching functionality for automating financial-record matching and identifying exceptions. | Custom / Contact Sales | N/A |
| **Adra Balancer** | Balance-sheet reconciliation and certification functionality for accounting teams. | Custom / Contact Sales | N/A |


---


# 💻 Open-Source GitHub Projects


## 🥇 Dedicated Reconciliation Engines


### [Settler](https://github.com/Settler/settler)


Open-source reconciliation infrastructure designed to match financial records across banks, Stripe, ERPs and ledgers.


Key capabilities include:


- Deterministic reconciliation
- Configurable matching rules
- Multi-source joins
- Field-level tolerances
- Mismatch detection
- Evidence generation
- Reconciliation runs
- CLI
- TypeScript SDK
- Self-hosting
- Audit-oriented evidence


Settler is one of the most directly relevant modern open-source projects for building a BlackLine/Duco-style reconciliation engine. The project describes its core, CLI, SDK and evidence model as Apache 2.0 licensed. 


---


### [Lerian Matcher](https://github.com/LerianStudio/matcher)


Open-source transaction-reconciliation engine designed for financial systems.


Useful capabilities include:


- Transaction matching
🧠 Matching Strategies

A sophisticated reconciliation engine should progressively apply different matching strategies.

Matching Strategy	Example
Exact Match	Amount + Date + Transaction ID
Reference Match	Invoice / Payment Reference
Amount Match	Exact amount
Tolerance Match	Amount within configured tolerance
Date Tolerance	Date within ±N days
Fuzzy Match	Similar descriptions
Composite Match	Amount + Currency + Date + Reference
One-to-Many	One bank transaction → multiple ledger records
Many-to-One	Multiple transactions → one settlement
Many-to-Many	Multiple records on both sides
Aggregation Match	Several transactions = one settlement
Rule-Based Match	Configurable business rules
Probabilistic Match	Confidence-based record linkage
ML Match	Learned from historical reconciliation decisions
Human-in-the-Loop	Low-confidence records routed for review
🔄 Typical Reconciliation Workflow
Import
  ↓
Normalize
  ↓
Deduplicate
  ↓
Exact Match
  ↓
Rule-Based Match
  ↓
Tolerance Match
  ↓
Fuzzy / Probabilistic Match
  ↓
Aggregation / Split Matching
  ↓
Exception Detection
  ↓
Human Review
  ↓
Approval
  ↓
Certification
  ↓
Audit Trail
  ↓
Financial Close
📦 Open-Source Project Categories
Category	Strong Open-Source Options
Dedicated Reconciliation	Settler, Lerian Matcher, OpenRec
Bank Reconciliation	OCA Account Reconcile, Pavit Bank Reconciliation, Mint
Accounting ERP	ERPNext, Odoo, LedgerSMB
Accounting	Beancount, GnuCash, hledger, Ledger
Matching	Splink, Dedupe, RapidFuzz, Record Linkage
Financial Ledger	TigerBeetle, Medici
Payment Infrastructure	jPOS
Automated Finance	n8n + PostgreSQL reconciliation workflows
AI-Assisted Reconciliation	Agent-for-accounting and similar emerging projects
🏆 Recommended Open-Source Combinations
🥇 Enterprise-Style Reconciliation Engine
Settler
    +
PostgreSQL
    +
ERP / Bank / PSP Connectors
    +
Custom Matching Rules
    +
Splink / RapidFuzz
    +
Exception Management UI
    +
Audit Evidence

This is probably the closest architectural direction for building an open-source Duco/AutoRek-style reconciliation engine.

🥈 ERP-Centric Reconciliation
ERPNext / Odoo
       +
OCA Account Reconcile
       +
Bank Connectors
       +
Custom Matching Rules
       +
Exception Workflow

Best when the accounting system itself is the center of the architecture.

🥉 Developer-First Accounting
Beancount
    +
beancount-import
    +
Python
    +
RapidFuzz
    +
Splink
    +
PostgreSQL

Best for programmable accounting and developer-controlled reconciliation.

💳 Payment Reconciliation
Stripe / PayPal / Square / ACH
             ↓
       n8n / API Ingestion
             ↓
       PostgreSQL Ledger
             ↓
      Matching Engine
             ↓
       Fee / Refund Logic
             ↓
       Exception Queue
             ↓
       Accounting / ERP

The open-source Multi-Processor Payment Reconciliation project provides a useful reference implementation for this architecture.

🔍 Commercial vs Open-Source
Capability	SaaS / Enterprise	Open Source
Account Reconciliation	✅	✅
Bank Reconciliation	✅	✅
Transaction Matching	✅	✅
Balance-Sheet Certification	✅	⚠️
Intercompany Reconciliation	✅	⚠️
Multi-Way Matching	✅	⚠️
Exception Management	✅	⚠️
Approval Workflow	✅	⚠️
Audit Trail	✅	✅
Evidence Management	✅	⚠️
Financial Close	✅	⚠️
AI-Assisted Matching	✅	⚠️
Fuzzy Matching	✅	✅
Probabilistic Matching	✅	✅
ERP Connectors	✅	Varies
Bank Connectivity	✅	Varies
Regulatory Controls	Strong	Must be configured
Self-Hosting	Usually ❌	✅
Source-Code Access	❌	✅
Customization	High	Very High
Implementation Effort	Lower	Higher
Infrastructure Ownership	Vendor	Customer
Enterprise Support	✅	Community / Commercial Services
🧩 The Open-Source Gap

The commercial market generally offers a single integrated control plane combining:

Account reconciliation

Transaction matching

Bank reconciliation

Intercompany reconciliation

Balance-sheet certification

Exception management

Workflow

Approvals

Audit evidence

Financial close

ERP integrations

Bank integrations

Role-based access

Segregation of duties

Reporting

Dashboards

AI-assisted matching

Open source is currently much more fragmented.

The closest practical architecture is therefore:

                    ┌─────────────────┐
                    │ Accounting / GL │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │ Data Ingestion  │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │ Normalization   │
                    └────────┬────────┘
                             │
             ┌───────────────▼───────────────┐
             │       MATCHING ENGINE         │
             │                               │
             │ Settler / Lerian / Custom     │
             │ Splink / RapidFuzz            │
             └───────────────┬───────────────┘
                             │
                    ┌────────▼────────┐
                    │   Exceptions    │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │ Review / Approve│
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │ Audit Evidence  │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │ Financial Close │
                    └─────────────────┘

This fragmentation itself represents an opportunity for open-source financial infrastructure: an integrated, self-hosted reconciliation control plane combining matching, evidence, exception management, workflow and financial-close capabilities could become a genuine open-source alternative to portions of BlackLine, Cadency, Duco and AutoRek.

📈 Account Reconciliation Technology Stack
┌──────────────────────────────────────────────┐
│                 USER LAYER                   │
│ CFO / Controller / Accountant / Auditor      │
└───────────────────────┬──────────────────────┘
                        │
┌───────────────────────▼──────────────────────┐
│              WORKFLOW LAYER                  │
│ Review / Approve / Certify / Escalate        │
└───────────────────────┬──────────────────────┘
                        │
┌───────────────────────▼──────────────────────┐
│            RECONCILIATION LAYER              │
│ Matching / Exceptions / Tolerance / Rules    │
└───────────────────────┬──────────────────────┘
                        │
┌───────────────────────▼──────────────────────┐
│                DATA LAYER                    │
│ ERP / Bank / PSP / GL / Subledger / CSV     │
└───────────────────────┬──────────────────────┘
                        │
┌───────────────────────▼──────────────────────┐
│              LEDGER LAYER                    │
│ Double Entry / Transaction Store / Audit     │
└──────────────────────────────────────────────┘
🌍 Open-Source Opportunity Areas

The most interesting areas for future open-source projects include:

 Universal bank-statement reconciliation

 ERP-to-bank reconciliation

 Payment-processor reconciliation

 Intercompany reconciliation

 Multi-way transaction matching

 One-to-many / many-to-one matching

 Subset-sum reconciliation

 AI-assisted reconciliation

 Human-in-the-loop exception management

 Automated reconciliation certification

 Immutable reconciliation evidence

 Financial-close orchestration

 Open reconciliation APIs

 ISO 20022 reconciliation

 CAMT.053 / CAMT.054 reconciliation

 MT940 reconciliation

 Open banking reconciliation

 Reconciliation-as-code

 Self-hosted reconciliation control planes

 Open-source alternatives to BlackLine / Cadency / Duco

🤝 How to Contribute

Fork the repository.

Add or update entries in README.md.

Keep SaaS/Hosted Platforms and Open-Source projects separate.

Prefer official websites and GitHub repositories.

For open-source projects, include the license where practical.

Clearly distinguish between:

Dedicated reconciliation platforms

Accounting systems with reconciliation

Transaction-matching engines

Record-linkage libraries

Financial ledger infrastructure

Avoid adding abandoned projects unless they have significant historical relevance.

Submit a Pull Request with a short explanation.

Contributions are especially welcome for open-source reconciliation engines, bank-reconciliation applications, financial matching algorithms, accounting platforms, payment-reconciliation workflows and self-hosted alternatives to enterprise financial-close platforms.

⚠️ Disclaimer

This is a community-curated list and is not exhaustive or an endorsement.

Commercial product capabilities, ownership and packaging can change over time.

Open-source projects differ substantially in scope.

Some projects listed here are complete accounting applications; others are specialized reconciliation engines, modules, libraries or infrastructure components.

A matching library should not be interpreted as a complete enterprise replacement for BlackLine, Cadency, AutoRek, Duco or SmartStream.

Financial reconciliation systems should be implemented with appropriate accounting controls, auditability, access controls and segregation of duties.

Always verify the current license, project activity, security posture and production readiness before adopting an open-source project.

Financial systems should be validated against the applicable accounting, regulatory and organizational requirements.

Made for CFOs, controllers, accountants, auditors, finance teams, fintech engineers, banks, payment companies, ERP teams and developers building open financial infrastructure.

⭐ Star the repository if you find it useful.

Let's make account reconciliation more open, automated, auditable and transparent.
