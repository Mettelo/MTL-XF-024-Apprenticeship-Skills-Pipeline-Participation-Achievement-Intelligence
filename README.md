# MTL-XF-024 — Apprenticeship Skills Pipeline, Participation & Achievement Intelligence

**Mettelo Project Studio** · Cross-Functional · Master specification  
**Client:** Confidential Regional Skills & Employer Engagement Authority  
**Sector:** Education / Skills / Economic Development  
**Status:** Pre-launch; documentation ready, data acquisition/freeze pending  
**Recommended team:** 6–8 people · **Delivery window:** 8 weeks  
**Master repository:** `Mettelo/MTL-XF-024-Apprenticeship-Skills-Pipeline-Participation-Achievement-Intelligence`

> This is a **simulated confidential-client engagement** using official public/open data. The client label is fictional and intentionally anonymous. Do not imply a real external Mettelo customer, employment by that client, privileged access or confidential source data. Public source statistics remain public; the engagement framing does not make them confidential.

## Business challenge

**Apprenticeship Skills Pipeline, Participation & Achievement Intelligence.** A regional skills authority wants to know whether apprenticeship starts are translating into participation and achievements, which age/level/geographic segments are weakening, and where employer or funding intervention may be required.

Current reporting fragments the evidence needed for a repeatable management review. The team must explain which signals are reliable, which comparisons are valid and where further investigation is needed. No budget, operational failure or improvement outcome is asserted as an observed client fact.

## Commissioned decision

> Which geographic, age and apprenticeship-level segments warrant employer-engagement or participation-support investigation based on starts, participation and achievement patterns?

The product supports a simulated stakeholder review. A dashboard alone is insufficient: the recommendation must be traceable to governed definitions, a reproducible model, reconciled analysis and a transparent investigation framework.

## Business questions

- Where are starts, participation and achievements moving in different directions?
- Which available age/level/geographic segments show sustained decline?
- Where are comparable population-based participation gaps visible?
- How does the shortlist change when using counts versus valid population rates?
- What linked learner and employer evidence is needed to investigate progression or completion?

## Approved data and cohort

DfE Apprenticeships — geography, starts, participation, achievements and population dataset. It contains 100,864 rows and covers 2020/21–2025/26.

Use only the agreed DfE geography/starts/participation/achievements/population CSV, intended 2020/21–2025/26. Confirm available dimensions and reporting windows before modelling. Keep incomplete 2025/26 periods separate. Do not substitute the previously discussed 135–150 MB learner files.

Exact copyable URLs and acquisition gates are in [SOURCE_REGISTER.md](data/SOURCE_REGISTER.md). No raw data is uploaded by this build. Source coverage and size statements inherited from the agreement are expected values until controlled acquisition verifies them; current URLs are not a substitute for a frozen file manifest.

## What the team must build

1. Produce a starts/participation/achievements trend for comparable windows, with age/level/geography views only where present.
2. Identify up to ten weakening skills segments and separate declining volume from population-adjusted participation.
3. Compare count-led and rate-led support scenarios and list linked learner/employer evidence required before making progression claims.

Produce the full D1–D12 delivery pack: discovery, governance, ingestion/model, quality, KPI catalogue, analysis, decision framework, BI, assurance/UAT, handover, executive briefing and contribution record. [Deliverables](project/DELIVERABLES.md) defines locations, dates and evidence for each.

## Core measures

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

## Cross-functional ownership

| Accountable role | Project responsibility and evidence |
| --- | --- |
| Business Analyst / Delivery Lead | Own the commissioned decision for Confidential Regional Skills & Employer Engagement Authority; record at least eight prioritised requirements, each linked to a deliverable and test; maintain weekly scope and decision logs. |
| Data Governance Analyst | Register every 024 input and critical field; approve the frozen cohort, licence evidence, glossary and 100% headline-KPI lineage before analysis. |
| Data Engineer | Implement the stated 024 analytical grain, ingestion and exclusions; deliver a clean rerun with row-count/checksum evidence and no unexplained key duplicates. |
| BI Developer | Build executive, diagnostic and quality views for the commissioned decision; reconcile at least five 024 dashboard measures and test every visible filter. |
| Skills Participation Analyst | Validate all eight measures and inspect comparable age/level/geographic trends. |
| Employer Engagement & Policy Analyst | Write up to ten segment-specific investigation actions and the employer evidence needed for each. |
| Skills Evaluation Analyst | Review cohort limitations and execute denominator, partial-year and unlinked-ratio tests. |

Roles may be combined by a smaller team, but each responsibility needs a named owner. A different member reviews critical calculations and final evidence wherever practical.

## Interpretation rules

- Same-period starts and achievements refer to different learner cohorts; their ratio is not a completion rate.
- Keep overlapping totals and suppressed values separate from additive segment records.
- Do not infer local employer vacancies or labour-market alignment without additional governed evidence.

## Measurable success

- All source files and transformations have provenance and licence evidence; approved inputs have SHA-256 manifests.
- All headline metrics have tested definitions and source-field lineage.
- At least five published values and five dashboard measures reconcile with declared source rounding.
- At least five findings address the business questions and quantify materiality.
- Up to ten investigation cases have evidence, reason codes, owners and limitations; at least two priority scenarios are compared.
- At least ten UAT scenarios pass or have explicitly accepted low-impact limitations; no critical/high defect remains.
- A second member reproduces the core outputs from the same frozen inputs.

These are delivery acceptance thresholds, not promises of real-world service improvement. See [acceptance criteria](project/ACCEPTANCE_CRITERIA.md).

## Delivery sequence

Weeks 1–2: decision requirements, source inspection and freeze approval. Weeks 3–4: model, reconciliation and KPI definitions. Weeks 5–6: analysis, investigation framework and BI draft. Weeks 7–8: UAT, independent rerun, briefing and handover.

## Start here

1. Read the [project brief](project/PROJECT_BRIEF.md) and [business context](project/BUSINESS_CONTEXT.md).
2. Review [deliverables](project/DELIVERABLES.md), [acceptance criteria](project/ACCEPTANCE_CRITERIA.md) and [governance](project/GOVERNANCE.md).
3. Inspect the [data workspace](data/README.md), [source register](data/SOURCE_REGISTER.md), [raw guidance](data/raw/README.md), [reference guidance](data/reference/README.md) and [metadata guidance](data/metadata/README.md).
4. Create `MTL-XF-024-<team-name>` under the **Mettelo GitHub organisation**, add each member's individual account and follow the [team repository standard](submission/TEAM_REPOSITORY_STANDARD.md).
5. Use the [submission guide](submission/SUBMISSION_GUIDE.md) and [final submission template](submission/FINAL_SUBMISSION_TEMPLATE.md).

## Master and team repositories

This master holds the challenge specification. Teams deliver their analysis and artefacts in their own Mettelo organisation repository. Do not submit team work by replacing this master specification. Use issues, branches, meaningful commits, PRs and reviews to demonstrate actual collaboration.

## Specification map

```text
README.md
project/README.md
project/PROJECT_BRIEF.md
project/BUSINESS_CONTEXT.md
project/DELIVERABLES.md
project/ACCEPTANCE_CRITERIA.md
project/GOVERNANCE.md
data/README.md
data/SOURCE_REGISTER.md
data/raw/README.md
data/reference/README.md
data/metadata/README.md
submission/README.md
submission/TEAM_REPOSITORY_STANDARD.md
submission/SUBMISSION_GUIDE.md
submission/FINAL_SUBMISSION_TEMPLATE.md
```

**Mettelo — Built for What’s Next**
