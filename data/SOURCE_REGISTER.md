# MTL-XF-024 — Source register and verification record

**Project:** Apprenticeship Skills Pipeline, Participation & Achievement Intelligence  
**Documentation review:** 16 October 2026  
**State:** official documentation checked; acquired-file validation and freeze approval pending.  
**Steward:** Data Governance Analyst, with the project domain specialist.

## Source/cohort decision

Use the agreed geography CSV. Completed-year trend baseline is 2020/21–2024/25; display 2025/26 August–April provisional figures separately. No year-on-year comparison with 2025/26 is permitted unless the same August–April window is available and verified. Use the publisher's per-100,000 population unit and available age/level/geography combinations.

**Outside core:** Learner completion/survival, course-duration effects, employer vacancies, subject alignment and individual progression need additional registered sources. Do not fetch the large learner files as a hidden core dependency.

## Official publication and methodology references

| Official reference | URL |
| --- | --- |
| Official geography dataset and field preview | https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/a7743194-48bc-4e04-9102-4b0177ff4a84 |
| Release | https://explore-education-statistics.service.gov.uk/find-statistics/apprenticeships/2025-26 |
| Methodology navigation | https://explore-education-statistics.service.gov.uk/find-statistics/apprenticeships/2025-26/methodology |

References above were inspected for this revision. They establish only the evidence described below; they are not a completed file acquisition, licence clearance or signed freeze.

## Verification findings

The catalogue lists age_summary, apps_level, starts, participation, achievements, population_estimate and three indicative rates per 100,000. Footnotes distinguish programme-based starts/achievements from learner participation and their age reference dates. The current 2025/26 entries cover August–April provisionally; earlier years cover complete academic years. Field presence does not guarantee every dimensional combination.

**Field/reference mapping and acquisition instructions:** Map time_period/time_identifier, geographic_level, available geography code, apps_level and age_summary to the grain. Preserve population_estimate and *_rate_per_100000_population. Prefer publisher rates for reconciliation; compute alternatives only with the same valid denominator and recorded rounding.

**Remaining status:** Catalogue schema preview, rate unit and reporting-window footnotes verified; full file combinations, suppression, licences and freeze identity pending.

## Exact copyable file URLs

Original agreed URLs are retained. Entries labelled required supplement/reference or fallback are explicit changes from the initial pack. Do not silently replace an input with a newer release.

### S1 — Agreed core input 1

```text
https://explore-education-statistics.service.gov.uk/data-catalogue/data-set/a7743194-48bc-4e04-9102-4b0177ff4a84/csv
```

**Acquisition:** a candidate file already exists in the repository; validation/provenance and freeze approval remain pending. No source bytes were uploaded by this revision. Record actual version, coverage, schema and licence before approving use. Core source reference; actual file identity remains to be verified.

## Existing raw file observed during this revision

The repository already contains [app-geography-population-202526-q3.csv](raw/app-geography-population-202526-q3.csv), listed by GitHub as 20,469,846 bytes with Git blob SHA `c4e0571fbdce02f9975a8a6d6ca304b8c64ff18d`. It was preserved unchanged; this update did not upload it. The connector returned no preview content for the large file, so field/row validation, publisher-version matching, SHA-256 and freeze approval remain pending. A Git blob SHA is not the required acquisition SHA-256.

## File validation and licence record

For every actually used input record:

`source_id, role_core_reference_fallback_extension, original_url, resolved_url, retrieved_utc, actual_release, filename, bytes, sha256, format, sheets_or_members, rows, geography, period_start, period_end, grain, schema_version, methodology_evidence, licence_notice, attribution, redistribution_conditions, approved_by, approval_date`

Retain the relevant publication/file notices, including exceptions and third-party conditions. Do not assume all publishers use the same licence. A stated publication licence does not remove the need to check file-specific terms. Keep unverified values pending; never invent a hash or approval.

## Support and freeze decision

Complete the [source-to-deliverable matrix](README.md). The domain specialist verifies actual grain, units, period comparability and supported metrics; the steward verifies identity and reuse terms. Required missing fields block dependent core outputs. Every activated extension is separately registered. Where a fallback is used, record why, which original it replaces, overlap handling and impact on outputs.

If an agreed URL fails, seek the same official archived release and record evidence. A browser format limitation does not prove a file is unavailable, and a successful page fetch does not prove payload integrity. Preserve the frozen version and metadata in the approved location so future website changes do not silently alter the cohort.
