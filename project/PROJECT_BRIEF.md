# MTL-XF-024 — Project brief

This is a **simulated confidential-client engagement using official public/open data**. Client and stakeholder role labels describe a fictional engagement; do not claim a real external Mettelo customer, employment, endorsement or privileged data access. No raw data is uploaded by this specification update.

**Client:** Confidential Regional Skills & Employer Engagement Authority. **Decision owner:** Director of Skills & Employment. **Team:** 6–8. **Duration:** 8 weeks. **Review:** quarterly skills participation and employer-engagement review.

## Business problem and commission

The simulated regional skills authority plans employer-engagement and participation-support activity through a quarterly review. Its teams need to decide which geographic, age and apprenticeship-level segments deserve closer enquiry before commissioning new outreach.

The Director of Skills & Employment needs to target employer-engagement and participation-support work where the apprenticeship pipeline appears to be weakening. Separate starts, participation and achievements reports do not show whether an apparent change reflects fewer entrants, a different age/level mix or a non-comparable reporting window.

An unsupported completion narrative could send staff towards provider-performance enquiries when the real question is participation or employer demand. The commission is to provide a comparable segment review and an outreach agenda, while clearly separating what aggregate annual activity can show from questions requiring linked learner or employer evidence.

> Which geographic, age and apprenticeship-level segments warrant employer-engagement or participation-support investigation based on starts, participation and achievement patterns?

**Required management handover:** A skills review pack with completed-year segment trends, a separately labelled provisional watchlist, count-led and rate-led scenarios, and an employer-engagement enquiry register. Each enquiry must name the segment, supported signal, lead role and evidence needed to distinguish participation from learner progression.

See [the management use case](BUSINESS_CONTEXT.md#practical-management-use-case) for how the review meeting uses this evidence.

## Core deliverable boundary

Use the agreed geography CSV. Completed-year trend baseline is 2020/21–2024/25; display 2025/26 August–April provisional figures separately. No year-on-year comparison with 2025/26 is permitted unless the same August–April window is available and verified. Use the publisher's per-100,000 population unit and available age/level/geography combinations.

**Optional / out of core:** Learner completion/survival, course-duration effects, employer vacancies, subject alignment and individual progression need additional registered sources. Do not fetch the large learner files as a hidden core dependency.

File availability does not prove dimensional support. Before analytical build, the team completes the source→field→metric→deliverable matrix in [data guidance](../data/README.md). Missing mandatory support blocks the gate and requires an approved official replacement or scope decision.

## Analytical model

Reporting year × coverage window × geography level/code × available age band × apprenticeship level × other published breakdowns. Population and learner measures may have different valid denominator coverage.

The source contract above controls where a general grain description is conditional. Do not create dimensions absent from the approved input.

## Objectives

1. No core trend compares August–April provisional activity with August–July full-year activity.
2. Every population rate uses per 100,000 and retains source age-reference limitations.
3. Every segment action distinguishes participation support from a request for linked progression evidence.

## Business questions

1. Where are starts, participation and achievements moving in different directions?
2. Which available age/level/geographic segments show sustained decline?
3. Where are comparable population-based participation gaps visible?
4. How does the shortlist change when using counts versus valid population rates?
5. What linked learner and employer evidence is needed to investigate progression or completion?

## Cross-functional delivery model

| Delivery role | Required project contribution |
| --- | --- |
| Business Analyst / Delivery Lead | Map the quarterly skills participation and employer-engagement review, document eight prioritised user requirements and maintain requirement→deliverable→test links; Director of Skills & Employment owns business approval. |
| Data Governance Analyst | Own the MTL-XF-024 source/metadata register, cohort decision, licence evidence and 100% headline-measure lineage; resolve the specific risk: Partial-year comparisons and same-period achievement ratios can create false claims about weakening learner completion. |
| Data Engineer | Implement the declared facts, keys, hierarchy and join controls; account for every source row and deliver a second-member reproducible run at the chosen MTL-XF-024 scope. |
| BI Developer | Implement the quarterly skills participation and employer-engagement review overview, diagnostic and quality pages; reconcile five measures and ensure cohort/extension warnings survive filters and export. |
| Skills Participation Analyst | Validate all eight measures and inspect comparable age/level/geographic trends. |
| Employer Engagement & Policy Analyst | Write up to ten segment-specific investigation actions and the employer evidence needed for each. |
| Skills Evaluation Analyst | Review cohort limitations and execute denominator, partial-year and unlinked-ratio tests. |

Assign named team members and review partners at kickoff; roles may be combined, but a distinct member must review critical calculations and perform the final clean rerun. The executive and operational stakeholder roles are specified in [business context](BUSINESS_CONTEXT.md).

## Required investigation approach

Compare weakening completed-year segments ordered by absolute starts/participation decline and by compatible population-adjusted participation decline. Keep 2025/26 partial-year signals in a separate provisional watchlist. Use identical eligibility criteria for the compared scenarios; no completion-risk score.

## Milestones and acceptance

| Gate | Reviewers | Evidence / decision |
| --- | --- | --- |
| G1 — scope/source, end Week 2 | Business Analyst + Data Governance Analyst + domain specialist | Approve actual period, geography, grain, required input and field support in a source-to-deliverable matrix. Catalogue schema preview, rate unit and reporting-window footnotes verified; full file combinations, suppression, licences and freeze identity pending. Unsupported mandatory outputs remain blocked, not quietly reclassified as completed. |
| G2 — model/metrics, end Week 4 | Data Engineer + domain specialist + independent reviewer | Approve row accounting, keys, hierarchy, join cardinality, five source reconciliations and all core metric definitions. |
| G3 — analytical decision review, end Week 6 | Director of Skills & Employment + operational stakeholders | Compare weakening completed-year segments ordered by absolute starts/participation decline and by compatible population-adjusted participation decline. Keep 2025/26 partial-year signals in a separate provisional watchlist. Use identical eligibility criteria for the compared scenarios; no completion-risk score. Retain an evidence-insufficient case and a manual review route. |
| G4 — release, end Week 8 | Simulated Mettelo panel + independent reviewer | Accept D1–D12 only after ten executed domain tests, five BI reconciliations, clean rerun evidence and resolution of all critical/high defects. |

D1–D12 are defined in [deliverables](DELIVERABLES.md). AC1–AC12 and DT1–DT10 are defined in [acceptance criteria](ACCEPTANCE_CRITERIA.md). No real production deployment, automatic funding/service allocation, private-client data or paid-source dependency is required.
