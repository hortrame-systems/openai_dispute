# Provider records needed for reconciliation

Reading copy of `02_PUBLIC_REVIEW/PROVIDER_RECORDS.md` in the v1.0 public archive.

For each disputed request or debit, the remaining questions require:

1. Request, response, turn and parentage identifiers, with timestamps and completion/retry status.
2. Requested and historically resolved service tier; effective configuration/catalog revision.
3. Authorization provenance: writer, previous setting, source surface/admin/default, time and applicable consent.
4. Input, cached-input, output and reasoning usage at the billed request's accounting boundary.
5. Account, workspace/seat, authentication principal, and included versus purchased funding pool.
6. Historical rates, model/tier/long-context multiplier stack, plan entitlement and allowance resets.
7. Purchase/reload transactions, effective threshold/limit, credit quantities, balance and unused/expired/stranded credits.
8. Request-level credit debits, before/after balances, delayed settlement or negative-balance behavior, deduplication and adjustments.
9. Guardian/background request accounting and its linkage to user work.

Stable opaque identifiers or an attributable provider attestation can preserve row-level linkage without disclosing unrelated provider internals. Aggregate assurance cannot supply the missing linkage.

These records are discriminating evidence, not an inference about what the ledger must show or a unilateral claim of legal authority over it. Absence from the client is neutral. A fully reconciled ordinary debit is a valid possible result.
