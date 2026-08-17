# AcmeMux roadmap

The canonical public product direction is
[acmemux.com/roadmap](https://acmemux.com/roadmap/). This GitHub mirror gives
contributors the same horizons and status vocabulary used by the website.

## Product destination

AcmeMux begins with one administrator, one reviewed upstream lego runtime, and
one native workspace. The long-term goal is a self-hosted certificate lifecycle
platform that can discover, issue, renew, deploy, and account for public and
private certificates across an operator's environment.

The destination includes unified inventory, discovery, policy and approvals,
renewal, alerts, constrained deployment, access control, audit evidence,
reporting, backup, and tested recovery. It must remain understandable and
recoverable by the person responsible during an outage.

## Product horizons

| Horizon | Outcome | Representative capabilities |
| --- | --- | --- |
| Foundation | Operate one lego workspace safely | Reviewed runtime, typed native configuration, constrained operations, daily evaluation, health evidence |
| Dependable operation | Trust unattended renewal | Signed packaging, short-lived profiles, alerts, durable history, backup and restore, qualified platforms |
| Connected lifecycle | Find and move certificates | Multiple workspaces, discovery, broader inventory, deployment adapters, APIs, webhooks, templates, policy |
| Lifecycle platform | Run public and private certificate lifecycle in one self-hosted control plane | Issuance, identity, approvals, audit, compliance evidence, resilient recovery, infrastructure integrations |

Horizons are direction, not release promises. A future capability is not called
supported until its architecture, security boundary, qualification evidence,
documentation, and recovery path are complete.

## Priority policy

Security incidents, critical defects, dependency emergencies, and release
integrity work can preempt every feature queue. After that, accepted feature
work is ordered as follows:

1. Features selected by $500-per-month fast-track partners with a 12-month
   commitment, after maintainer acceptance.
2. Accepted community proposals ranked by unique positive reactions in the
   Ideas discussion category.
3. Maintainer-selected work required to advance the product direction.

Funding never bypasses architecture, security, licensing, testing, or review.

## Status vocabulary

- **Proposed:** useful idea that has not been accepted.
- **Researching:** feasibility or security boundaries are being investigated.
- **Planned:** accepted, scoped, and eligible for implementation.
- **In progress:** implementation is actively underway.
- **Shipped:** included in a tagged release.
- **Declined:** intentionally outside the product direction or trust boundary.

## MVP release track

| Item | Status | Notes |
| --- | --- | --- |
| Single-administrator native lego control plane | Shipped in MVP source | One runtime and one workspace |
| Curated CA, HTTP-01, and five-provider DNS-01 configuration | Shipped in MVP source | Exact supported lego artifacts only |
| Manual and durable daily certificate evaluation | Shipped in MVP source | lego remains authoritative for renewal |
| Certificate health and latest redacted result | Shipped in MVP source | No long-term history yet |
| Debian 13 amd64 source-built systemd distribution | Shipped in MVP source | Package repositories remain deferred |
| First public tagged release and release artifacts | In progress | Requires release qualification and a green verification run |

## Near-term candidates

| Candidate | Status | Why it matters |
| --- | --- | --- |
| Let's Encrypt short-lived certificate profile | Proposed | Proves automation-dependent renewal without forcing classic certificates early |
| Native Debian package and signed repository | Proposed | Makes installation and upgrades easier to audit |
| Additional qualified distributions and arm64 | Proposed | Broadens self-hosted deployment choices |
| Renewal failure notifications | Proposed | Makes unattended operation easier to trust |
| Durable operation history | Proposed | Supports incident review beyond the latest result |
| Backup and restore workflow | Proposed | Makes application-state recovery repeatable |

## Later lifecycle candidates

| Candidate | Horizon |
| --- | --- |
| Certificate deployment integrations | Connected lifecycle |
| Broader inventory and certificate discovery | Connected lifecycle |
| Multiple workspaces and execution hosts | Connected lifecycle |
| Lifecycle templates, policy, and approvals | Connected lifecycle |
| Service API, webhooks, and automation identities | Connected lifecycle |
| Multiple users, roles, and enterprise identity | Lifecycle platform |
| Private issuance and enrollment protocols | Lifecycle platform |
| Audit, reporting, compliance evidence, and resilient operation | Lifecycle platform |

## Vote or fund work

Search the [Ideas discussions](https://github.com/acmemux/AcmeMux/discussions/categories/ideas)
before opening a proposal. Add one positive reaction to the proposal's first
post to vote. Comments should provide use cases, constraints, and evidence.

A highly voted idea becomes a priority signal, not an automatic promise. Read
the [sponsorship policy](SPONSORSHIP.md) for funded work. New ideas require
feasibility review before a feature sponsorship is accepted.
