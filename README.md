# Codex credit depletion: public forensic review package

HORTRAME Systems | Public archive v1.0 | 6 October 2026

This repository publishes a client-side reconstruction of Codex tier settings, acute context-accounting activity and disputed credit depletion. It asks for independent technical review and request-level reconciliation, not acceptance of a predetermined billing conclusion.

## Download and verify

[Download the public evidence archive](https://raw.githubusercontent.com/hortrame-systems/openai_dispute/d4e223fd7b8556071614b556ed102b1fd75767e6/OpenAI_Codex_Forensic_Public_Review_Package_20261006_v1.0.zip).

The link is pinned to the original upload commit. The archive has not been changed by the addition of this landing page.

**SHA-256**

```text
2735eda6746b271a09526dbda245c706c7cdb3f9df6bc6cb8e9a6d8ad287e67a
```

[Zenodo DOI](https://doi.org/10.5281/zenodo.23192953) | [GitHub release](https://github.com/hortrame-systems/openai_dispute/releases/tag/v1.0) | [Checksum file](ZIP_SHA256SUMS.txt) | [Dated support history](SUPPORT_HISTORY.md) | [Provider records needed](PROVIDER_RECORDS.md) | [Related public tracker](https://github.com/openai/codex/issues/41220)

The archive contains the evidence tables, analysis, correction history and executable reproduction tools. The documents displayed here are a reading aid; the numbered archive remains the source for the released findings and their qualifications.

## What the record shows

The account owner reported recurring rapid credit use followed by an acute episode on **15 September 2026 in America/Toronto, corresponding to 16 September UTC**. The owner states that Fast/Priority was not knowingly authorized. That statement is testimony, not a finding about the historical authorization records.

The released client-side reconstruction identifies:

- Six paired persisted task segments with 56 usage updates and 50 post-initial continuations. Their final cumulative input counters sum to **29,225,371 tokens**.
- Post-initial deltas of **26,386,511 input tokens**, including **26,350,976 cached-input tokens**. These are accounting counters summed across segments, not unique context size, physical resident memory or one request containing 29 million tokens.
- **21 guardian submissions**, one represented in those six segments and 20 additional. Tokens and debits for the additional submissions remain unresolved.
- Five acute new-turn client requests carrying Priority fields. A defined September 2–15 known-tier settings cohort contains **1,441 Priority records out of 1,444**. This is a settings-event statistic, not a billed-token share.

Source: the archive's `README.md`, `03_CORRECTED_DERIVED_EVIDENCE/`, and the claim/source coverage under `07_EXTERNAL_REVIEW_MATERIALS/`.

## Workload generation and billing are different questions

Fast/Priority is relevant because it is a recorded tier state and a possible cost multiplier. A price multiplier does not explain why a workload generated repeated large cached-input counts. Context replay, orchestration, legitimate continuation and accounting behavior remain competing explanations.

This does **not** establish that ordinary charging cannot explain the acute depletion. The release retains a provider-favorable frozen-rate scenario mapping known-model usage to **651.3204 credits against a nominal 728-credit reported decline**, or **89.47% compatibility**. That scenario uses reported balances, a cross-time conversion and an assumed multiplier, and leaves additional guardian work unpriced. It proves neither historical billing correctness nor an additional overcharge.

A post-event configuration snapshot containing Priority is also preserved as an alternative local explanation. Its historical effectiveness and writer are unresolved.

## What remains unproved

The archive does not establish fraud, intent, wrong-account billing, unauthorized debits, double billing, a specific credit entitlement or causation by a cache defect. Large cached-input totals alone do not prove waste or environmental harm. Some extraction/authentication claims require retained confidential originals.

Historical tier authorization, request-to-account and funding-pool attribution, effective pricing, debit and settlement records are needed to reconcile the incident. Their absence from the client does not establish either party's conclusion. An ordinary, fully reconciled debit remains a possible result.

## Why the support history is included

On **3 October 2026 UTC**, Support represented one thread as open and escalated for provider-side reconciliation, but could not confirm that substantive examination had begun. On **6 October UTC**, another thread was closed without the requested reconciliation. The subsequent AI-assisted response could not confirm the earlier internal case states.

These statements document a procedural tension, not proof that every case was closed or that no internal investigation exists. The [dated support history](SUPPORT_HISTORY.md) preserves the distinctions. Private remediation in credits concerns the same underlying incident; the remedy is administered through Support rather than requested from public reviewers.

## Reproduce the included calculations

Python 3.11 or newer is required. The archive states that its Python programs use only the standard library. Keep the virtual environment outside the extracted package so it does not become part of the evidence directory.

Example from this repository's root on a Unix-like system:

```sh
sha256sum -c ZIP_SHA256SUMS.txt
unzip OpenAI_Codex_Forensic_Public_Review_Package_20261006_v1.0.zip
python3 -m venv .venv
cd OpenAI_Codex_Forensic_Public_Review_Package_20261006_v1.0
../.venv/bin/python -B 05_VERIFICATION/verify_public_release.py
../.venv/bin/python -B 05_VERIFICATION/run_included_reproductions.py
```

On Windows, use the virtual environment's `Scripts/python.exe` instead of `bin/python` and extract the ZIP with the normal archive tool.

Read `05_VERIFICATION/PUBLIC_REPRODUCTION.md` inside the archive before running the tools. Included arithmetic and counter-boundary checks are distinct from controlled-source re-extraction or verification of OpenAI's billing ledger.

## Review and corrections

Public reviewers are asked to identify reproducible errors, test alternative explanations, and cite the exact file, row, counter boundary or calculation involved. No common cause is assumed for other reports in the Codex tracker.

Do not publish credentials, private prompts, customer material, payment details or raw account identifiers in issues. Retain originals privately. The archive excludes confidential raw material and its private identifier map, and documents the associated provenance and access limits.

The archive's own README and release notes take precedence over shorthand descriptions of it. Corrections should be dated and reviewable, not silently substituted for a previously released finding.
