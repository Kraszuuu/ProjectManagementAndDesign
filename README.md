# Group 5 EMR Presentation — Review Notes

## Purpose

This document records the review feedback on the Group 5 presentation and the
follow-up actions agreed by the team.

Reviewed artefact:

- `ICT_Project/presentation/Group 5 Presentation.pdf` (25 slides)

Feedback received:

> Please be careful our key activities and WBS have to match because key
> activities should reflect our scope as well as WBS. Also she will analyze cost
> estimation because she couldn't understand. It seems good guys.

Overall assessment: the deck is well structured and communicates the project
clearly (Business Model Canvas, RACI, WBS, phased plan, PERT, TCO, ROI and NPV).
The two comments are nevertheless valid: the traceability between scope, key
activities, WBS and cost is incomplete, and the cost section mixes several
perspectives and does not cover the full WBS. Both points should be addressed
before the next review.

---

## 1. Alignment: Key Activities, Scope and WBS

### Current mapping

| Key Activity (slide 5) | WBS (slide 12) | Observation |
|---|---|---|
| EMR Software Development | 1.3.1–1.3.4 | Too broad; covers four separate work packages |
| Integration (e-Nabız, PACS) | 1.4.1–1.4.2 | Consistent |
| National-system integration | 1.4.1 | Duplicate of the previous activity |
| Cybersecurity testing | 1.5.2 | Consistent, but naming differs from the WBS ("Security & Penetration Testing / KVKK audit") |

### Gaps

- At least 6 of the 13 WBS tasks have no corresponding Key Activity:
  - 1.1 Project Initiation
  - 1.2.1 Cloud Datacenter Setup
  - 1.2.2 Endpoint Fleet Procurement
  - 1.5.1 Paper & Legacy Data Migration
  - 1.6.1 On-Site Clinical Training
  - 1.6.2 Go-Live & Hypercare
- Network infrastructure (LAN cabling, firewall) appears in Phase 1 of the
  implementation strategy but is absent from both the WBS and the Key Activities.
- Key Activities are therefore not a faithful summary of the project scope, and
  the WBS cannot be traced back to them.

### Additional consistency findings

- **WBS hierarchy:** the deck lists leaves such as 1.2.1, 1.3.1 and 1.4.1 but no
  parent nodes 1.2, 1.3, 1.4, 1.5 or 1.6. A WBS should show the full hierarchy.
- **Implementation plan vs WBS:** Phase 1 includes LAN cabling and firewall,
  Phase 3 includes a pilot in three departments, and Phase 4 includes expansion
  to ER/ICU and paper phase-out. None of these has a WBS task or a cost line.
- **Sequencing:** Phase 1 places system integration in months 1–6, while WBS task
  1.4.1 depends on 1.3.4 (Patient Portal), so integration cannot start that early.
- **RACI vs WBS:** the RACI covers 15 deliverables, the WBS has 13 tasks. RACI
  adds "Stakeholder Requirements" and "Security Framework", while the WBS
  includes network infrastructure that is missing from the RACI.
- **Scope promises:** offline mode, patient portal and the "≤ 3 clicks" design
  target are central to the value proposition, but there is no usability,
  availability or acceptance-testing task in the WBS.

### Proposed Key Activities

The Key Activities should be the level-2 branches of the WBS:

1. Infrastructure and cloud deployment (datacenter, LAN, firewall)
2. Endpoint hardware procurement and rollout (4,000 medical tablets)
3. EMR software development (database/API, web and mobile apps, offline sync,
   patient portal)
4. Systems integration (e-Nabız, PACS, LIS)
5. Data migration and digitization
6. Security testing and KVKK compliance
7. Training and change management
8. Go-live, hypercare and support

### Proposed WBS structure

```
1.0  EMR Implementation
1.1  Project Initiation and Architecture
1.2  Infrastructure and Hardware
     1.2.1 Cloud Datacenter Setup
     1.2.2 Network Infrastructure (LAN, firewall)      <- add, restores M2
     1.2.3 Endpoint Fleet Procurement
1.3  Software Development
     1.3.1 Central Database and Backend APIs
     1.3.2 Web and Mobile Applications
     1.3.3 Offline Sync Engine
     1.3.4 Patient Portal
1.4  System Integration
     1.4.1 National Health Integration (e-Nabız)
     1.4.2 PACS and LIS Integration
1.5  Data and Security
     1.5.1 Paper and Legacy Data Migration
     1.5.2 Security Testing and KVKK Audit
1.6  Rollout and Support
     1.6.1 Pilot Deployment
     1.6.2 On-Site Clinical Training
     1.6.3 Go-Live and Hypercare
```

Every leaf should then appear in the cost model and in the milestone plan.

---

## 2. Cost Estimation

### Main findings

