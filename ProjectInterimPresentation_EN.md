# Project Interim Presentation — Notes on Incomplete Items

This document collects notes on the 7 items that need to be completed before the interim presentation.

**Initial status (9 requirement items):**

| # | Item                                                             | Status                              |
| - | ---------------------------------------------------------------- | ----------------------------------- |
| 1 | Project Proposal (problem, variants, background, benchmark, BMC) | PARTIAL                             |
| 2 | Stakeholder Analysis                                             | CLOSED                              |
| 3 | Project Organizational Structure                                 | CLOSED (new names are correct)      |
| 4 | Project Team                                                     | PARTIAL                             |
| 5 | Draft WBS                                                        | MISSING                             |
| 6 | Action Plan                                                      | PARTIAL                             |
| 7 | Responsibility Chart (RACI)                                      | MISSING                             |
| 8 | Cost Baseline and Project Budget                                 | BUDGET READY, COST BASELINE MISSING |
| 9 | Financial Feasibility (ROI, NPV)                                 | PARTIAL                             |

The notes below cover items **1, 4, 5, 6, 7, 8, 9** (7 items). Item 8 is included because the budget itself exists, but a formal, approved, time-phased cost baseline is missing.

---

## 1. Project Proposal

**Status:** partial.

**What already exists:**

- Problem definition, background and context: `ICT_Project/Rozdziały/introduction.tex`.
- Possible solutions: three EMR variants with a comparison table and a selection: `ICT_Project/Rozdziały/project-idea.tex:22-269`.
- Industry and EU regulatory context (Digital Decade 2030, eHealth, GDPR).

**Gaps:**

1. **Benchmarking of existing solutions is cost-only.** `ICT_Project/Rozdziały/kosztorys.tex:109-153` compares Oracle Cerner and Epic solely by cost per bed. There is no feature comparison with real systems (e.g., Comarch, Asseco, Dedalus, Epic, Oracle Cerner).
2. **No Business Model Canvas (BMC).** The project contains no BMC in any form. The file `TR_artifacts/Project Proposal Sample/Project_Proposal_PWr_filled.md` is a working content mapping, not a delivered artifact.
3. **Context analysis is uneven.** The industry and hospital process are well described, but the market (size, trends, competition, public funding) and the organization itself (structure, IT budget, digital maturity) are weak.
4. **Variant selection lacks a weighted scoring matrix.** The assessment is qualitative (yes/partial/none), which weakens the "possible solution options" part.

**What to add:**

- **Feature benchmark table:** rows = features, columns = our solution + 3 competitors. Features: EMR completeness, mobile access, offline mode, patient portal, P1/LIS (HL7/FHIR)/PACS integrations, roles and permissions, 2FA and audit log, SLA, deployment model (cloud/on-prem), analytics/AI module, indicative cost. Mark unconfirmed values as assumptions and provide sources.
- **Business Model Canvas — 9 blocks:**
  - Customer segments: Szpital im. Bajgla (medical staff, administration, patients); secondarily other Polish public hospitals.
  - Value proposition: a central, secure EMR instead of paper; full documentation in at most 3 clicks, 24/7; GDPR and e-Health compliance; patient portal; offline and mobile mode.
  - Channels: web application, mobile app/tablets, patient portal, SMS gateway, on-site training and helpdesk.
  - Customer relationships: turnkey contract, SLA, 6-FTE maintenance team, L1/L2 helpdesk, hypercare, super-user programme.
  - Revenue streams: contract price PLN 34.75 million net (milestone payments), OPEX PLN 6.54 million/year, optional modules (Variant III); hospital financing: own funds, KPO, FENG, Ministry of Health, CeZ.
  - Key resources: development and maintenance team, Microsoft Azure (Poland Central + West Europe DR), fleet of 810 tablets and 680 workstations, licences, digitisation scanners.
  - Key activities: development, integrations, digitisation and migration, deployment and training of 2,600 people, security (DPIA, pentests, ISO 27001, SIEM/SOC), support.
  - Key partners: Microsoft Azure, Centrum e-Zdrowia, hardware vendors, SMS gateway/Profil Zaufany, certification bodies.
  - Cost structure: CAPEX PLN 27.27 million net, OPEX PLN 6.54 million/year, 5-year TCO approx. PLN 67.5 million, adoption costs approx. PLN 5.5 million.
- **Market and organizational analysis:** a short subsection on the HIS/EMR market in Poland, healthcare digitalisation funding and the hospital's digital maturity.
- **Optional:** a weighted scoring matrix for the three variants.

**Completion criterion:** a slide/section with a completed BMC (9 blocks), a feature benchmark table with at least 3 competitors and sources, and no "to be completed" markers.

---

## 4. Project Team

**Status:** partial.

**What already exists:**

- Team composition and student numbers: `ICT_Project/main.tex:11-13`.
- Division of work by report chapter: `ICT_Project/Rozdziały/work_table.tex:31-94`.

**Gaps:**

