ISO/IEC 27001:2022 · Clause 4 · Study notes

# ISMS-SCP-001: Context and Scope

How to build the first document of an ISMS: Understanding the organisation, its interested parties, and where the ISMS starts and stops. Each section gives a general method you can apply to any organisation, followed by a worked example from my notes.

Doc ID**ISMS-SCP-001**

Clauses**4.1 · 4.2 · 4.3**

Feeds into**6.1 · 6.2 · 9.3**

Review**Annual + MR**

Purple: Concept explained simply Blue: What the standard requires Orange: Auditor tip / common mistake Green: ISO 27001 text (reference) Dashed: Worked example from my notes

[Big picture](#big-picture) [1 Purpose](#purpose) [2 Issues (4.1)](#issues) [3 Interested parties (4.2)](#parties) [4 Scope (4.3)](#scope) [5 Review](#review) [Check yourself](#check) [ISO 27001 text](#norm)

## The big picture

Concept

Clause 4 answers three questions before any control is chosen. **Who are we and what is happening around us?** (4.1). **Who cares about our information security, and what do they want?** (4.2). **So what exactly are we protecting?** (4.3). Everything later in the ISMS (risk assessment, objectives, controls) builds on these answers.

**4.1**Issues

+

**4.2**Interested parties

→

**4.3**Scope

→

**6.1**Risks & opportunities

→

**6.2**Objectives

→

**9.3**Management review

↺ back to 4.1

Auditor tip

**Document all three: Issues (4.1), interested parties (4.2) and scope (4.3).** Clause 4.3 states it directly for the scope: "The scope shall be available as documented information." For 4.1 and 4.2, the need to document comes from other clauses: 7.5.1 b, Annex A 5.31 and 9.3.2 b/c (explained in "Check yourself" below). In practice, one combined context-and-scope document covers all three.

01

## Purpose

A short paragraph saying why the document exists. Example wording:

This document records the internal and external issues and the interested parties relevant to the Company's information security, and defines the boundaries and applicability of the ISMS, in line with ISO/IEC 27001:2022 clauses 4.1 to 4.3.

Concept

Keep the purpose to two or three sentences. Its job is to tell a reader (or auditor) which clauses this document satisfies.

02

## Internal and external issues

4.1

Standard requires

The organisation determines the external and internal issues that are relevant to its purpose and that affect its ability to achieve the intended outcomes of the ISMS. Since Amendment 1 (2024), it must also determine whether **climate change** is a relevant issue.

Concept: How ISO updates a standard

ISO doesn't reissue the whole standard for a small change. It publishes an **amendment** (Amd): A short, separate document that adds or changes specific clauses. You then read the two together, written as **ISO/IEC 27001:2022 + Amd 1:2024**.

- **Amendment (Amd):** Adds or changes requirements. Example: Amd 1:2024 added the climate change text to 4.1 and 4.2.
- **Technical Corrigendum (Cor):** Only fixes errors in the text. Example: ISO 27001:2013 had Cor 1:2014 and Cor 2:2015.
- **New edition:** A full rewrite when the changes are big. Example: 2013 → 2022.

Tip: When you buy or check the standard, always ask "are there amendments?" so you're reading the current requirements.

Concept

An "issue" is any condition, inside or outside the company, that could help or hurt information security. **External** = Things you cannot control (laws, threats, market). **Internal** = Things you can (structure, people, technology, culture).

### How to identify the issues for any organisation

1. Hold a short workshop with top management and the heads of IT, HR, Legal and Operations.
2. Collect inputs: Business strategy, organisation chart, client contracts, list of applicable laws, previous incidents and audit findings, the IT landscape.
3. Go through each external category (laws, market, threats, suppliers, technology, environment) and each internal one (structure, people, processes, technology, culture, resources).
4. For each issue, write down its impact on information security and how the ISMS responds (see Option C below).
5. Get the list approved by management and review it at least once a year.

| Type | Areas to check in every organisation |
| --- | --- |
| External | Laws and regulations that apply (data protection, sector rules, national cyber laws); client and market expectations; the threat landscape; key suppliers and cloud dependency; economic conditions; environment and climate |
| Internal | Organisation structure and governance; workforce model (office, hybrid, remote); technology and hosting; processes and documentation maturity; security culture; budget, people and skills |

Worked example

- **External:** Regulatory (GDPR, Cap. 586, NIS2, DORA), market and client expectations, threat landscape, reliance on cloud.
- **Internal:** Organisation structure, hybrid workforce, Azure hosting, culture, resources.

Three formats work. Pick one, or combine PESTLE (external) with SWOT (both).

### Option A: PESTLE (external issues)

Concept

PESTLE is a checklist of six lenses so you don't forget a category of external issue: Political, Economic, Social, Technological, Legal, Environmental.

| Category | General European examples |
| --- | --- |
| Political | EU digital sovereignty push (preference for EU cloud providers); geopolitical tension raising state-sponsored cyber threats; sanctions affecting suppliers in certain countries |
| Economic | Inflation squeezing security budgets; cyber insurance premiums rising and insurers demanding controls (MFA, backups); shortage of security professionals in the EU labour market |
| Social | Hybrid and remote work as the norm; growing public awareness of privacy; customers expecting fast breach notification |
| Technological | Cloud dependency (AWS, Azure, Google); AI-generated phishing and deepfakes; ransomware-as-a-service; legacy systems in hospitals and manufacturing |
| Legal | GDPR (all sectors); NIS2 (essential and important entities, e.g. energy, health, transport, digital infrastructure); DORA (financial entities and their ICT providers); EU AI Act; Cyber Resilience Act (products with digital elements); national laws transposing NIS2 |
| Environmental | Climate change: Floods, heatwaves affecting data centres, energy price volatility, sustainability reporting (CSRD) |

Auditor tip

The 2024 amendment requires you to **decide whether** climate change is relevant, not to declare it relevant. If you conclude it isn't, write down why. Saying nothing at all is the finding.

### Option B: SWOT (internal + external)

Concept

SWOT splits issues on two axes. Rows: **Internal** vs **external**. Columns: **Helpful** vs **harmful**. Strengths and weaknesses are internal; opportunities and threats are external. Example for a mid-sized European SaaS company:

|  | Helpful | Harmful |
| --- | --- | --- |
| Internal | **Strengths:** Cloud-native architecture, security-aware engineering team, existing GDPR programme | **Weaknesses:** Small security team, undocumented processes, shadow IT, weak asset inventory |
| External | **Opportunities:** Certification opens enterprise and public-sector tenders; NIS2/DORA clients look for compliant suppliers | **Threats:** Ransomware, supply chain attacks, new regulation with high fines, key supplier failure |

The same grid looks different in other sectors. Every organisation has all four quadrants, so each example below is complete:

| Sector | Strength | Weakness | Opportunity | Threat |
| --- | --- | --- | --- | --- |
| Hospital | Clinical staff trust and established procedures | Legacy medical devices that can't be patched | Digital health funding for modernisation | Ransomware disrupting patient care |
| Bank | Mature risk culture | Complex legacy core banking | DORA programme budget drives security improvements | DORA supervisory scrutiny and third-party concentration risk |
| Manufacturer | Strong safety culture and disciplined change control on the production floor | OT networks connected to IT | Industry 4.0 projects allow security to be designed in from the start | Production stoppage from an attack |

### Option C: Simple issues table

Concept

This is the format auditors like most, because each issue shows its **impact** and **how the ISMS responds**. That last column is what proves the context actually drives your controls.

| Issue | Int / Ext | Impact on the ISMS | How it is addressed |
| --- | --- | --- | --- |
| Subject to NIS2 as an important entity | External | Mandatory risk management measures, 24-hour early warning for significant incidents | Incident Management Policy, risk methodology, legal register |
| Main platform hosted on a public cloud provider | Internal | Availability and security depend on a third party | Supplier and Cloud Security Policies, shared responsibility model |
| Shortage of skilled security staff | External | Risk of single points of knowledge | Competence matrix, documented procedures, managed service provider |
| Large share of staff working remotely | Internal | Larger attack surface, endpoint risk | Remote Working Policy, endpoint controls, awareness training |
| Climate-related heatwaves and floods | External | Possible data centre or office disruption | Business continuity plan, multi-region hosting |

Common mistake

Copying a generic list that could describe any company. An auditor will ask "how does this issue show up in your risk register?" If an issue has no link to a risk, control or objective, it is decoration.

03

## Interested parties and their requirements

4.2

Standard requires

1. Determine the interested parties relevant to the ISMS.
2. Determine their relevant requirements.
3. Determine which of those requirements will be addressed through the ISMS. **(new in 2022)**

Concept

An interested party (stakeholder) is anyone who can affect, be affected by, or believe they are affected by your information security. Point (c) exists because not every requirement belongs to the ISMS. A client's pricing demand is real, but it is not an information security requirement.

### How to build the list for any organisation

1. List everyone who relies on, regulates, supplies, owns or works for the organisation.
2. Find their requirements in real sources: Contracts and SLAs, data processing agreements, laws and regulator guidance, tender questionnaires, insurance policies, staff handbook.
3. For each requirement, decide: Is it about information security? If yes, mark it "Yes" and name the policy, process or control that meets it. If no, mark it "No" and say where else it is handled.
4. Feed the "Yes" requirements into the legal and contractual register (control 5.31) and the risk assessment.

Template with typical parties found in most organisations:

| Interested party | Typical requirement | Via ISMS? | Typical way it is addressed |
| --- | --- | --- | --- |
| Clients / customers | Confidentiality of their data, agreed availability, proof of security (certificate, questionnaires), breach notification | Yes | Contracts, SLA monitoring, certification, incident management |
| Employees and contractors | Clear rules, protection of their personal data, secure working tools | Yes | Acceptable use policy, awareness training, HR privacy notice |
| Owners / top management / board | Protect reputation and revenue, meet legal duties, support business growth | Yes | ISMS objectives, management review, risk reporting |
| Regulators and authorities | Compliance with data protection and sector laws, incident reporting within legal deadlines | Yes | Legal register, privacy programme, incident procedure |
| Suppliers and service providers | Customer meets its side of shared responsibilities; payment and commercial terms | Partly | Supplier security policy and reviews; commercial terms handled by Finance/Procurement |
| Auditors (internal, external, certification body) | Access to evidence, conformity with the standard | Yes | Internal audit programme, document control |
| Insurers | Minimum controls such as MFA, backups, EDR | Yes | Access control, backup and endpoint standards |
| Partners, public, media | Trust, honest communication after an incident | Partly | Incident communication plan; general PR handled by Marketing |

Worked example

- **Clients:** Confidentiality of their data, availability per SLA, ISO 27001 certificate; financial-sector clients pass down DORA obligations.
- **Employees:** Secure tools for remote work, protection of HR data.
- **Shareholders / management:** Win certified-supplier tenders.
- **Regulators:** IDPC for GDPR and Cap. 586 (Malta's Data Protection Act), 72-hour breach notification; MFSA where relevant.
- **Suppliers:** Microsoft (Azure, M365) expects the company to secure its side of the shared responsibility model.
- **Auditors:** Certification body and internal auditor.

Auditor tip

If you mark a requirement "No / not via ISMS", say where it *is* handled. An empty answer looks like an oversight.

04

## ISMS scope

4.3

Standard requires

Determine the boundaries and applicability of the ISMS, considering the issues in 4.1, the requirements in 4.2, and the **interfaces and dependencies** between your activities and those performed by other organisations. The scope must be available as documented information.

Concept

Scope answers one question: **What exactly does the ISMS protect?** You draw a line around the organisation. Everything inside must follow the ISMS; everything outside must be named, with a reason, and any connection across the line must be managed. A scope has five parts, covered below.

### a) Scope statement

One or two sentences, the same wording that will appear on the certificate. Fill in this template:

The information security management system of *\[organisation name\]* covering *\[activities, products or services\]*, provided from *\[locations / remote work\]*, *\[optional: supported by named departments\]*.

Concept

Write it so a client reading the certificate understands what is covered: **What** (services/products), **Where** (locations), **Who** (teams). Avoid vague wording like "all IT systems"; name the business activity.

Worked example

The information security management system covering the development, hosting, operation and support of the Company's SaaS platform, delivered from the Malta office and by remote staff.

Auditor tip: Do we need the SoA version in the scope?

No. ISO 27001 clause 4.3 does not ask for it, so your own scope statement can leave it out (as above). You will still often see it on the **certificate**, because ISO/IEC 27006 (the rules for certification bodies) requires the certificate to reference the SoA version. The certification body adds that, not you. Keeping it out of your scope statement also means you don't have to update the scope every time the SoA changes.

### b) Organisational boundaries

Which parts of the organisation are inside the line. List:

- **Legal entities:** Which company or companies (important in groups with subsidiaries).
- **Departments and teams:** Usually every team that touches in-scope information, including support functions like HR, Finance and Facilities.
- **Locations:** Offices, data centres, warehouses, and remote or home working.
- **People:** Employees, contractors, interns, and third-party staff with access.

Worked example

- Departments: Engineering, Operations, Support, HR, Management.
- Locations: Malta office, remote workers.

### c) Technical boundaries

Which systems and technology are inside the line. Go through each category below and name what the organisation actually uses. The two example columns show how different setups fill the same category.

| Category | What to name | Example: Cloud company | Example: On-premises company |
| --- | --- | --- | --- |
| Products / applications | The systems that deliver the in-scope service, and all their environments | SaaS platform (production, staging) | ERP (Enterprise Resource Planning: One system that runs finance, HR, purchasing and stock, such as SAP or Microsoft Dynamics), internal business apps |
| Hosting | Where those systems run | Azure / AWS / Google Cloud accounts | Own server room, colocation data centre |
| Identity | Where users and logins are managed | Microsoft Entra ID, Okta | Active Directory |
| Email and collaboration | Where staff store and share information | Microsoft 365, Google Workspace | Exchange server, file shares |
| Endpoints | Devices people use | Laptops, mobile phones | Desktops, shop-floor or OT terminals |
| Networks | How systems connect | Cloud virtual networks, VPN | LAN, WAN, firewalls, Wi-Fi |
| Supporting tools | Tools that run or protect the above | CI/CD pipeline, backups, SIEM, ticketing | Backup servers, monitoring, ticketing |

Auditor tip

Decide explicitly whether **test and development environments** are in scope. They often hold copies of real client data, and auditors ask about them. Name the cloud accounts or subscriptions precisely, so anyone can tell which resources the controls cover.

Worked example

- **The platform and its environments (production, staging):** The product the company sells, plus its pre-release copy.
- **Azure subscriptions and tenants:** The cloud accounts where the platform runs; naming them shows exactly which cloud resources are covered.
- **Microsoft 365 and endpoint estate:** Email, Teams, SharePoint, OneDrive, and the staff laptops and phones that access them.

### d) Interfaces and dependencies

Activities performed by other organisations that the in-scope service depends on (clause 4.3 c). For each one, say who controls it and how you manage the connection.

| Typical dependency | Who controls it | How the interface is managed |
| --- | --- | --- |
| Cloud or hosting provider (data centres, hardware) | Provider | Shared responsibility model, review of the provider's ISO 27001 / SOC 2 reports, supplier assessment |
| Outsourced services (managed IT, SOC, payroll, development) | Supplier | Contract security clauses, NDAs, periodic supplier review |
| Parent company or shared group services | Group | Intra-group agreement, defined responsibilities |
| Office building access and utilities | Landlord | Lease terms, own access control inside the premises |
| Internet and telecom | Telecom provider | SLA, redundant connection where needed |

Worked example

- **Azure data centres:** Controlled by Microsoft; managed through the shared responsibility model and Microsoft's ISO 27001 / SOC 2 reports.
- **Outsourced suppliers:** For example managed SOC and payroll; managed through contract clauses and supplier reviews.
- **Malta office building:** Controlled by the landlord; the company runs its own access control inside the office.

### e) Exclusions, with justification

Anything left outside the line (a subsidiary, a site, a product line) must be named with a reason. A good justification shows the excluded part does not share systems, data or people with the in-scope part.

Common mistake

Two different kinds of "exclusion" get mixed up:

- **Scope exclusions** (a business unit, a site, a product) go here, with justification.
- **Annex A control exclusions** go in the Statement of Applicability (6.1.3 d), not in the scope.
- Clauses 4 to 10 can **never** be excluded.

An auditor will also check that an excluded part doesn't share systems or people with the in-scope part. If it does, the boundary isn't real.

05

## Review

9.3.2

State when the document is reviewed: at minimum **annually** and as an **input to each management review**.

Standard requires

Management review inputs include **9.3.2 b** changes in external and internal issues relevant to the ISMS, and **9.3.2 c** changes in needs and expectations of interested parties (added in 2022).

Concept

Context is not a one-time exercise. If something changes (a new regulation, a new cloud provider, a merger), update this document. That update can then ripple into the **scope**, the **risks** and the **objectives**. This is the loop shown in the big picture above.

Auditor tip

Keep a revision history table (version, date, author, change summary, approver). In the surveillance audit, the first thing they check is whether the "annual" review actually happened.

## Check yourself

Which parts of clause 4 should be documented, and where is that written?

All three: Issues (4.1), interested parties (4.2) and scope (4.3). For the scope it is written directly in clause 4.3: "The scope shall be available as documented information." For 4.1 and 4.2, it comes from three other places in the standard:

**7.5.1 b:** The ISMS must include the documented information the organisation decides is necessary for its effectiveness. Context and interested parties are needed for the risk assessment and objectives, so they belong there.

**Annex A 5.31:** Legal, statutory, regulatory and contractual requirements must be identified, **documented** and kept up to date. This covers a large part of the 4.2 requirements.

**9.3.2 b and c:** Management review must look at **changes** in issues and interested parties. You can only show a change if the previous version was recorded.

What did ISO 27001:2022 add to 4.2?

Point (c): Determine which interested-party requirements will be addressed through the ISMS.

What does Amendment 1 (2024) require about climate change?

Determine whether climate change is a relevant issue (4.1), and a note that interested parties can have climate-related requirements (4.2).

Where do you justify excluding an Annex A control?

In the Statement of Applicability (6.1.3 d), not in the scope document.

Which management review inputs link back to this document?

9.3.2 b (changes in internal/external issues) and 9.3.2 c (changes in interested parties' needs and expectations).

## Reference: What ISO 27001 says

Clause 4

The original requirement text, kept here so you can compare the notes above with the standard itself.

ISO/IEC 27001:2022 · 4 Context of the organization

### 4.1 Understanding the organization and its context

The organization shall determine external and internal issues that are relevant to its purpose and that affect its ability to achieve the intended outcome(s) of its information security management system.

NOTE Determining these issues refers to establishing the external and internal context of the organization considered in Clause 5.4.1 of ISO 31000:2018.

**Added by Amd 1:2024:** The organization shall determine whether climate change is a relevant issue.

### 4.2 Understanding the needs and expectations of interested parties

The organization shall determine:

1. a) interested parties that are relevant to the information security management system;
2. b) the relevant requirements of these interested parties;
3. c) which of these requirements will be addressed through the information security management system.

NOTE The requirements of interested parties can include legal and regulatory requirements and contractual obligations.

**Added by Amd 1:2024 (NOTE 2):** Relevant interested parties can have requirements related to climate change.

### 4.3 Determining the scope of the information security management system

The organization shall determine the boundaries and applicability of the information security management system to establish its scope.

When determining this scope, the organization shall consider:

1. a) the external and internal issues referred to in 4.1;
2. b) the requirements referred to in 4.2;
3. c) interfaces and dependencies between activities performed by the organization, and those that are performed by other organizations.

The scope shall be available as documented information.

### 4.4 Information security management system

The organization shall establish, implement, maintain and continually improve an information security management system, including the processes needed and their interactions, in accordance with the requirements of this document.

Study notes for ISO/IEC 27001:2022 incl. Amd 1:2024. Example content is illustrative; adapt it to the real organisation before use.