# AYTHER Support Guide

Last updated: August 25, 2026

AYTHER is currently in early development. Public support is community-based and
provided on a best-effort basis. There are no stable releases, guaranteed
response times, or paid support plans at this stage.

This guide explains where to ask for help and what information to provide so
that maintainers and contributors can respond effectively.

## Choose the right place

Open an issue in the repository that owns the affected component:

| Topic | Repository |
| --- | --- |
| AYTHER ecosystem, public scope, or this top-level documentation | [Ayther-Dev/AYTHER](https://github.com/Ayther-Dev/AYTHER/issues) |
| Emulation integration, audiovisual identification, substitution, rendering, or engine APIs | [Ayther-Dev/AYTHER-Engine](https://github.com/Ayther-Dev/AYTHER-Engine/issues) |
| Game-session host, input, overlay, playback, or runtime behavior | [Ayther-Dev/AYTHER-Runtime](https://github.com/Ayther-Dev/AYTHER-Runtime/issues) |
| Launcher, library, navigation, or player-facing experience | [Ayther-Dev/AYTHER-Play](https://github.com/Ayther-Dev/AYTHER-Play/issues) |
| Public interfaces, contracts, pack tooling, examples, or third-party integration | [Ayther-Dev/AYTHER-SDK](https://github.com/Ayther-Dev/AYTHER-SDK/issues) |

If you are unsure, use the top-level
[AYTHER issue tracker](https://github.com/Ayther-Dev/AYTHER/issues) and explain
which component you believe is involved. Maintainers may transfer or redirect
the issue.

An empty or incomplete repository does not represent a supported release.
Repositories are being initialized progressively.

## Before opening an issue

Please:

1. search existing open and closed issues for the same problem;
2. read the relevant repository's README and available documentation;
3. confirm that you are using an official AYTHER repository or release;
4. reproduce the problem with the latest public version when practical;
5. separate AYTHER behavior from failures in an emulator core, driver,
   operating system, game file, or unofficial pack; and
6. remove secrets, personal information, copyrighted commercial game data, and
   other material you do not have permission to share.

Do not create duplicate issues in several repositories. Link related issues
instead.

## Bug reports

A useful bug report includes:

- a concise, descriptive title;
- the affected AYTHER component;
- version, tag, commit SHA, or build date;
- operating system and version;
- CPU architecture and relevant GPU or driver details;
- installation or build method;
- exact steps to reproduce;
- expected and actual behavior;
- whether the issue happens consistently;
- the smallest non-infringing fixture or configuration that reproduces it;
- relevant logs, error messages, screenshots, or stack traces; and
- troubleshooting steps already attempted.

Use fenced code blocks for logs and terminal output. Shorten repetitive output,
but do not omit the first error or the surrounding context. Redact usernames,
paths, tokens, email addresses, keys, and other sensitive values.

When a problem depends on a particular game, do not upload or link to its ROM,
BIOS, music, graphics, or other protected content. Where possible, provide:

- a ROM hash or other non-reconstructive identifier;
- the game's region and revision;
- the emulator core name and version;
- a minimal synthetic or homebrew reproduction;
- non-infringing metadata; and
- the precise point at which the behavior appears.

A hash identifies data for compatibility purposes; it does not establish that
the underlying copy is authorized.

## Build and installation questions

For build failures, also include:

- compiler and linker versions;
- CMake, Rust, package-manager, and SDK versions as applicable;
- the exact command that failed;
- relevant build options and environment details;
- the first meaningful error, not only the final summary;
- whether the build directory was clean; and
- any local patches or dependency overrides.

Support is prioritized for configurations documented by the affected repository.
Maintainers may be unable to investigate unsupported toolchains, obsolete
drivers, heavily modified forks, or incomplete third-party packages.

## Feature requests

Feature requests are welcome during public development, but they are not product
commitments.

Describe:

- the problem or user need;
- who benefits from solving it;
- the proposed behavior;
- an example workflow;
- relevant alternatives or workarounds;
- the affected component; and
- compatibility, performance, security, or legal constraints.

Avoid combining unrelated requests in one issue. A request may be declined,
deferred, split, or moved to a roadmap without implying a delivery date.

Do not request support for obtaining or distributing unauthorized ROMs, BIOS
files, keys, protected assets, or circumvention material.

## Questions and discussions

Use repository issues for actionable bugs, documentation gaps, and concrete
feature proposals. If GitHub Discussions is enabled for the relevant repository
or organization, use it for open-ended questions, ideas, showcases, and general
conversation.

Until an official discussion forum is announced, avoid opening issues solely
for promotion, general emulation debate, or sharing third-party downloads.

English is preferred for public technical issues because it reaches the widest
set of contributors. Spanish reports are also welcome. Maintainers may translate
or normalize issue titles and summaries for discoverability.

## Security vulnerabilities

Do not disclose a suspected vulnerability in a public issue.

Follow [SECURITY.md](SECURITY.md). Use GitHub's private **Report a
vulnerability** feature when it is enabled for the affected repository, or email
[david.lazarte@gmail.com](mailto:david.lazarte@gmail.com) with the subject
**[AYTHER SECURITY] Brief description**.

Security reports sent through the support issue trackers may be closed or have
sensitive content removed to protect users.

## Intellectual property and content concerns

For copyright, trademark, ROM, BIOS, pack-content, provenance, or other
intellectual-property concerns, follow [LEGAL.md](LEGAL.md).

Rights holders or their authorized representatives may contact
[david.lazarte@gmail.com](mailto:david.lazarte@gmail.com). Include the exact
location of the material, the right at issue, your authority to report it, and
enough information to evaluate the concern.

Do not use a technical support issue for a formal legal notice.

## AYTHER trademarks

Questions about the AYTHER name, logos, icons, product names, domain, community
branding, merchandise, sponsorship claims, or permission requests are governed
by [TRADEMARKS.md](TRADEMARKS.md).

Send permission requests to
[david.lazarte@gmail.com](mailto:david.lazarte@gmail.com). Silence or lack of a
response does not constitute authorization.

## What support does not include

AYTHER does not provide support for:

- finding, downloading, sharing, validating the ownership of, or bypassing
  protections on commercial ROMs, BIOS files, firmware, keys, or game assets;
- determining whether a user's copy, backup, modification, pack, or distribution
  is lawful;
- unofficial builds presented as official releases;
- modified forks whose maintainers have not reproduced the issue upstream;
- third-party emulator cores, drivers, operating systems, services, or packs
  when the problem is exclusively in that third-party component;
- recovering lost credentials, private keys, game data, or user files;
- guaranteed platform compatibility before it is documented;
- individualized legal advice;
- private implementation consulting through the public issue tracker; or
- guaranteed response, resolution, release, or roadmap dates.

Compatibility with AYTHER does not mean that a third-party pack, core, tool, or
service is official, reviewed, secure, licensed, or endorsed.

## Community expectations

Everyone requesting or providing support must:

- be respectful and patient;
- provide accurate information;
- avoid harassment, pressure, threats, or repeated unsolicited contact;
- protect other people's privacy and intellectual property;
- follow the applicable code of conduct when published; and
- keep discussion focused on resolving the reported problem.

Maintainers may edit titles, request additional information, apply labels,
transfer issues, lock disruptive conversations, or close reports that are
duplicates, unsupported, inactive, abusive, unsafe, or outside the project's
scope.

## Response and issue lifecycle

AYTHER is maintained by a small project team. Public support is best effort:

- acknowledgment and investigation times vary;
- severity, reproducibility, user impact, and maintainer availability affect
  prioritization;
- asking for an update does not increase priority;
- lack of activity does not mean that a report has been accepted or scheduled;
  and
- closing an issue does not necessarily mean the underlying idea lacks value.

Issues may be marked as needing information and closed if the requested details
are not provided after a reasonable period. A closed issue may be reopened when
new, reproducible information becomes available.

## Commercial support

AYTHER does not currently advertise a public commercial-support offering.
Any future support, sponsorship, partnership, or professional-services program
will be announced through [ayther.dev](https://ayther.dev) or an official
repository. Unsolicited messages or third-party claims do not create an official
AYTHER support relationship.

---

For project news and official repositories, visit
[ayther.dev](https://ayther.dev) and the
[Ayther-Dev GitHub organization](https://github.com/Ayther-Dev).
