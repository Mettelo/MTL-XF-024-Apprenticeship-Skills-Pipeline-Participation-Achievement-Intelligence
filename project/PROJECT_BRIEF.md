# MTL-XF-024 — Project brief

## Engagement

This is a **simulated confidential-client engagement** using official public/open data. The client label is fictional and intentionally anonymous. Do not imply a real external Mettelo customer, employment by that client, privileged access or confidential source data. Public source statistics remain public; the engagement framing does not make them confidential.

**Simulated sponsor:** Confidential Regional Skills & Employer Engagement Authority. **Duration:** 8 weeks. **Team:** 6–8 members. **Track:** Cross-Functional. **Sector:** Education / Skills / Economic Development.

## Commission

Which geographic, age and apprenticeship-level segments warrant employer-engagement or participation-support investigation based on starts, participation and achievement patterns?

**Apprenticeship Skills Pipeline, Participation & Achievement Intelligence.** A regional skills authority wants to know whether apprenticeship starts are translating into participation and achievements, which age/level/geographic segments are weakening, and where employer or funding intervention may be required.

## Outcomes and boundaries

- Produce a starts/participation/achievements trend for comparable windows, with age/level/geography views only where present.
- Identify up to ten weakening skills segments and separate declining volume from population-adjusted participation.
- Compare count-led and rate-led support scenarios and list linked learner/employer evidence required before making progression claims.

Deliver evidence for a management investigation decision, with an auditable shortlist of up to ten cases and at least two alternative prioritisation scenarios. Do not manufacture a full shortlist where the data supports fewer cases. Findings may conclude that evidence is insufficient.

**Data boundary:** Use only the agreed DfE geography/starts/participation/achievements/population CSV, intended 2020/21–2025/26. Confirm available dimensions and reporting windows before modelling. Keep incomplete 2025/26 periods separate. Do not substitute the previously discussed 135–150 MB learner files.

**Model boundary:** Reporting year × coverage window × geography level/code × available age band × apprenticeship level × other published breakdowns. Population and learner measures may have different valid denominator coverage.

**Out of scope:** real operational deployment, confidential case-level data, guaranteed savings/outcome improvements, paid-source dependencies and automatic allocation of services or funding. Optional modelling or enriched sources must not delay or replace the core D1–D12 pack.

## Users and acceptance owners

- Simulated sponsor/review panel: approves commissioned question, changes and final investigation recommendation.
- Domain service/planning user: checks whether diagnostic evidence supports the proposed review action.
- Data steward: verifies source/version, licence, definitions, quality and retention evidence.
- BI user: tests overview, drill-down, filters and limitations.
- Independent reviewer: verifies calculations, rerun and requirement-to-test traceability.

These are simulated stakeholder roles, not claims of access to a real organisation.

## Work allocation

| Accountable role | Project responsibility and evidence |
| --- | --- |
| Business Analyst / Delivery Lead | Own the commissioned decision for Confidential Regional Skills & Employer Engagement Authority; record at least eight prioritised requirements, each linked to a deliverable and test; maintain weekly scope and decision logs. |
| Data Governance Analyst | Register every 024 input and critical field; approve the frozen cohort, licence evidence, glossary and 100% headline-KPI lineage before analysis. |
| Data Engineer | Implement the stated 024 analytical grain, ingestion and exclusions; deliver a clean rerun with row-count/checksum evidence and no unexplained key duplicates. |
| BI Developer | Build executive, diagnostic and quality views for the commissioned decision; reconcile at least five 024 dashboard measures and test every visible filter. |
| Skills Participation Analyst | Validate all eight measures and inspect comparable age/level/geographic trends. |
| Employer Engagement & Policy Analyst | Write up to ten segment-specific investigation actions and the employer evidence needed for each. |
| Skills Evaluation Analyst | Review cohort limitations and execute denominator, partial-year and unlinked-ratio tests. |

At kickoff, replace role ownership with named team members and record review partners in `CONTRIBUTIONS.md`. Multiple roles per member are permitted, but critical calculations need a reviewer distinct from their author.

## Working stages

1. Week 1: agree at least eight requirements and define expected decisions.
2. Week 2: inspect actual file schemas, establish available coverage and approve cohort freeze.
3. Week 3: implement and reconcile analytical facts, keys and exclusions.
4. Week 4: approve the 8-measure KPI catalogue and denominator rules.
5. Week 5: complete five supported findings and domain comparisons.
6. Week 6: compare two decision scenarios, produce the investigation shortlist and BI draft.
7. Week 7: execute ten or more assurance/UAT scenarios, including project-specific edge cases.
8. Week 8: independent rerun, executive briefing, presentation and final handover.

## Sign-off

Follow [D1–D12](DELIVERABLES.md) and [AC1–AC12](ACCEPTANCE_CRITERIA.md). Approve only with reproducible evidence, no unresolved critical/high defects and transparent conditional-data limitations. A change in source availability must be logged; do not silently substitute a newer release.
