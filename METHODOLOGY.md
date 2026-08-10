# Methodology

AllX402 public reports are generated from an internal catalog snapshot and reviewed evidence inputs. The public repository contains generated aggregate outputs only; it does not run probes, a website, a wallet, or a payment service.

## Evidence boundaries

- **Protocol probe outcome** records whether an unpaid request produced a parseable HTTP 402 challenge.
- **Time-spaced unpaid screening** requires three independent rounds at the configured intervals. It is not paid-delivery evidence.
- Round 2 must occur 5–18 hours after Round 1. Round 3 must occur 18–36 hours after Round 1 and at least 5 hours after Round 2. Reports publish the observed offsets rather than replacing them with target times.
- **Paid delivery success** requires a paid request plus validated delivery. Ambiguous outcomes are reported separately and excluded from the success-rate denominator.
- Rate-limited, access-blocked, method-not-tested, and platform-inconclusive outcomes must not be silently counted as supplier failures.

## Publication controls

The generator uses an aggregate field whitelist. Public artifacts exclude endpoints, recipient addresses, transaction hashes, request headers, raw responses, stack traces, local filesystem paths, secrets, unreviewed candidate details, and personal or customer data.

When a source file is absent, the report marks that source as unavailable. It does not reinterpret missing evidence as zero failures, zero changes, or successful delivery.
