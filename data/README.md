# MTL-XF-024 — Data workspace

## Required sources and cohort

DfE Apprenticeships — geography, starts, participation, achievements and population dataset. It contains 100,864 rows and covers 2020/21–2025/26.

Use only the agreed DfE geography/starts/participation/achievements/population CSV, intended 2020/21–2025/26. Confirm available dimensions and reporting windows before modelling. Keep incomplete 2025/26 periods separate. Do not substitute the previously discussed 135–150 MB learner files.

[Source register and exact URLs](SOURCE_REGISTER.md)

**Current state:** specification only. No raw datasets have been downloaded or uploaded in this build. Expected size, row count and history statements from the earlier agreement require verification against the actual files. Do not mark the cohort frozen until the manifest and metadata are complete.

## Controlled acquisition and preparation

1. Read [SOURCE_REGISTER.md](SOURCE_REGISTER.md); use the exact agreed URLs and official publisher documentation.
2. Validate that the response is the expected CSV/ODS/XLSX/ZIP rather than an error page. Inspect archive contents and sheet names where relevant.
3. Record resolved URL, UTC retrieval, release, coverage, filename, bytes, SHA-256 and licence evidence. Log discrepancies before changing sources.
4. Preserve original bytes in an approved immutable snapshot; later upload only where instructed and redistribution is permitted.
5. Record source fields, types, valid values, suppression, units and publisher methodology in [metadata](metadata/README.md).
6. Implement the analytical grain below, verify keys/cardinality and account for excluded/quarantined records.
7. Reconcile at least five published measures and create curated outputs reproducibly in the team repository.

## Analytical grain

Reporting year × coverage window × geography level/code × available age band × apprenticeship level × other published breakdowns. Population and learner measures may have different valid denominator coverage.

## Required metric contract

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

## Mandatory quality risks

- Same-period starts and achievements refer to different learner cohorts; their ratio is not a completion rate.
- Keep overlapping totals and suppressed values separate from additive segment records.
- Do not infer local employer vacancies or labour-market alignment without additional governed evidence.

1. Reconcile five starts, participation or achievements measures to published cells.
2. Reject a population denominator with mismatched age or geography.
3. Test that a partial-year starts count cannot be compared with a full year.
4. Verify achievement-to-starts ratios are never labelled completion rates, including when above one.

## Folder ownership

- [raw](raw/README.md): unmodified approved source snapshots; guidance only at present.
- [reference](reference/README.md): governed code lists, hierarchies and crosswalks.
- [metadata](metadata/README.md): source notices, schema, glossary, lineage and manifest evidence.

Curated data, processing code, logs and test results belong in the team delivery repository. Preserve a reproducible boundary between source inputs and generated products. Do not add personal, confidential or paid-source data.
