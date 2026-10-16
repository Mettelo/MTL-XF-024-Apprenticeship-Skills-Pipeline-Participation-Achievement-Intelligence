# MTL-XF-024 — Submission guide

## What to submit

Submit the Mettelo organisation team repository URL, final commit/tag, completed `submission/FINAL_SUBMISSION.md`, and links to D1–D12. Use the provided [template](FINAL_SUBMISSION_TEMPLATE.md). The final version must remain reproducible after review; record changes made after submission.

## Before submitting

1. Confirm the repository README states the simulated engagement and commissioned decision: Which geographic, age and apprenticeship-level segments warrant employer-engagement or participation-support investigation based on starts, participation and achievement patterns?
2. Complete the source manifest and cohort sign-off. Use only the agreed DfE geography/starts/participation/achievements/population CSV, intended 2020/21–2025/26. Confirm available dimensions and reporting windows before modelling. Keep incomplete 2025/26 periods separate. Do not substitute the previously discussed 135–150 MB learner files.
3. Link the requirements matrix, model, field lineage, quality/reconciliation evidence and all 8 metric definitions.
4. Link at least five findings and the up-to-ten-case investigation shortlist, including owners, evidence gaps and two compared scenarios.
5. Reconcile at least five headline dashboard measures and test all visible filters; provide a free review path and static export.
6. Execute ten or more UAT scenarios, including all domain cases below. Resolve critical/high defects and disclose any accepted remaining limitations.
7. Have another member reproduce the core outputs using documented steps; retain the run environment, checks and results.
8. Complete contribution evidence for each member and prepare the two-page briefing and 15–20 minute presentation.

## Required domain checks

1. Reconcile five starts, participation or achievements measures to published cells.
2. Reject a population denominator with mismatched age or geography.
3. Test that a partial-year starts count cannot be compared with a full year.
4. Verify achievement-to-starts ratios are never labelled completion rates, including when above one.

## Panel presentation

Explain the decision, actual cohort and limitations; demonstrate one source-to-KPI-to-dashboard chain; present five findings; compare two prioritisation scenarios; justify the investigation cases; show one case where action is not supported; describe next evidence-gathering steps and named role ownership.

Expect challenges on definitions, denominators, exclusions, comparability, threshold choices, sensitivity, reproducibility and contribution. Label feedback and approvals as simulated where appropriate. Do not invent contact with real stakeholders.

## Acceptance and changes

Use [AC1–AC12](../project/ACCEPTANCE_CRITERIA.md) to record pass/fail, evidence and reviewer. An unavailable conditional analysis needs a supported explanation and alternative; it cannot be disguised as a result. Source changes require registration, impact review and rerun. Final acceptance is recorded by the simulated Mettelo review panel, not self-certified as a real-client outcome.
