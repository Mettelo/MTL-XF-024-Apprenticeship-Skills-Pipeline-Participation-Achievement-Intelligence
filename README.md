# MTL-XF-024 — Apprenticeship Skills Pipeline, Participation & Achievement Intelligence

**Mettelo Project Studio** · Cross-Functional · Master project specification  
**Client:** Confidential Regional Skills & Employer Engagement Authority  
**Accountable simulated executive:** Director of Skills & Employment  
**Sector:** Education / Skills / Economic Development  
**Team:** 6–8 people · **Window:** 8 weeks  
**Status:** documentation revised; file acquisition and cohort freeze pending  
**Review cadence:** quarterly skills participation and employer-engagement review

> This is a **simulated confidential-client engagement using official public/open data**. Client and stakeholder role labels describe a fictional engagement; do not claim a real external Mettelo customer, employment, endorsement or privileged data access. No raw data is uploaded by this specification update.

## Business problem

The skills authority needs to distinguish a reduction in starts from weaker participation or a shift in the age/level mix. These series count different activities and people, and the latest provisional period does not span the same months as completed academic years. A simple achievements-divided-by-starts chart can therefore imply a completion problem that the source cannot establish.

## Commissioned decision

> Which geographic, age and apprenticeship-level segments warrant employer-engagement or participation-support investigation based on starts, participation and achievement patterns?

## Practical use

The Director compares completed-year participation across compatible areas, then opens the latest provisional view as a separate panel. An age/level segment with weaker participation may warrant employer outreach, while an apparent achievements-to-starts imbalance prompts a request for linked learner progression evidence. The product does not claim that current starters have already completed or dropped out.

The full [business context](project/BUSINESS_CONTEXT.md) names operational stakeholders, decisions, risks and proposed benefit measures.

## What must be delivered

1. Produce a starts/participation/achievements trend for comparable windows, with age/level/geography views only where present.
2. Identify up to ten weakening skills segments and separate declining volume from population-adjusted participation.
3. Compare count-led and rate-led support scenarios and list linked learner/employer evidence required before making progression claims.

The complete D1–D12 pack includes discovery, source governance, ingestion/model, quality, metric catalogue, analysis, investigation scenarios, BI, assurance/UAT, independent handover, executive briefing and contribution evidence. A dashboard by itself does not satisfy the commission.

## Fixed core and optional work

**Core:** Use the agreed geography CSV. Completed-year trend baseline is 2020/21–2024/25; display 2025/26 August–April provisional figures separately. No year-on-year comparison with 2025/26 is permitted unless the same August–April window is available and verified. Use the publisher's per-100,000 population unit and available age/level/geography combinations.

**Extensions:** Learner completion/survival, course-duration effects, employer vacancies, subject alignment and individual progression need additional registered sources. Do not fetch the large learner files as a hidden core dependency.

Source support is checked at the Week 2 gate. A required output is blocked until its fields and cohort are verified; it cannot pass acceptance through a generic “data unavailable” disclaimer. An explicitly optional extension may remain unavailable with a reason. See [exact source URLs and verification evidence](data/SOURCE_REGISTER.md).

## Measurable project outcomes

1. No core trend compares August–April provisional activity with August–July full-year activity.
2. Every population rate uses per 100,000 and retains source age-reference limitations.
3. Every segment action distinguishes participation support from a request for linked progression evidence.

All headline metrics require field lineage; five source values and five BI measures must reconcile. DT1–DT10 must be executed, a second member must reproduce the core outputs, and no critical/high defect may remain. These assess delivery quality; real-world savings or service improvement are not claimed.

## Investigation rules

Compare weakening completed-year segments ordered by absolute starts/participation decline and by compatible population-adjusted participation decline. Keep 2025/26 partial-year signals in a separate provisional watchlist. Use identical eligibility criteria for the compared scenarios; no completion-risk score.

- Same-period starts and achievements refer to different learner cohorts; their ratio is not a completion rate.
- Keep overlapping totals and suppressed values separate from additive segment records.
- Do not infer local employer vacancies or labour-market alignment without additional governed evidence.

## Team and stakeholder ownership

Director of Skills & Employment approves business scope and the investigation recommendation. The Business Analyst, Data Governance Analyst, Data Engineer and BI Developer work with the specialist roles in the [project brief](project/PROJECT_BRIEF.md). Assign individual owners at kickoff and record substantive work and independent reviews in `CONTRIBUTIONS.md`.

## Delivery plan

Weeks 1–2: decision requirements and verified cohort. Weeks 3–4: model, reconciliation and metric definitions. Weeks 5–6: analytical findings, alternative investigation scenarios and BI draft. Weeks 7–8: simulated UAT, independent rerun, executive briefing and handover.

## Start here

1. [Project brief](project/PROJECT_BRIEF.md) and [business context](project/BUSINESS_CONTEXT.md).
2. [D1–D12 deliverables and metric contracts](project/DELIVERABLES.md).
3. [AC1–AC12 and DT1–DT10 acceptance tests](project/ACCEPTANCE_CRITERIA.md).
4. [Governance and sign-off](project/GOVERNANCE.md).
5. [Data workspace](data/README.md), [source register](data/SOURCE_REGISTER.md), [raw](data/raw/README.md), [reference](data/reference/README.md) and [metadata](data/metadata/README.md) guidance.
6. [Team repository standard](submission/TEAM_REPOSITORY_STANDARD.md), [submission guide](submission/SUBMISSION_GUIDE.md) and [final template](submission/FINAL_SUBMISSION_TEMPLATE.md).

## Master and team repositories

This master repository holds the Mettelo-controlled specification. Create `MTL-XF-024-<team-name>` under the **Mettelo GitHub organisation** and add every member's individual account. Delivery analysis, code, tests, BI and contribution evidence belong in that team repository. Use issues, branches, meaningful commits, PRs and reviews where practical.

The required master areas are `project/`, `data/` (including raw/reference/metadata guidance) and `submission/`; [the documentation index](project/README.md) explains their authority and current revision.

**Mettelo — Built for What’s Next**
