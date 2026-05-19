# Security Policy

## Reporting

Report vulnerabilities **privately**, by email, to **scalcerano@gmail.com**.
Do not open a public issue for a security problem. We will acknowledge receipt
and keep you informed; please allow a reasonable window before any public
disclosure.

## What counts as a vulnerability at day zero

ANTS has no running network yet. Today the attack surface is the
*specification*. A "vulnerability" is therefore primarily a soundness break in
the protocol design — most critically in the load-bearing layers:

- **RFC-0002 (Verification)** — a way to defeat the verification statistics or
  the challenge cryptography (e.g., an attributable-fault forgery, a way to
  evade the sequential test, a break in the commit/challenge binding).
- **RFC-0004 (Identity)** — a cheaper-than-stated Sybil or genesis-bootstrap
  attack, or a way to make the credible-fork-threat non-credible.
- **RFC-0003 (Reputation)** — a consensus-free-layer break, eclipse beyond the
  stated bound, or tenure forgery the trilemma does not cover.

A clean argument that one of the RFCs' stated guarantees does not hold is a
security report, and we would rather receive it privately first.

When code and a reference node exist, this policy will be extended with
supported-versions and disclosure-timeline detail.
