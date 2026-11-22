# Security Policy

This is the organization-wide security policy for the
[NeoNephos Foundation](https://neonephos.org) `neonephos` GitHub organization.
GitHub applies it to every repository in this organization that does not ship
its own `SECURITY.md`. A repository that needs its own intake channel or its
own contacts overrides this file by committing a `SECURITY.md` of its own, as
required by the
[NeoNephos Security Guidelines §5.2](https://github.com/neonephos/guidelines-development/blob/main/security-guidelines/security-guidelines.md#52-securitymd).

## Reporting a Vulnerability

If you discover a security vulnerability in a repository of this organization,
please report it responsibly through one of the channels below.
**Do not open a public issue for security vulnerabilities.**

### What to Include in Your Report

To help us assess and address the vulnerability efficiently, please include:

- **Affected repository** and component(s), with version or commit
- **Steps to reproduce** the vulnerability
- **Impact assessment** — what an attacker could achieve
- Whether the vulnerability is **already publicly known**
- Any suggested fix or mitigation (optional)

### GitHub Private Vulnerability Reporting (preferred)

Please use GitHub's built-in private vulnerability reporting on the affected
repository:

1. Open the repository the vulnerability affects on GitHub.
2. Navigate to its **Security** tab.
3. Click **Report a vulnerability**.
4. Fill in the details and submit.

The report is visible only to the designated security contacts and is never
public.

*For more information, see [Privately reporting a security vulnerability](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability).*

### Fallback Contact

Reporters without a GitHub account, and reporters who cannot reach the
Security tab of the affected repository, may report vulnerabilities by email
to the NeoNephos Technical Advisory Council at
**[tac@lists.neonephos.org](mailto:tac@lists.neonephos.org)**. This is a
private list; do not include vulnerability details in any public channel.

## Security Contacts

The following teams are responsible for handling vulnerability reports for
repositories that rely on this organization-wide policy:

| Name | Handle | Role |
|------|--------|------|
| NeoNephos Technical Advisory Council | [@neonephos/tac](https://github.com/orgs/neonephos/teams/tac) · [tac@lists.neonephos.org](mailto:tac@lists.neonephos.org) | Lead Security Contact |
| NeoNephos Account Administration | [@neonephos/account-administrators](https://github.com/orgs/neonephos/teams/account-administrators) | Security Contact |

Hosted NeoNephos projects designate their own security contacts in their own
`SECURITY.md`, per
[Security Guidelines §5 and §6](https://github.com/neonephos/guidelines-development/blob/main/security-guidelines/security-guidelines.md#5-security-contact-per-project).

## Supported Versions

The repositories in this organization hold foundation governance, community,
documentation and website content, and they are not released as versioned
artifacts. **Only the latest state of the default branch receives security
updates**; older commits, tags and forks are not supported. Where a repository
does publish releases, it states its own version support policy in its own
`SECURITY.md`, which then takes precedence over this file.

## Response Process

This organization follows the
[NeoNephos Security Guidelines](https://github.com/neonephos/guidelines-development/blob/main/security-guidelines/security-guidelines.md)
for vulnerability handling. In summary:

- **Initial response**: We will respond to your report within **14 calendar
  days** of receipt, in line with the
  [OpenSSF Best Practices](https://www.bestpractices.dev/) requirement.
- **Embargo**: Vulnerability details will remain confidential for up to **90
  days** from report receipt while a fix is developed, consistent with the
  [Google Project Zero disclosure policy](https://googleprojectzero.blogspot.com/2021/04/policy-and-disclosure-2021-edition.html).
- **Disclosure**: Once a fix is available (or the embargo expires), we will
  publish a security advisory with full details.

### Severity Response Targets

| Severity | CVSS Score | Fix Target | Disclosure Target |
|----------|------------|------------|-------------------|
| Critical | 9.0 – 10.0 | ≤ 14 days | ≤ 30 days         |
| High | 7.0 – 8.9 | ≤ 30 days     | ≤ 60 days         |
| Medium | 4.0 – 6.9 | ≤ 90 days   | ≤ 90 days         |
| Low | 0.1 – 3.9 | Best effort    | Best effort       |

*These are **SHOULD**-level targets as defined by the
[NeoNephos Security Guidelines](https://github.com/neonephos/guidelines-development/blob/main/security-guidelines/security-guidelines.md#7-severity-classification-and-response-targets).
The 90-day embargo ceiling is a **MUST** aligned with Google Project Zero. All
timelines are measured from report receipt (Day 0); fix and disclosure may
occur simultaneously.*

## Disclosure Policy

We follow
[coordinated disclosure](https://en.wikipedia.org/wiki/Coordinated_vulnerability_disclosure).
We ask that you:

- Allow us reasonable time to investigate and address the vulnerability before
  public disclosure.
- Do not exploit the vulnerability beyond what is necessary to demonstrate the
  issue.
- Do not access or modify data belonging to other users.

We are committed to crediting reporters in our security advisories unless you
prefer to remain anonymous.

## CRA Stewardship

CRA stewardship: the repositories covered by this policy are supported under
the Linux Foundation CRA stewardship framework, as described at
https://www.linuxfoundation.org/security. Security vulnerabilities should be
reported through the mechanisms described above, which we will coordinate with
our CRA steward. For actively exploited vulnerabilities and severe incidents
that may require CRA escalation, the TAC notifies the steward within 24 hours
of becoming aware, in line with
[Security Guidelines §11](https://github.com/neonephos/guidelines-development/blob/main/security-guidelines/security-guidelines.md#11-eu-cyber-resilience-act-cra-compliance).

**CRA Steward Contact**: `steward@linuxfoundation.org`

**Commercial intent**: the content of the repositories covered by this
organization-wide policy is **not intended for commercial** distribution. These
repositories carry foundation governance documents, community material,
guidelines, artwork and website sources; they are not products placed on the
EU market, so the CRA obligations that apply to manufacturers do not apply to
them. Hosted NeoNephos projects that do publish software state their own
commercial-intent determination in their own `SECURITY.md`, and that
determination is revisited with the TAC before a repository's first public
release.