1. **Only 6 of 13 WBS tasks are costed.**
   The PERT table covers 1.2.1, 1.2.2, 1.3.1, 1.3.2, 1.4.1 and 1.6.1.
   The following are outside the budget: 1.1, 1.3.3 (offline sync), 1.3.4
   (patient portal), 1.4.2 (PACS/LIS), 1.5.1 (migration), 1.5.2 (security
   testing) and 1.6.2 (go-live). The deck itself states that the estimate
   covers "6 critical budget work packages". The TRY 179.2M CAPEX is therefore
   not a cost baseline for the full scope.

2. **Payment gates total 85%, not 100%.**
   M0 10% + M1 15% + M3 25% + M4 20% + M5 10% + M6 5% = 85%.
   M2 (15%, network infrastructure) is missing. This is a direct consequence of
   the network work package being absent from the WBS.

3. **Contract value and TCO are inconsistent.**
   CAPEX TRY 179.2M + 5 × TRY 65M = TRY 504.2M TCO, while the proposed contract
   is TRY 350M net. On those figures the project would be TRY 154.2M below cost,
   which contradicts the reported ROI of 195% and NPV of TRY 222M.

4. **Revenue definition is unclear.**
   TRY 854.2M equals TRY 504.2M of cost plus TRY 350M of "target". This is a
   cost-plus calculation, not gross revenue. The deck mixes the vendor
   perspective (revenue, margin) with the hospital perspective (investment
   appraisal). The two should be separated and labelled explicitly.

5. **ROI denominator is inconsistent.**
   ROI 195% = TRY 350M / TRY 179.2M, i.e. net benefit divided by CAPEX only.
   If total investment (CAPEX + 5-year OPEX = TRY 504.2M) is used, ROI is about
   69%. The formula and the perspective must be stated.

6. **NPV timing is optimistic.**
   NPV TRY 222M at a 10% discount rate assumes revenue from year 1, while the
   implementation lasts 16 months. Cash flows should start after go-live. A 10%
   discount rate also needs justification in the TRY environment, given
   inflation and local interest rates.

7. **No contingency and no OPEX breakdown.**
   PERT produces an expected value, not a P80 budget. There is no contingency or
   management reserve, no VAT/KDV treatment and no inflation escalation. The
   TRY 65M annual OPEX (about 36% of CAPEX) is not itemized.

8. **Stale and duplicated slides.**
   Slide 5 says "Full CAPEX/TCO: pending validation", while slide 22 already
   reports CAPEX TRY 179.2M. Slides 16 and 19 duplicate the same PERT table, and
   slide 16 carries the wrong subtitle ("4-Phase Deployment Concept").

### Arithmetic reference

| Item | Value |
|---|---|
| PERT expected CAPEX | TRY 179,166,667 |
| Annual OPEX | TRY 65,000,000 |
| 5-year TCO (179.2 + 5 × 65) | TRY 504,200,000 |
| Proposed contract | TRY 350,000,000 |
| Contract vs TCO | TRY -154,200,000 |
| Revenue stated in deck | TRY 854,200,000 (504.2 + 350) |
| ROI as stated (350 / 179.2) | 195% |
| ROI on total investment (350 / 504.2) | about 69% |

---

## 3. Recommended Actions

Priority order:

1. Rebuild Key Activities as the six to eight level-2 WBS branches.
2. Complete the WBS: add parent nodes, network infrastructure (which restores
   M2), pilot, expansion to ER/ICU and paper phase-out; remove the duplicated
   "National-system integration" activity.
3. Cost every WBS leaf; add contingency to reach a P80 budget; itemize OPEX.
4. Add a single traceability table: Scope item → Key Activity → WBS ID → Cost →
   Milestone.
5. Bring payment gates to 100%, reconcile the TRY 350M contract with the
   TRY 504.2M TCO, and restate ROI and NPV with explicit formulas and timing.
6. Add a five-year cash-flow table, IRR, payback period and sensitivity analysis
   (tablet price ±20%, three-month delay, TRY inflation/FX, cloud consumption).
7. Remove the duplicate PERT slides and update slide 5 so that it no longer says
   "pending validation".

---

## 4. Reference: Where the CAPEX and OPEX Figures Are Documented

For readers who want the detailed cost breakdown, the CAPEX and OPEX figures are
also documented in `ICT_Project/presentation/ict_presentation.pdf` on slides 17
and 18 (slide 17 = CAPEX, slide 18 = OPEX; pages 18 and 19 in a 1-based PDF
viewer). That presentation is one of the project's knowledge sources and is a
useful reference for the cost methodology.

Two points should be kept in mind when reusing those figures:

- `ict_presentation.pdf` is expressed in PLN and refers to the Wrocław scope,
  whereas the Group 5 deck is expressed in TRY and refers to the Istanbul scope.
  Currency and scope should be aligned before any figure is carried over.
- The full calculation methodology and assumptions are in
  `ICT_Project/LaTeX/ENG/Chapters/cost-estimate.tex`, which can be used as the
  reference for rebuilding the cost baseline.

The presentation is one of several project sources; it is intended to support the
analysis, not to replace the underlying report and calculations.
