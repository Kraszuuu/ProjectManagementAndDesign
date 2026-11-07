# Project Proposal — PWr ICT Project (filled onto `Project Proposal Sample.pptx`)

Mapping of the **PWr "ICT_Project"** contents (*"Projektowanie bezpiecznej architektury ICT –
system EMR for Szpital im. Bajgla we Wrocławiu"*) onto the slides of
`TR_artifacts/Project Proposal Sample/Project Proposal Sample.pptx`.

Each section below corresponds to one slide of the sample deck. Content is taken from the
PWr LaTeX chapters (`introduction`, `empatyzacja`, `project-idea`, `implementation`,
`kosztorys`, `functionalities`) and reorganised to fit the proposal slides. Anything not
present in the source is marked **`[to complete]`**.

---

## Slide 1 — Title slide

**GROUP / COMPANY NAME:** `PWr ICT Project Group` *(no commercial brand in the source — use the group/university name)*

**Project name:** Integrated medical information system (EMR) for **Szpital im. Bajgla we Wrocławiu**

**Student names and numbers:**
| Name | Student no. |
|------|-------------|

**Institution:** Wrocław University of Science and Technology (PWr)
**Framing for ITU:** social/entrepreneurial e-health project → **SDG 3 (Good Health and Well-being)**, with links to SDG 9 (industry/innovation) and SDG 10 (reduced inequalities).
**Elevator pitch (1–2 sentences):** *One secure digital environment that puts a patient's full medical record — history, test results, imaging, orders — into the hands of authorised hospital staff in at most three clicks, 24/7, while giving patients online access to their own results.*

---

## Slide 2 — The need and the problem you need to solve

**Context.** The EU "Digital Decade 2030" programme requires all citizens to have access to electronic health records by 2030; Poland already scores 90% in eHealth maturity, yet many hospitals still run on paper.

**The need.** Szpital im. Bajgla is a large multi-department hospital (surgical, internal medicine, neurology, orthopaedics, oncology, paediatrics, ICU, ER, laboratory, diagnostic imaging, mortuary) that still manages medical records **on paper**. There is no single, central environment for managing documentation and information flow.

**Problems to solve:**
- **Slow, fragmented information flow** — records, results, orders and nursing reports are physically carried between departments; access depends on where the paper file currently is.
- **Critical delays** between departments, the laboratory and diagnostic imaging — problematic exactly when speed matters (ER, ICU).
- **No quick access to full patient history** — repeated hospitalisations require manually searching archives; the same data is re-typed into multiple documents (error risk).
- **Unsafe data handling** — paper can be lost, mis-filed, handed to the wrong person or damaged; no real control over who accessed what; sensitive data (GDPR) needs role-based access, authentication and audit.
- **No patient access** — patients cannot see their results or treatment history; obtaining documents requires a physical visit.
- **Growing data volume / organisational strain** — the paper model does not scale and does not match EU eHealth direction.

**Stakeholders affected:** hospital director, board, IT staff, physicians, nurses, lab/diagnostics staff, administrators, patients (incl. elderly and digitally low-skilled users), and a malicious actor (system must resist unauthorised access).

**Success criteria (target functionality).**
- Digital handling of patient records without paper flow in daily work.
- Real-time add/view/update of medical records by authorised users across departments.
- Central access from one environment: history, lab results, diagnostic documentation, current orders.
- Role-based access levels (lab adds results; physician sees full record; administration sees only what it needs).
- Online patient access to selected results, visit history and basic treatment information.
- Concurrent multi-user operation with no data loss and 24/7 continuity.

---

## Slide 3 — Value Proposition Canvas

**Customer Segment(s):** hospital medical staff (physicians, nurses, lab/diagnostics) · hospital administration · patients.

### Customer profile
**Jobs to be done**
- Get a patient's full history, latest results and current orders in seconds.
- Coordinate care across departments, laboratory and imaging.
- Update documentation once, without re-typing.
- Check test status / receive results quickly.
- (Patients) view results and treatment history without visiting the hospital.

**Pains**
- Paper chaos: records lost, mis-filed or delayed between departments.
- No real-time access to current data → delays in ER/ICU.
- Repeated manual data entry, illegible notes, outdated data.
- No mobile access on the ward; no remote/offline availability.
- Weak access control and audit on paper; GDPR exposure.
- Patients wait / must collect documents in person.

**Gains**
- Any patient information in **≤ 3 clicks**.
- Mobile (tablet) access at the bedside and **offline mode** with sync.
- Automatic result delivery and notifications.
- Legible, single source of truth; less admin time → more time with the patient.
- Secure, auditable, role-based access; passenger/patient self-service online.

### Value map
**Products & services**
- Integrated **EMR platform** (web app + mobile app + patient portal).
- Central patient database; electronic orders; integrations with P1/e-Health, LIS (HL7/FHIR) and PACS (DICOM).

**Pain relievers**
- Role-based access, individual accounts, 2FA, full audit log, auto-logout.
- Powerful search by PESEL; structured documentation to eliminate re-typing.
- Offline mode with conflict-aware sync for weak ward Wi-Fi.

**Gain creators**
- Real-time data synchronisation across departments.
- Automatic routing of lab/imaging results into the record; push/SMS notifications.
- Patient portal (responsive, WCAG 2.1 AA, mObywatel / Profil Zaufany login, PDF downloads).

---

## Slide 4 — Business Canvas (Business Model Canvas)

| Block | Content (from the PWr project) |
|---|---|
| **Customer segments** | Szpital im. Bajgla (large multi-department public hospital) — medical staff, administrative staff, patients; secondary: other Polish public hospitals. |
| **Value propositions** | Central, secure EMR replacing paper: full record in ≤3 clicks, 24/7; real-time cross-department data; reduced admin burden; improved patient safety; GDPR/eHealth compliance; patient portal; offline + mobile. |
| **Channels** | Web application · mobile app (tablets) · patient portal · SMS gateway · on-site training, hypercare and helpdesk. |
| **Customer relationships** | Long-term "turnkey" delivery contract; SLA-backed support; 6-FTE maintenance & development team; helpdesk L1/L2; 3-month hypercare; "super-user" programme; account/PM contact. |
| **Revenue streams** | **Contract price 34.75 m PLN net** (milestone-based) · **OPEX 6.54 m PLN/year** (cloud, licenses, support, spare fleet) · optional modules (analytics/AI = Variant III). *Hospital-side financing:* own funds + KPO (health digitalisation), EU FENG / regional funds, Ministry of Health and Centrum e-Zdrowia grants. |
| **Key resources** | Development & maintenance team · Microsoft Azure cloud (Poland Central + West Europe DR) · end-point fleet (810 tablets, 680 AiO workstations, 2 000 2FA readers, …) · software licenses · digitisation scanners · certified security stack. |
| **Key activities** | Software development (microservices, RxH) · integrations (P1, HL7/FHIR, DICOM/PACS) · documentation digitisation & ETL migration · deployment & training (2 600 users) · security (DPIA, pentests, ISO 27001, SIEM/SOC) · support. |
| **Key partners** | Microsoft Azure · Centrum e-Zdrowia (P1) · hardware vendors (tablets, switches, APs, firewalls) · SMS gateway / Profil Zaufany · certification & audit bodies. |
| **Cost structure** | **CAPEX 27.27 m PLN net** (A team 5.30 · B cloud setup 0.96 · C equipment 10.51 · D licenses 0.49 · E migration 1.73 · F integrations 1.08 · G security 0.73 · H deployment/training 1.55 · + reserves) · **OPEX 6.54 m PLN/yr** · **TCO 5 yr ≈ 67.5 m PLN net**; organizational adoption ≈ 5.5 m PLN (opportunity cost). |

---

## Slide 5 — Lean Canvas

| Block | Content |
|---|---|
| **Problem** | Top 3: (1) paper documentation, no central system; (2) slow, fragmented flow between departments / lab / imaging, critical in ER & ICU; (3) no patient access + weak access control & audit. |
| **Customer segments** | Hospital staff (physicians, nurses, lab/diagnostics, administration) · patients. |
| **Unique value proposition** | *The single secure digital environment for the entire hospital — the full patient record at hand in ≤3 clicks, 24/7, on any device.* |
| **Solution** | EMR platform (web + mobile + offline sync), central DB, electronic orders, P1/LIS/PACS integrations, role-based access, patient portal. |
| **Channels** | Web app, mobile app, patient portal, SMS notifications, direct sales to hospital + on-site training/helpdesk. |
| **Revenue streams** | Contract 34.75 m PLN net (milestone payments) + OPEX 6.54 m PLN/yr; public-sector funding (KPO, FENG, MoH, CeZ). |
| **Cost structure** | Team/dev 5.30 m · equipment 10.51 m · migration 1.73 m · integrations 1.08 m · security 0.73 m · deployment/training 1.55 m · cloud licenses; TCO 5 yr ≈ 67.5 m PLN. |
| **Key metrics** | % of records handled electronically · time to access a record · uptime (SLA 99.9%) · active users (2 600 staff / up to 400 k patients) · admin time saved · 2FA/audit coverage. |
| **Unfair advantage** | Deep fit to Polish hospital processes + native integration with the national P1 platform, GDPR/e-Zdrowia compliance and offline ward workflow — hard to copy quickly. |

---

## Slide 6 — Social Business Model Canvas

*(Recommended variant for this public-health/social project.)*

| Block | Content |
|---|---|
| **Segments — Beneficiary** | Patients of Szpital im. Bajgla (incl. elderly, low digital skills) who gain access to their own medical data. |
| **Segments — Customer** | Szpital im. Bajgla (the paying organisation) and external stakeholders (public payers: MoH, CeZ, EU funds). |
| **Value proposition — User (beneficiary)** | Easier, faster, safer care; online access to results/history; no need to collect paper documents; simple, accessible interface. |
| **Value proposition — Customer (payer)** | Efficient, compliant, paperless hospital; reduced admin cost; higher patient safety; EU Digital Decade alignment. |
| **Type of intervention** | Product/service delivery — deployment of a secure digital EMR system (not advocacy/research). |
| **Channels** | Web + mobile apps, patient portal, SMS, on-site training and support. |
| **Key activities** | Development, integration (P1/LIS/PACS), migration/digitisation, training, security & auditing, support. |
| **Key resources** | Dev/maintenance team, Azure cloud, device fleet, licenses, certified security capabilities. |
| **Partners + key stakeholders** | Microsoft Azure, Centrum e-Zdrowia, hardware vendors, certification/audit bodies; stakeholders: hospital board, staff, patients, MoH, media. |
| **Impact measures** | % digitised documentation · time to access a record · reduction in administrative workload · patient portal adoption · digital-accessibility compliance (WCAG 2.1 AA) · contribution to **SDG 3**. |
| **Surplus** | Where does surplus go? — reinvested into system development, accessibility features and reduction of the hospital's long-term operating cost. |
| **Revenue** | Contract price (34.75 m PLN net) + OPEX (6.54 m PLN/yr); public financing: KPO, FENG / regional funds, MoH and CeZ grants. |
| **Cost structure** | CAPEX 27.27 m PLN net (with reserves) · OPEX 6.54 m PLN/yr · adoption cost ≈ 5.5 m PLN (opportunity cost, excluded from the contract). |

---

## Slide 7 — Benchmark (Your company vs competitors)

The sample slide is a **feature comparison matrix** (Your company vs 3 competitors). The PWr
source only contains a **cost benchmark** (Oracle Cerner, Epic EMR — with PPP correction);
a feature benchmark must be built. Polish EMR/HIS vendors (e.g. **Comarch**, **Asseco**) and
international systems (**Epic**, **Oracle Cerner**, **Dedalus**) are the natural comparison set.

| Feature | **Our solution (PWr EMR, Variant II)** | Competitor 1 *(international, e.g. Epic / Oracle Cerner)* | Competitor 2 *(PL vendor, e.g. Comarch)* | Competitor 3 *(PL vendor, e.g. Asseco)* |
|---|---|---|---|---|
| Central patient database | Yes | Yes | Yes | Yes |
| Electronic medical record (EMR) | Full | Full | Full | Full |
| Mobile access for staff | Yes (tablets) | Partial | Partial | Partial |
| Offline mode + sync | **Yes (full)** | Varies | Limited | Limited |
| Patient portal | Yes | Yes | Yes | Yes |
| Integration P1 / LIS (HL7/FHIR) / PACS | Yes | Yes | Yes | Yes |
| Role-based access | Yes | Yes | Yes | Yes |
| 2FA + full audit log | Yes | Yes | Varies | Varies |
| Availability SLA | **99.9%** | 99.9%+ | Varies | Varies |
| Analytics / AI module | Optional (Variant III) | Yes | Limited | Limited |
| Deployment model | Cloud (Azure, EEA) | Cloud / on-prem | On-prem / cloud | On-prem / cloud |
| Indicative cost / bed | **~24 k PLN CAPEX (≈ 59 k PLN TCO 5 yr)** | ~120–272 k PLN (PPP-adjusted) | `[to complete]` | `[to complete]` |

**Price benchmark (from `kosztorys.tex`, PPP-adjusted to PLN):**
- Oracle Cerner, ~500 beds: 48–120 m PLN → **57.6–163.2 k PLN/bed**.
- Epic EMR, ~1000 beds: 200–400 m PLN → **120–272 k PLN/bed**.
- Our Variant II: CAPEX/bed ≈ **23.7 k PLN**, TCO 5 yr/bed ≈ **58.7 k PLN** → in the lower part of the benchmark range.

> ⚠️ Competitor feature values are indicative and marked `[to complete]` where the source has no data — confirm against current vendor documentation before presenting.

---

## Notes / gaps to close before submitting as an ITU proposal

From `new_artifacts/checklist_ITU_requirements_vs_PWr_project_EN.md`:

- **SDG link** — only implied; must be stated and measured explicitly (SDG 3).
- **Team size** — 6 members; ITU requires 7–8 → add 1–2 people.
- **Weighted scoring model** for variant selection — currently qualitative only.
- **Draft WBS, RACI matrix, team qualifications** — not yet created.
- **Feature-based competitor benchmark** — build from the table above (real vendor data).
- **Elevator pitch** — drafted on Slide 1; expand to a 60–90 s script.

---

*Source of truth: `ICT_Project/` (LaTeX, 6 members, June 2026). This file is a non-graphical
content mapping only — it does not reproduce slide formatting.*