1. **No project positions.** There is no assignment such as: project manager, deputy, business analyst, architect, backend/frontend/mobile, QA, UX/UI, security and compliance, financial controller, communication/presentation.
2. **No qualifications.** Education, technical skills, experience, certifications, tool and language proficiency are not described.
3. **No justification for team selection.** It is not explained why this team can deliver the project and what competency gaps it has.
4. **Confusing roles from the cost estimate.** `ICT_Project/Rozdziały/kosztorys.tex:301-322` lists roles such as "Project Manager", "Architect", "DevOps", etc., but these are roles of a fictional vendor in the estimate, not roles of the student team members. Without separating these layers, the presentation is unclear.
5. **No availability information.** Neither the workload dimension (FTE) nor individual availability is given.

**What to add:**

- A table: **member | student number | project role | scope of responsibility | qualifications | availability (FTE)**.
- A short paragraph justifying the team composition and role assignment.
- A clear note: the roles in the cost estimate (CAPEX category A) are vendor-side assumptions, not the project team composition.
- Mapping of project roles to chapters/areas: PM, requirements analysis, architecture, development, UX, QA, security, finance, presentation.

**Completion criterion:** a "Project Team" slide with roles and qualifications for each member and a consistent report subsection.

---

## 5. Draft Work Breakdown Structure (WBS)

**Status:** missing.

**What already exists (but is not a WBS):**

- `work_table.tex` — division of work by report chapter.
- Milestones M0–M6 in `kosztorys.tex:641-668` — a list of payment milestones, not a work breakdown structure.

**Gaps:**

- No 2–3 level hierarchy with work package identifiers.
- No resource assignment to packages.
- No predecessors or dependencies.
- No package descriptions/justifications or WBS dictionary.
- No link between the WBS and the schedule, RACI and budget.

**Proposed structure (example):**

1. Initiation
   1.1 Contract signing and team mobilisation
   1.2 Project plan and organization
   1.3 Stakeholder analysis and communication
2. Analysis
   2.1 Functional and non-functional requirements
   2.2 Analysis of clinical and administrative processes
   2.3 Compliance analysis (GDPR, e-Health, AI Act)
3. Design
   3.1 System architecture
   3.2 UX/UI design and patient portal
   3.3 P1/LIS/PACS integration design
4. Software development
   4.1 Backend and database
   4.2 Web frontend
   4.3 Mobile application
   4.4 External integrations
5. Infrastructure and hardware
   5.1 Azure environment and DR
   5.2 LAN/Wi-Fi network and firewall
   5.3 Delivery and configuration of end-user devices
6. Migration and digitisation
   6.1 Digitisation of active documentation
   6.2 ETL migration and data validation
7. Security and compliance
   7.1 DPIA and GDPR audit
   7.2 Penetration tests
   7.3 ISO/IEC 27001 certification and SIEM/SOC
8. Deployment and training
   8.1 Pilot in 3 departments
   8.2 Staff training (2,600 people)
   8.3 Go-live
   8.4 Hypercare
9. Project closing
   9.1 Final acceptance
   9.2 Documentation and handover to maintenance
   9.3 Lessons learned

**What to add for each lowest-level package:**

- ID and name.
- Description/justification ("explanation").
- Package owner.
- Resources: people, hardware, cloud, licences.
- Predecessors.
- Duration and final deliverable.
- WBS dictionary as a table.

**Completion criterion:** a WBS chart + a package table with resources, predecessors and descriptions, plus a WBS dictionary.

---

## 6. Action Plan

**Status:** partial.

**What already exists:**

- Phased deployment concept: `ICT_Project/Rozdziały/implementation.tex:10-18`.
- Payment milestones M0–M6: `ICT_Project/Rozdziały/kosztorys.tex:641-668`.

**Gaps:**

1. **No task list with durations and dates.** A description of stages is not an action plan.
2. **No dependencies or predecessors.** It is unclear what conditions the start of subsequent tasks.
3. **No owner or resource assignments.**
4. **No schedule.** There is no Gantt chart, PERT/CPM network, critical path or buffers.
5. **No link to the WBS.** The action plan should derive from work packages.
6. **M0–M6 are payment gates, not tasks.** They do not replace a schedule.
7. **No calendar dates.** The 16 person-months of the project manager in the cost estimate do not translate into any deadline.

**What to add:**

- An activity table: **ID (from WBS) | task | start | finish | duration | predecessors | owner | resources | deliverable/milestone**.
- An assumed start date and a horizon consistent with the cost estimate (approx. 16 months).
- A Gantt chart with tasks and M0–M6 as control points.
- A PERT/CPM network, ES/EF/LS/LF calculations and the critical path.
- Consideration of parallel streams (e.g., network infrastructure M2 in parallel with M1–M3).
- Time buffers and linking payment milestones to the schedule.

**Completion criterion:** an activity table + Gantt + critical path + dates consistent with the budget and WBS.

---

## 7. Responsibility Chart (RACI)

**Status:** missing.

**What already exists:** nothing — `work_table.tex` indicates the chapter author (de facto Responsible), but it is not a RACI matrix.

**Gaps:**

