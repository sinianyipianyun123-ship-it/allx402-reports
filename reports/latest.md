# AllX402 Weekly Verification Report — 2026-W32

Generated: 2026-08-09T13:46:25.288Z

## Snapshot

| Metric | Value |
|---|---:|
| Catalog records | 208 |
| Active records | 202 |
| Canonical x402 v2 | 170 |
| Legacy or non-canonical | 32 |
| Time-spaced candidates | 10 |
| Time-spaced passes | 0 |
| Paid delivery calls | 0 |
| Paid delivery successes | 0 |

## Protocol probe outcomes

- `endpoint_failed`: 2
- `method_not_tested`: 3
- `probe_inconclusive`: 1
- `protocol_verified`: 202

## Protocol compatibility

- `legacy_or_noncanonical`: 32
- `not_verified`: 6
- `standard_x402_v2`: 170

## Time-spaced unpaid screening

- Input available: yes
- Candidates: 10
- Completed rounds: 1 round(s): 10
- Time-spaced passes: 0
- Paid-test eligible after all gates: 0

Screening status:

- `deep_screen_pending`: 9
- `method_not_tested`: 1

## Paid delivery verification

- Paid calls: 0
- Succeeded with validated delivery: 0
- Failed: 0
- Ambiguous: 0
- Success rate: Not available

Protocol verification and paid-delivery verification are separate. A valid HTTP 402 response does not prove that payment was made or that useful content was delivered.

## Reviewed status changes

No reviewed status-change input was supplied; this does not mean that no changes occurred.

- No records available.

## Limitations

- A valid unpaid HTTP 402 challenge does not prove paid delivery.
- Closely spaced historical probes are not counted as time-spaced screening passes.
- Observed prices are snapshots; callers must read the live 402 quote before any payment.
- Missing paid-test or change-log inputs are reported as unavailable, not inferred.
