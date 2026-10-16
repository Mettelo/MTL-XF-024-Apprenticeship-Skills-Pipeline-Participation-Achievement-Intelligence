# MTL-XF-024 — Required deliverables

**Commissioned decision:** Which geographic, age and apprenticeship-level segments warrant employer-engagement or participation-support investigation based on starts, participation and achievement patterns?

All locations below refer to the team's delivery repository. The master repository defines the requirements and contains no completed analysis. Owners are assigned from [the project roles](PROJECT_BRIEF.md).

## D1 — Discovery & decision requirements

**Due:** Week 1  
**Team artefact location:** `docs/01-discovery/`

Decision statement; stakeholder map; as-is reporting to investigation-review process; at least eight prioritised requirements. Answer these questions: Where are starts, participation and achievements moving in different directions? Which available age/level/geographic segments show sustained decline? Where are comparable population-based participation gaps visible? How does the shortlist change when using counts versus valid population rates? What linked learner and employer evidence is needed to investigate progression or completion?

**Acceptance evidence:** All requirements have an owner, priority, deliverable and test ID; domain analyst approves scope.

## D2 — Governed sources & cohort

**Due:** Week 2  
**Team artefact location:** `docs/02-data-governance/; data/`

Use only the agreed DfE geography/starts/participation/achievements/population CSV, intended 2020/21–2025/26. Confirm available dimensions and reporting windows before modelling. Keep incomplete 2025/26 periods separate. Do not substitute the previously discussed 135–150 MB learner files. Register exact files, metadata, licences, checksums, coverage and critical fields; record rejection of unavailable dimensions.

**Acceptance evidence:** 100% of inputs registered; no claimed freeze until acquisition evidence exists.

## D3 — Reproducible analytical model

**Due:** Week 3  
**Team artefact location:** `src/; sql/; docs/03-data-model/`

Reporting year × coverage window × geography level/code × available age band × apprenticeship level × other published breakdowns. Population and learner measures may have different valid denominator coverage. Deliver load, type checks, hierarchy handling, lineage, exclusions and environment instructions.

**Acceptance evidence:** A second member regenerates equivalent curated outputs from identical inputs; no unexplained duplicate analytical keys.

## D4 — Quality & reconciliation

**Due:** Week 3  
**Team artefact location:** `docs/04-data-quality/; tests/`

Profile missingness, suppression, valid values, keys and join coverage. Reconcile five starts, participation or achievements measures to published cells. Reject a population denominator with mismatched age or geography. Test that a partial-year starts count cannot be compared with a full year. Verify achievement-to-starts ratios are never labelled completion rates, including when above one.

**Acceptance evidence:** Every input row is accounted for as retained, excluded or quarantined; five published cells reconcile within declared rounding.

## D5 — KPI catalogue

**Due:** Week 4  
**Team artefact location:** `docs/05-kpi-catalogue/`

Define all 8 measures listed below with formula, grain, denominator, unit, source fields, exclusions, owner, refresh and limitations.

**Acceptance evidence:** 100% headline metrics trace to source fields and tested transformations; conditional unavailable measures are explicitly marked.

## D6 — Domain analytical assessment

**Due:** Week 5  
**Team artefact location:** `analysis/; docs/06-analysis/`

Produce a starts/participation/achievements trend for comparable windows, with age/level/geography views only where present. Identify up to ten weakening skills segments and separate declining volume from population-adjusted participation.

**Acceptance evidence:** At least five evidence-backed findings state period, population, comparison, magnitude, uncertainty and limitation; negative findings count.

## D7 — Investigation decision framework

**Due:** Week 6  
**Team artefact location:** `docs/07-decision-framework/`

Compare count-led and rate-led support scenarios and list linked learner/employer evidence required before making progression claims. Record eligibility, thresholds, weights if used, reason codes and manual review triggers.

**Acceptance evidence:** Every shortlisted case has metrics, rationale, owner and evidence gaps; at least two scenarios compared; fewer than ten is valid where evidence is insufficient.

## D8 — BI decision-support product

**Due:** Draft Week 6; final Week 7  
**Team artefact location:** `dashboard/`

Executive overview answering 'Which geographic, age and apprenticeship-level segments warrant employer-engagement or participation-support investigation based on starts, participation and achievement patterns?' plus diagnostic and data-quality views; visible periods, units, denominator notes, resettable filters and accessible labels.

**Acceptance evidence:** Five headline measures reconcile; every filter tested; export screenshots/PDF plus reproducible build or free access instructions.

## D9 — Independent assurance & UAT

**Due:** Week 7  
**Team artefact location:** `docs/08-assurance-uat/`

At least ten scenarios including the four project-specific tests below; requirement-to-test matrix, expected/actual evidence, defect log and simulated stakeholder feedback.

**Acceptance evidence:** No unresolved critical/high defect; accepted lower-severity limitations have a named reviewer and explicit impact.

## D10 — Technical & operational handover

**Due:** Week 8  
**Team artefact location:** `docs/09-technical-handover/`

Clean setup, architecture, frozen input manifest, run/refresh steps, output checks, troubleshooting and change-control process for Apprenticeship Skills Pipeline, Participation & Achievement Intelligence.

**Acceptance evidence:** Another member reproduces the core outputs without undocumented edits and records environment, duration and discrepancies.

## D11 — Executive recommendation

**Due:** Week 8  
**Team artefact location:** `deliverables/`

Maximum two-page briefing and 15–20 minute presentation: commissioned decision, five findings, investigation shortlist, sensitivity, missing evidence, responsibilities and next review.

**Acceptance evidence:** Every quantitative claim links to an artefact/metric; no unsupported causal, policy or operational guarantee.

## D12 — Contribution & delivery record

**Due:** Weekly; final Week 8  
**Team artefact location:** `CONTRIBUTIONS.md; delivery issues/PRs`

Record who delivered and reviewed each MTL-XF-024 work package, including domain, governance, engineering, BI and assurance contributions.

**Acceptance evidence:** Every member links to substantive artefacts and review/presentation evidence; commit count alone is insufficient.

## Required KPI definitions

| Metric | Required definition / calculation |
| --- | --- |
| Starts | Published apprenticeship starts for the exact period and segment. |
| Participation | Published participation measure; retain publisher definition of persons/episodes and period. |
| Achievements | Published achievements for the exact period and segment. |
| Comparable starts change | Current starts minus previous matching-window starts, plus percentage change where base > 0. |
| Population participation rate | 1,000 × participation / compatible published population where ages, geography and period align. |
| Achievement-to-starts activity ratio | Achievements / starts in the same period; label as an unlinked activity ratio, never a completion probability. |
| Segment share | 100 × segment starts / compatible parent starts, excluding overlapping categories. |
| Coverage | Valid non-suppressed segment-period cells / expected selected cells. |

For every metric record business purpose, formula, source fields, grain, unit, numerator/denominator, exclusions, suppression, zero-base behaviour, owner, refresh and test evidence. Do not populate conditional metrics from invented fields.

## Mandatory domain scenarios

1. Reconcile five starts, participation or achievements measures to published cells.
2. Reject a population denominator with mismatched age or geography.
3. Test that a partial-year starts count cannot be compared with a full year.
4. Verify achievement-to-starts ratios are never labelled completion rates, including when above one.

## Review gates

Week 2: cohort and source approval. Week 4: model, DQ and metrics approval. Week 6: analytical and decision-framework review. Week 8: UAT, independent rerun and final panel review. Record reviewer, date, artefact version and decision at every gate.