- No R (Responsible), A (Accountable), C (Consulted), I (Informed) roles for project tasks.
- No link to the WBS and schedule.
- No indication of the ultimately accountable person for each package.

**What to add:**

- A matrix: **rows = WBS packages**, **columns = team members** (6 people) + optionally the hospital side (sponsor, IT, medical staff) as consulted/informed stakeholders.
- Rules: exactly one "A" per row, at least one "R", "C"/"I" only where justified.
- A legend and a short justification of assignments.
- Consistency with the action plan and organizational structure.

**Example rows:** requirements, architecture, UX/UI, backend, integrations, security/DPIA, migration, training, go-live, closing.

**Completion criterion:** a complete RACI table with a legend, no rows without "A" and "R", consistent with the WBS.

---

## 8. Cost Baseline and Project Budget

**Status:** budget ready, formal cost baseline missing.

**What already exists:**

- Detailed cost estimate: CAPEX, OPEX, 5-year TCO, reserves, scenarios, contract price, payment schedule, funding sources: `ICT_Project/Rozdziały/kosztorys.tex`.
- Unit metrics (cost per bed, cost per staff account).

**Gaps:**

1. **No cost baseline as an approved budget distributed over time.** The cost estimate is a static estimate, whereas a baseline requires assigning costs to periods (month/quarter).
2. **No separation of the cost baseline from the management reserve.** Reserves are calculated, but there is no clear policy for releasing them.
3. **No change control procedure.** Thresholds and the approval process for deviations are not defined.
4. **No link between costs and the WBS and schedule.** It is unknown how much a given work package costs.
5. **No basis for EVM.** There is no PV/EV/AC or CPI/SPI (this may come later, but a baseline is a prerequisite).
6. **The payment schedule is cash flow to the vendor, not the project cost.** These two things must be separated.

**What to add:**

- A **time-phased budget** table: CAPEX categories A–H and OPEX assigned to months/quarters in line with the action plan.
- A **cumulative S-curve** (planned expenditure over time).
- Baseline definition: approved value, approval date, approver.
- Reserve policy: technical vs management reserve, who can release it and when.
- Change control procedure: threshold (e.g., 5%), form, approval.
- Link to the WBS: cost assigned to work packages.

**Completion criterion:** a time-phased budget table + S-curve + description of the baseline and change control.

---

## 9. Financial Feasibility

**Status:** partial.

**What already exists:**

- Investment and operating costs: CAPEX PLN 27.27 million net, contract price PLN 34.75 million, OPEX PLN 6.54 million/year, 5-year TCO approx. PLN 67.5 million, adoption costs approx. PLN 5.5 million: `ICT_Project/Rozdziały/kosztorys.tex`.

**Gaps:**

1. **No estimate of expected benefits/revenues.** There is no monetisation of staff time savings, administrative work, paper and archiving, duplicate tests, etc.
2. **No ROI, NPV, IRR or payback period.** None of these indicators appears in the repository.
3. **No cash flows over time or discount rate.** NPV requires year-by-year cash flows.
4. **Inconsistent perspective.** The cost estimate mixes the vendor perspective (cost of delivery, margin) and the hospital perspective (contract price, TCO). The feasibility analysis must adopt the investor perspective, i.e., the hospital's.
5. **No sensitivity analysis.** It is unknown how NPV changes under worse assumptions.
6. **No break-even point.**

**What to add:**

1. **Clearly define the perspective:** the hospital as investor.
2. **Monetise benefits (conservatively, with sources):**
   - staff time savings: number of people × hours/year × hourly cost,
   - reduction in administrative and documentation work,
   - fewer duplicate tests and errors,
   - savings on paper, printing, archiving and rented space,
   - shorter hospital stay, if it can be justified,
   - describe qualitative benefits (patient safety, portal) separately.
3. **Build annual cash flows** over a 5–10 year horizon: year 0 — investment, years 1–5 — OPEX and benefits, possibly a residual value.
4. **Calculate indicators:**
   - NPV = sum of CF_t / (1+r)^t − initial investment,
   - ROI = (total benefits − total costs) / total costs × 100%,
   - IRR,
   - payback period (simple and discounted).
5. **Adopt a discount rate** (e.g., 5–8% for the public sector) and justify it.
6. **Sensitivity analysis:** benefits −20%/+20%, OPEX +30%, delay of 6/12 months; present the NPV range.
7. **Include adoption costs** on the hospital side and avoid double-counting the vendor margin.
8. **Conclusion:** whether the project is financially feasible, under what assumptions, and what the break-even point is.

**Completion criterion:** an assumptions table, a cash flow table, NPV/ROI/IRR/payback, a sensitivity analysis and an unambiguous conclusion.

---

## Suggested order of work

1. WBS (item 5) — the basis for the action plan, RACI and budget.
2. Action Plan (item 6) — a schedule with dependencies.
3. Responsibility Chart RACI (item 7) — based on the WBS.
4. Cost Baseline (item 8) — distributing the budget over time.
5. Financial Feasibility (item 9) — benefits and indicators.
6. Project Team (item 4) — roles and qualifications.
7. Project Proposal (item 1) — feature benchmark and BMC.
