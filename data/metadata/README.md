# MTL-XF-024 — Metadata, lineage and freeze evidence

Metadata makes apprenticeship skills pipeline, participation & achievement intelligence reproducible. This folder currently contains guidance; no acquisition manifest or source sign-off is claimed.

## Required records after acquisition

- Source manifest: source ID, exact/resolved URL, retrieval UTC, actual release, filename, bytes, SHA-256, archive members/sheets and coverage.
- Publisher methodology and licence/attribution evidence with provenance and retrieval date.
- Schema and field dictionary: name, type, meaning, units, key role, missing/suppression markers and valid values.
- Business glossary and critical data elements, with named steward and approved definitions.
- Grain, hierarchy and join-cardinality documentation.
- Field-level lineage from raw fields through transformations to each headline metric/dashboard measure.
- Quality profile, row-accounting reconciliation, exclusions, unresolved exceptions and their decision impact.
- Freeze approval, change log and later revision comparisons.

## Model contract

Reporting year × coverage window × geography level/code × available age band × apprenticeship level × other published breakdowns. Population and learner measures may have different valid denominator coverage.

## Metric definition coverage

- Starts: Published apprenticeship starts for the exact period and segment.
- Participation: Published participation measure; retain publisher definition of persons/episodes and period.
- Achievements: Published achievements for the exact period and segment.
- Comparable starts change: Current starts minus previous matching-window starts, plus percentage change where base > 0.
- Population participation rate: 1,000 × participation / compatible published population where ages, geography and period align.
- Achievement-to-starts activity ratio: Achievements / starts in the same period; label as an unlinked activity ratio, never a completion probability.
- Segment share: 100 × segment starts / compatible parent starts, excluding overlapping categories.
- Coverage: Valid non-suppressed segment-period cells / expected selected cells.

Every listed metric needs source fields, transformation/formula, valid grain, unit, numerator/denominator, exclusions, zero/missing behaviour, refresh expectation, owner and test reference. Mark conditional metrics unavailable if the actual source cannot support them.

Store actual evidence only; never invent publisher schema, a completed licence review, a checksum or a stakeholder approval. See [source register](../SOURCE_REGISTER.md) and [acceptance criteria](../../project/ACCEPTANCE_CRITERIA.md).
