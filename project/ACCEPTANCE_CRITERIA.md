# MTL-XF-024 — Acceptance criteria and domain tests

**Business decision owner:** Director of Skills & Employment. **Decision:** Which geographic, age and apprenticeship-level segments warrant employer-engagement or participation-support investigation based on starts, participation and achievement patterns?

## Delivery sign-off

| ID | Deliverables | Required pass evidence | Acceptance owner |
| --- | --- | --- | --- |
| AC1 | D1 | Eight user requirements cover the commissioned questions, named stakeholder actions and core/extension boundary. | Business Analyst / Director of Skills & Employment |
| AC2 | D2 | 100% of used source files have approved provenance, version/coverage, licence, retrieval UTC and SHA-256. Required fields and reference versions are checked. | Data Governance Analyst |
| AC3 | D3 | Every input row is accounted for; keys and all many-to-many/hierarchy effects have explicit checks and no unexplained duplication. | Data Engineer / independent reviewer |
| AC4 | D4 | Five source cells reconcile within a declared rounding tolerance; all material differences and non-additive totals are explained. | Domain specialist |
| AC5 | D5 | All 8 metric contracts are classified core/conditional and have tested definitions; no unsupported fields or fabricated unavailable values. | Data Governance Analyst / BI Developer |
| AC6 | D6 | Five findings cover all business questions or evidence gaps; period, eligible population, magnitude, comparison and limitation are visible. | Domain analyst |
| AC7 | D7 | The project-specific baseline and alternative below are implemented; eligibility, scenario changes, reason codes and evidence requests are visible. | Director of Skills & Employment |
| AC8 | D8 | Five BI measures reconcile to curated outputs; all filters/reset/export retain the scope, units and limitations. | BI Developer / operational UAT user |
| AC9 | D9 | DT1–DT10 have actual execution evidence and expected/actual outcomes; no unresolved critical/high defect. | Independent reviewer |
| AC10 | D10 | A distinct member's clean rerun reproduces equivalent core outputs with documented environment and checks. | Independent rerun reviewer |
| AC11 | D11 | Two-page maximum briefing and 15–20 minute presentation answer the decision and assign investigation owners without unsupported outcomes. | Director of Skills & Employment / Mettelo panel |
| AC12 | D12 | Every member links substantive authored and reviewed work, including handover or presentation contribution. | Delivery Lead |

## Project-specific business success

1. No core trend compares August–April provisional activity with August–July full-year activity.
2. Every population rate uses per 100,000 and retains source age-reference limitations.
3. Every segment action distinguishes participation support from a request for linked progression evidence.

## Required prioritisation and sensitivity

Compare weakening completed-year segments ordered by absolute starts/participation decline and by compatible population-adjusted participation decline. Keep 2025/26 partial-year signals in a separate provisional watchlist. Use identical eligibility criteria for the compared scenarios; no completion-risk score.

Record each case's entity/segment, valid period, supporting measures, reason code, scenario position, missing evidence, responsible operational role, next review and manual-review trigger. Fewer than ten cases is valid; padding unsupported cases fails acceptance.

## DT1–DT10 — minimum executed domain tests

| Test | Input / action | Expected pass evidence |
| --- | --- | --- |
| DT1 | Reconcile five starts, participation or achievements measures to published cells. | Five selected published values reproduce within declared source precision, with explicit source coordinates and scope. |
| DT2 | Reject a population denominator with mismatched age or geography. | The invalid comparison, join or denominator is rejected or flagged according to the documented rule; no silent fallback. |
| DT3 | Test that a partial-year starts count cannot be compared with a full year. | The edge case produces an explicit unavailable/exclusion result or a supported calculation, with affected rows quantified. |
| DT4 | Verify achievement-to-starts ratios are never labelled completion rates, including when above one. | The domain boundary remains visible in the analytical output and BI product; no unsupported inference. |
| DT5 | 500 participants / 100,000 compatible population | Rate = 500 per 100,000; do not label it per 1,000. |
| DT6 | 2025/26 August–April versus prior August–July | Year-on-year change unavailable unless a matching-window series is registered. |
| DT7 | Starts and participation use different published age conventions | Document that difference; do not interpret the age mix as linked progression. |
| DT8 | One learner has two starts but one participation count | Programme events and learner counts are not forced to match. |
| DT9 | An age/level total appears beside component rows | Do not add total and components or imply full additivity without a check. |
| DT10 | A latest-year provisional card is exported | Provisional status and coverage months remain visible in the export. |

Worked values are **synthetic test fixtures**, not claims about the public data or simulated client. For each test retain requirement ID, source/input or fixture, expected result, actual result, evidence link, tester, independent reviewer and date. DT1–DT4 additionally require the documented project-specific rule; their general evidence descriptions do not waive the named domain condition. Add dashboard/filter tests as needed beyond these ten.

## Scope gate and unresolved issues

**Mandatory core:** Use the agreed geography CSV. Completed-year trend baseline is 2020/21–2024/25; display 2025/26 August–April provisional figures separately. No year-on-year comparison with 2025/26 is permitted unless the same August–April window is available and verified. Use the publisher's per-100,000 population unit and available age/level/geography combinations.

**Optional extensions:** Learner completion/survival, course-duration effects, employer vacancies, subject alignment and individual progression need additional registered sources. Do not fetch the large learner files as a hidden core dependency.

A mandatory source/field gap blocks the affected deliverable and must be resolved by a registered official replacement or approved, versioned scope change. An explicitly optional result may be unavailable with a reason and a useful evidence request. Neither missing raw data nor unexecuted tests may be marked passed.

A critical/high defect materially changes a headline value, cohort, recommendation, provenance or reproducibility and blocks release. Lower-impact issues require a named acceptance owner and disclosed impact. All panel feedback and approvals must be recorded honestly as simulated where applicable.
