# AYTHER Security Policy

Last updated: August 24, 2026

AYTHER takes the security of its users, contributors, tools, and distribution
formats seriously. We appreciate responsible reports that give maintainers a
reasonable opportunity to investigate and address a vulnerability before it is
publicly disclosed.

## Supported versions

AYTHER is currently in early development and has not published a stable,
supported release.

| Version | Supported |
| --- | --- |
| Stable releases | None published yet |
| Latest public pre-release or default branch | Best-effort security fixes |
| Older commits, forks, unofficial builds, and modified distributions | Not supported |

This table will be replaced with an explicit release-support matrix when the
first stable version is published. Development branches may change without
notice and should not be treated as production-ready.

## Reporting a vulnerability

**Do not report security vulnerabilities in a public issue, pull request,
discussion, chat, or social-media post.**

Use one of these private channels:

1. **Preferred:** if the affected repository shows a **Report a vulnerability**
   button under its Security tab, submit a GitHub private vulnerability report
   in that repository.
2. **Fallback:** email
   [david.lazarte@gmail.com](mailto:david.lazarte@gmail.com) with the subject
   **[AYTHER SECURITY] Brief description**.

If a report affects more than one AYTHER repository, submit it against the
component with the greatest impact and list the other affected components.
Do not open duplicate public or private reports for the same vulnerability.

The reporting mailbox does not currently publish a PGP key. Do not send
credentials, private keys, personal data, proprietary ROMs, BIOS files, or other
sensitive third-party content. If sensitive evidence is essential, first send a
minimal description and request a secure exchange method.

## What to include

A useful report should contain:

- the affected AYTHER component and repository;
- the affected commit, tag, package, build, or version;
- operating system, architecture, compiler, and relevant configuration;
- a clear description of the vulnerability and its security impact;
- the preconditions and trust boundary involved;
- reproducible steps or a minimal proof of concept;
- expected and observed behavior;
- logs, stack traces, crash dumps, or sanitizer output with secrets and personal
  information removed;
- whether the issue is already known or publicly disclosed;
- any suggested mitigation or patch; and
- how you would like to be credited, or whether you prefer anonymity.

Please use the smallest safe test artifact possible. Do not attach copyrighted
commercial game data. When a game-specific condition is necessary, provide
non-infringing metadata, hashes, a minimal synthetic fixture, or instructions
that allow maintainers to reproduce the condition using lawfully obtained local
content.

## Security scope

Examples of issues that are in scope include:

- arbitrary code execution or memory corruption;
- unsafe handling of untrusted ROMs, packs, manifests, archives, images, audio,
  scripts, save data, or network responses;
- path traversal, archive extraction outside the intended directory, unsafe
  symbolic-link handling, or arbitrary file overwrite;
- pack-signature, integrity-check, provenance, or trust-verification bypasses;
- sandbox escapes or unexpected host access from pack scripts or Lua;
- command, argument, environment, configuration, or shader injection;
- privilege escalation or unintended access to local files, secrets, or user
  data;
- insecure deserialization, integer overflow, use-after-free, out-of-bounds
  access, or denial of service with realistic impact;
- insecure update, download, installation, or package-verification flows;
- network authentication, authorization, session, or transport-security flaws
  in public AYTHER services when those services become available;
- vulnerabilities crossing the intended boundary between AYTHER, emulator
  cores, enhancement packs, and the host system;
- exposed credentials or private signing material belonging to AYTHER; and
- dependency vulnerabilities that are reachable through an AYTHER component
  and have a concrete security impact.

## Generally out of scope

The following are normally outside the scope of this security process:

- legal, copyright, trademark, ROM, BIOS, or content-authorization disputes;
- vulnerabilities exclusively in an unmodified third-party emulator core,
  library, operating system, driver, or service that AYTHER does not maintain;
- issues affecting only unsupported forks, private modifications, obsolete
  commits, or unofficial packages;
- missing hardening suggestions without a demonstrated security consequence;
- self-inflicted failures that require a user to deliberately modify their own
  installation or disable documented protections;
- denial of service requiring unrealistic resources or no meaningful trust
  boundary;
- social engineering, phishing, physical attacks, or attacks against personal
  accounts unrelated to AYTHER software;
- reports produced solely by automated scanning without validation or a
  reproducible impact;
