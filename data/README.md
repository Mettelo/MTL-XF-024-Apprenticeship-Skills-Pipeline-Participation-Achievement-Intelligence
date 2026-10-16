# MTL-XF-024 — Data workspace and support gate

## Core contract

Use the agreed geography CSV. Completed-year trend baseline is 2020/21–2024/25; display 2025/26 August–April provisional figures separately. No year-on-year comparison with 2025/26 is permitted unless the same August–April window is available and verified. Use the publisher's per-100,000 population unit and available age/level/geography combinations.

## Optional work

Learner completion/survival, course-duration effects, employer vacancies, subject alignment and individual progression need additional registered sources. Do not fetch the large learner files as a hidden core dependency.

## Acquisition state

No raw data is uploaded by this update. Official documentation checks are recorded in [SOURCE_REGISTER.md](SOURCE_REGISTER.md). File payloads, full schemas, bytes/checksums and final reuse/freeze approvals remain pending where stated. Keep publication-level evidence distinct from acquired-file evidence.

## Required source-to-deliverable matrix

Before analysis, create a row per headline measure/required comparison:

`requirement_id | deliverable_id | metric | core_or_extension | source_id | actual_field_or_sheet | valid_grain | coverage | unit_denominator | metadata_evidence | support_status | owner | decision`

Allowed support statuses: documentation-supported; payload-verified; unsupported; optional-not-activated. “Documentation-supported” alone is insufficient for a completed data freeze. If a mandatory field is absent, block its output and resolve the source or approved scope; do not fabricate values or silently waive the requirement.

## Controlled preparation

1. Use registered exact URLs and inspect actual content type, archive members or sheets.
2. Record version, resolved URL, separate retrieval timestamps, bytes, SHA-256 and licence evidence.
3. Approve the actual cohort and scope matrix at G1.
4. Preserve original bytes; transform into curated facts with documented types, keys, hierarchies and joins.
5. Account for retained/excluded/quarantined rows and quantify all mapping gaps.
6. Reconcile five source values and execute [DT1–DT10](../project/ACCEPTANCE_CRITERIA.md).

## Model and measures

Reporting year × coverage window × geography level/code × available age band × apprenticeship level × other published breakdowns. Population and learner measures may have different valid denominator coverage.

The core contract above controls conditional dimensions. Metric formulas have one authoritative home: [DELIVERABLES.md](../project/DELIVERABLES.md). Do not create another incompatible formula copy in the data README.

## Data areas

- [Raw snapshots](raw/README.md): unmodified source bytes only when later authorised and permitted.
- [Reference data](reference/README.md): category/entity/period mappings with version and cardinality.
- [Metadata](metadata/README.md): manifest, dictionary, methodology, lineage and support/freeze decisions.

**Specific control:** Partial-year comparisons and same-period achievement ratios can create false claims about weakening learner completion.
