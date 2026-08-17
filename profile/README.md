# AcmeMux

AcmeMux starts as a security-focused graphical control plane for an existing
[lego](https://go-acme.github.io/lego/) ACME client and its native workspace.
It helps self-hosted operators review configuration, run constrained
certificate operations, schedule renewal evaluation, and understand certificate
health without replacing lego or creating a second private-key store.

The destination is broader: a self-hosted certificate lifecycle platform that
can discover, issue, renew, deploy, and account for public and private
certificates across an operator's environment. The narrow MVP is the trusted
foundation for inventory, policy, alerts, integrations, identity, audit, and
recovery rather than the end of the product.

AcmeMux is pre-release. The current qualified deployment target is a
source-built systemd service on Debian 13 amd64. Source is public, but no tagged
release exists yet. AcmeMux does not currently claim signed provenance.

- [Product website and technical guides](https://acmemux.com)
- [Product source and issue tracker](https://github.com/acmemux/AcmeMux)
- [Live dogfood certificate status](https://acmemux.com/certificate-status/)
- [Product vision and roadmap](https://acmemux.com/roadmap/)
- [Contributing guide](https://github.com/acmemux/.github/blob/main/CONTRIBUTING.md)
- [Roadmap ideas and voting](https://github.com/acmemux/AcmeMux/discussions/categories/ideas)
- [Sponsorship policy](https://acmemux.com/sponsor/)

## Built in public, operated on itself

The production website uses an internal AcmeMux instance, upstream lego,
Let's Encrypt DNS-01, and a narrowly scoped Route 53 identity. AcmeMux schedules
and evaluates the native workspace, upstream lego performs ACME issuance, and
separate least-privilege automation validates and activates the certificate
served by the website. Its deliberately accelerated dogfood setting targets a
visible replacement about every 72 to 96 hours while leaving margin below
Let's Encrypt's exact-set rate limit. The live website publishes the
certificate dates, fingerprint, and expected next replacement.

## How work is prioritized

Urgent security and release-integrity work comes first. Other accepted work is
selected by the maintainer using operator value, community evidence, security,
scope, and verifiability. Sponsorship supports maintenance and qualified
roadmap work; it does not provide an SLA, private support, implementation
priority, guaranteed delivery, or an exception from review.
