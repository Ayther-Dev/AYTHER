# AYTHER

**Real-time audiovisual remastering for retro games.**

[Website](https://ayther.dev) · [GitHub organization](https://github.com/Ayther-Dev)

> **Project status: early development.** AYTHER is not yet available as a stable
> end-user release. Public APIs, formats, compatibility, and repository contents
> may change while the first public version is being prepared.

AYTHER is a technology ecosystem for enhancing the audiovisual presentation of
retro games in real time. It preserves the original game's logic while allowing
compatible high-definition graphics, audio, effects, and presentation layers to
be applied during playback.

AYTHER does not modify the original game or embed it into a remaster package. The
game and the optional enhancement pack remain separate.

## Why AYTHER?

Traditional remasters often require rebuilding a game, modifying its executable,
or patching its original data. AYTHER takes a different approach: it observes the
game as it runs, identifies supported audiovisual elements, and renders compatible
enhancements without changing the original game logic.

This approach is designed to make remastering:

- **Non-destructive** — the original game remains unchanged.
- **Reversible** — enhanced and original presentation can coexist.
- **Content-independent** — the engine and enhancement packs are distributed
  separately from games.
- **Open to tooling** — public components, formats, and interfaces are being
  prepared for third-party integrations.

## How it works

```text
User-provided game
        │
        ▼
Emulation and game logic
        │
        ▼
Real-time audiovisual identification
        │
        ├── no compatible enhancement ──► original presentation
        │
        └── compatible enhancement ─────► enhanced presentation
```

The current development focus is **Sega Genesis / Mega Drive**. Support for any
additional platform will be announced only after its technical and legal scope has
been properly evaluated.

## Public ecosystem

This repository is the public entry point for the AYTHER ecosystem. Source code,
technical documentation, and releases belong in their corresponding repositories.

| Project | Purpose | Status |
| --- | --- | --- |
| [AYTHER Engine](https://github.com/Ayther-Dev/AYTHER-Engine) | Core emulation, audiovisual identification, substitution, and rendering technology | Early development |
| [AYTHER Runtime](https://github.com/Ayther-Dev/AYTHER-Runtime) | Session host used to run games with compatible enhancements | Early development |
| [AYTHER Play](https://github.com/Ayther-Dev/AYTHER-Play) | Player-facing launcher and library experience | Early development |
| [AYTHER SDK](https://github.com/Ayther-Dev/AYTHER-SDK) | Public interfaces, contracts, tools, and integration examples | Developer preview |

The repositories are being initialized progressively. An empty or incomplete
repository should not be interpreted as a published release.

## Core principles

### Bring Your Own ROM

AYTHER does not provide, host, or distribute commercial game ROMs. Users are
responsible for obtaining and using game content in accordance with the laws and
licenses applicable to them.

### Separate enhancement packs

Enhancement packs are independent from the original games. They must not contain
ROMs, BIOS files, unauthorized game assets, credentials, or other material that
their authors do not have permission to distribute.

### Public, interoperable foundations

AYTHER's public components are intended to provide documented interfaces and
formats that can be inspected, implemented, and integrated by the community under
their applicable licenses.

### Respect for creators and rights holders

Contributors are expected to publish only code, documentation, and assets they
have the right to share. AYTHER is a technological project and does not grant
rights over third-party games, trademarks, characters, artwork, music, or other
protected content.

## Documentation

Public documentation will be added progressively as each component reaches a
usable stage. It will cover:

- ecosystem architecture and component boundaries;
- building and running the public components;
- public APIs and integration contracts;
- the enhancement-pack format and validation rules;
- authoring workflows using public tools;
- compatibility, versioning, and migration policies.

Technical claims should be considered stable only when documented in the relevant
component repository and supported by a public release.

## Contributing

AYTHER is preparing its public contribution workflow. Contribution guidelines,
development requirements, issue templates, and the code of conduct will be
published before general contributions are accepted.

In the meantime, you can follow the repositories in the
[Ayther-Dev organization](https://github.com/Ayther-Dev) to track their public
development.

## Security

Please do not disclose suspected security vulnerabilities in public issues.
Private reporting instructions will be published in `SECURITY.md` before the first
public release.

## Licensing

The public AYTHER components are intended to be released under FOSS licenses.
The license applicable to each repository will be stated in its own `LICENSE`
file. Until that file is present, no open-source license should be assumed.

The AYTHER name, logo, and visual identity are not automatically licensed for use
under the software licenses. A separate trademark policy will define their
permitted uses.

## Disclaimer

AYTHER is an independent project. It is not affiliated with, authorized by,
endorsed by, or sponsored by Sega or any other video game publisher, console
manufacturer, or rights holder. All third-party names and trademarks belong to
their respective owners.

---

**AYTHER** · [ayther.dev](https://ayther.dev)
