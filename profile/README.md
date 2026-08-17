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

The project is at MVP stage. The first qualified deployment target is a
source-built systemd service on Debian 13 amd64. The source repository is being
prepared for its first public tagged release.

- [Product website and technical guides](https://acmemux.com)
- [Live dogfood certificate status](https://acmemux.com/certificate-status/)
- [Product vision and roadmap](https://acmemux.com/roadmap/)
- [GitHub roadmap mirror](https://github.com/acmemux/.github/blob/main/ROADMAP.md)
- [Contributing guide](https://github.com/acmemux/.github/blob/main/CONTRIBUTING.md)
- [Roadmap ideas and voting](https://github.com/acmemux/.github/discussions/categories/ideas)
- [Sponsorship policy](https://acmemux.com/sponsor/)

## Built in public, operated on itself

The production website uses an internal AcmeMux instance, upstream lego,
Let's Encrypt DNS-01, and a narrowly scoped Route 53 identity to evaluate,
issue, and deploy its own TLS certificate. Its deliberately accelerated
dogfood setting targets a visible replacement about every 72 to 96 hours while
leaving margin below Let's Encrypt's exact-set rate limit. The live website
publishes the certificate dates, fingerprint, and expected next replacement.

## How work is prioritized

Urgent security and release-integrity work always comes first. For accepted
feature work, the order is:

1. written sponsor-funded commitments;
2. accepted roadmap items ranked by community votes; and
3. maintainer-selected work.

Money does not buy a security exception, an unreviewed merge, or control of the
project. A feature sponsorship guarantees priority only after feasibility,
scope, acceptance criteria, and funding are agreed in writing.
