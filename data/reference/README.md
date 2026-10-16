# MTL-XF-024 — Reference data and mappings

## Purpose

Maintain the code lists and crosswalks needed to implement this analytical grain:

Reporting year × coverage window × geography level/code × available age band × apprenticeship level × other published breakdowns. Population and learner measures may have different valid denominator coverage.

Potential references are the publisher's geography/entity identifiers, category hierarchies, period definitions, units, status codes and revision markers. Include only references actually needed by the model. Register any separately downloaded official file as an additional source.

## Required mapping evidence

Each reference needs source/version, licence, valid-from/to dates, key uniqueness, allowed values, business meaning, owner and transformation use. For each crosswalk record source key, target key, relationship cardinality, rationale and treatment of unmapped or changed entities. Quantify 100% of unmatched keys; do not silently drop them or infer a mapping from similar names.

Avoid multiplying facts when a reference is many-to-many. Keep parent totals distinct from child categories. Non-official analyst-created groupings must be labelled as project assumptions and sensitivity-tested where they affect the investigation shortlist.

## Domain constraints

- Same-period starts and achievements refer to different learner cohorts; their ratio is not a completion rate.
- Keep overlapping totals and suppressed values separate from additive segment records.
- Do not infer local employer vacancies or labour-market alignment without additional governed evidence.

The domain specialist approves category meaning and comparability. The Data Engineer supplies uniqueness, join-cardinality and coverage checks before the reference enters the curated model.
