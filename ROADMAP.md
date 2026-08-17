# AcmeMux roadmap

AcmeMux is an MVP maintained by one owner. This roadmap is a demand signal and
planning tool, not a promise that every proposed feature will ship.

## Priority policy

Security incidents, critical defects, dependency emergencies, and release
integrity work can preempt every feature queue. After that, accepted feature
work is ordered as follows:

1. Sponsor-funded commitments with written scope and acceptance criteria.
2. Accepted community proposals ranked by unique positive reactions in the
   Ideas discussion category.
3. Maintainer-selected work based on product direction, dependencies, and
   available time.

Funding never bypasses architecture, security, licensing, testing, or review.
An arbitrary request cannot purchase an automatic merge. A funded feature is
accepted only after a feasibility review; once accepted and funded, it is put
at the front of the feature queue. Any delivery date or refund terms belong in
the written sponsorship agreement.

## Status vocabulary

- **Proposed:** useful idea that has not been accepted.
- **Researching:** feasibility or security boundaries are being investigated.
- **Planned:** accepted, scoped, and eligible for implementation.
- **In progress:** implementation is actively underway.
- **Shipped:** included in a tagged release.
- **Declined:** intentionally outside the product boundary.

## MVP release track

| Item | Status | Notes |
| --- | --- | --- |
| Single-administrator native lego control plane | Shipped in MVP source | One runtime and one workspace |
| Curated CA, HTTP-01, and five-provider DNS-01 configuration | Shipped in MVP source | Exact supported lego artifacts only |
| Manual and durable daily certificate evaluation | Shipped in MVP source | lego remains authoritative for renewal |
| Certificate health and latest redacted result | Shipped in MVP source | No long-term history |
| Debian 13 amd64 source-built systemd distribution | Shipped in MVP source | Package repositories remain deferred |
| First public tagged release and release artifacts | In progress | Requires release qualification and a green verification run |

## Candidate roadmap

These candidates are not yet support commitments:

| Candidate | Status | Why it matters |
| --- | --- | --- |
| Let's Encrypt short-lived certificate profile | Proposed | Demonstrates high-frequency, automation-dependent renewal without forcing classic certificates early |
| Native Debian package and signed repository | Proposed | Removes source compilation and makes upgrades easier to audit |
| Additional qualified distributions and arm64 | Proposed | Broadens self-hosted deployment choices |
| Renewal failure notifications | Proposed | Makes unattended operation easier to trust |
| Long-term operation audit history | Proposed | Supports incident review beyond the latest result |
| Backup and restore workflow | Proposed | Makes application-state recovery repeatable |
| Certificate deployment integrations | Proposed | Connects issued material to serving systems through constrained adapters |
| Additional DNS providers and ACME profiles | Proposed | Extends curated coverage without equating compiled support with qualified support |
| Multiple workspaces | Proposed | Supports operators with separate trust and credential boundaries |
| Multiple users, roles, and enterprise identity | Proposed | Enables team operations and delegated access |
| Remote runners or hosted service | Proposed | Separates the control plane from certificate execution hosts |

## Vote on a feature

Search the [Ideas discussions](https://github.com/acmemux/.github/discussions/categories/ideas)
before opening a proposal. Add one positive reaction to the proposal's first
post to vote. Comments are for use cases, constraints, and implementation
evidence; duplicate comments are not extra votes.

A highly voted idea becomes the highest-ranked community candidate, not an
automatic promise. The maintainer still confirms fit, security, and dependency
order before changing its status to Planned.

## Fund a roadmap item

Read the [sponsorship policy](SPONSORSHIP.md). Funding an already accepted item
is the fastest path to priority. New ideas require feasibility review before a
feature sponsorship is accepted.