- version disclosure, banner information, or dependency-version reports without
  evidence that the vulnerable behavior is reachable; and
- requests for compensation, payment, or a bounty.

For intellectual-property or content concerns, follow
[LEGAL.md](LEGAL.md). For misuse of AYTHER names or logos, follow
[TRADEMARKS.md](TRADEMARKS.md).

An issue involving a third-party dependency may still be in scope when AYTHER's
use, configuration, packaging, or failure to update that dependency creates a
specific exploitable condition in an official AYTHER build.

## Research rules

To protect users and preserve eligibility for coordinated handling:

- test only against systems, accounts, data, and content you own or are
  explicitly authorized to use;
- make a good-faith effort to avoid privacy violations, data destruction,
  service disruption, persistence, or impact on other people;
- access only the minimum data necessary to demonstrate the issue;
- stop testing and report promptly if you encounter user data, credentials,
  private keys, or an active compromise;
- do not use a vulnerability to obtain money, services, access, or leverage;
- do not deploy malware, establish persistence, exfiltrate data, or pivot to
  unrelated systems;
- do not publicly disclose exploit details before coordinated disclosure or
  before maintainers have had a reasonable opportunity to respond; and
- comply with applicable law and the rules of any third-party platform involved.

## Response targets

AYTHER is currently maintained by a small project team. The following are
targets, not guaranteed service-level commitments:

| Stage | Target |
| --- | --- |
| Acknowledgment | Within 5 business days |
| Initial assessment | Within 10 business days |
| Status updates for accepted reports | At least every 14 days when practical |
| Fix and disclosure | Based on severity, complexity, and release readiness |

Maintainers may ask for additional information, accept the report for private
investigation, mark it as a duplicate, redirect it to an upstream project, or
close it as not applicable. Acknowledgment does not mean that a vulnerability
has been confirmed.

If you do not receive an acknowledgment within 7 business days, send one
follow-up email referencing the original report. Please do not create a public
issue merely to request status.

## Coordinated disclosure

When a vulnerability is confirmed, maintainers will aim to:

1. assess severity, affected components, and supported versions;
2. develop and test a correction or mitigation privately;
3. coordinate a reasonable disclosure date with the reporter;
4. publish fixed versions when feasible;
5. publish a security advisory describing impact, affected versions, and
   remediation; and
6. request or reference a CVE when appropriate.

Disclosure timing depends on user risk, active exploitation, fix availability,
upstream coordination, and third-party dependencies. AYTHER may disclose earlier
when necessary to protect users, when details are already public, or when active
exploitation is observed.

Do not publish a proof of concept, exploit, or detailed reproduction steps until
the advisory is public or a disclosure date has been agreed. Once an advisory is
published, researchers may discuss their work while continuing to protect
private data and third-party rights.

## Credit and bounty policy

AYTHER will make a reasonable effort to credit reporters who request recognition
and whose reports lead to a confirmed security fix. Reporters may also request
anonymity.

AYTHER does not currently operate a paid bug-bounty program and cannot promise
payment, merchandise, employment, or any other reward. Do not begin testing on
the assumption that compensation will be offered.

## Good-faith research and safe harbor

When security research is conducted in good faith, follows this policy, avoids
harm, and is reported promptly, AYTHER will not initiate legal action against
the researcher for that research on AYTHER-owned systems or software.

If a third party initiates legal action and the researcher has complied with
this policy, AYTHER may, at its discretion and where appropriate, clarify that
the research was conducted under this policy.

This safe-harbor statement:

- applies only to rights controlled by David Lazarte or the AYTHER project;
- does not authorize access to third-party systems, accounts, games, ROMs,
  services, infrastructure, or intellectual property;
- does not waive obligations under open-source licenses or applicable law;
- does not cover extortion, threats, intentional harm, data theft, privacy
  violations, or public disclosure contrary to this policy; and
- is not a promise to defend or indemnify a researcher against third-party
  claims.

If you are uncertain whether planned testing is covered, contact
[david.lazarte@gmail.com](mailto:david.lazarte@gmail.com) before proceeding.

## Security updates

Security fixes and advisories will be published through the affected
repository's Releases and Security sections when those channels become
available. Users should obtain releases only from official AYTHER repositories
or [ayther.dev](https://ayther.dev), verify published signatures or checksums
when provided, and avoid unofficial binaries presented as official releases.
