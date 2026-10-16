# Vericairn

Vericairn is a local-first creation and operations platform. It helps a person or an organization turn an
intention into an understood, authorized, produced, reviewed, delivered and maintained result, with its
decisions, sources, relationships and history intact.

Work in Vericairn lives in an estate: the continuing body of work behind a venture, held as append-only records of
its decisions, work, reviews, acceptances and releases. Vericairn renders the estate's current state from those
records and refuses a record that would make the estate invalid. Agents propose and produce; milestones and
releases are accepted by a person, from the recorded evidence.

Vericairn is built, released and maintained in its own estate, by one person working with coding agents.

## Editions

- **Community** is the free foundation, under the Apache License 2.0, commercial use included. Everything released
  so far is Community.
- **Standard** is reserved for an optional offering on the same core. What it adds is not yet chosen, and nothing
  is sold under it.
- **Pro** is planned for coordination programs that operate goals across work orders. Its repository is public
  for review under the PolyForm Noncommercial License 1.0.0, and it never becomes open source.
  Commercial use needs a license, and none is offered yet. Nothing has been released from it.

## Repositories

- [vericairn](https://github.com/Vericairn/vericairn): the Community edition under Apache-2.0, with the record
  format, the runtime and its daemon, the command line, the SDK, Workbench and the releases' documentation sets.
- [vericairn-pro](https://github.com/Vericairn/vericairn-pro): the repository for the planned Pro edition, published
  for review under the PolyForm Noncommercial License 1.0.0. It is not open source and takes no outside contributions.
- [.github](https://github.com/Vericairn/.github): this profile, and the default community files for every
  Vericairn repository that has none of its own.

## Get it

Vericairn is published on [GitHub Releases](https://github.com/Vericairn/vericairn/releases) as unsigned developer
builds. Nothing is code-signed or notarized yet, so verify every download against its checksum.

- The current published release is [0.6.1](https://github.com/Vericairn/vericairn/releases/tag/v0.6.1), published
  on October 16, 2026: self-contained archives of the command line and of Workbench for Linux, macOS and Windows,
  on x64 and arm64, with `SHA256SUMS`, a software bill of materials, the third-party notices and its
  documentation set.
- Its [install guide](https://github.com/Vericairn/vericairn/blob/v0.6.1/docs/releases/0.6.1/install.md) covers
  Linux, macOS and Windows, checking a download, Workbench and the MCP server.
- The [documentation sets](https://github.com/Vericairn/vericairn/blob/main/docs/releases/README.md) of the
  releases from 0.2.0 on are kept in the repository.

0.6.0 was withdrawn before publication. 0.6.1 carries that candidate's features with the corrections described
in its [documentation set](https://github.com/Vericairn/vericairn/blob/v0.6.1/docs/releases/0.6.1/README.md).

## Status

Released, in the Community edition:

- **The command line**, `vericairn`, for people and scripts. It includes `vericairn mcp serve`, a Model Context
  Protocol server through which coding agents work in an estate; no agent harness has been qualified with it.
- **The daemon**, which owns an estate's live state and serves it to clients on the same machine.
- **The SDK**, the typed .NET client of the daemon's API.
- **Workbench**, the desktop application, a client of the daemon.

0.6.1 adds Community goals and independent evaluations, roster routing and asks, a progress report, coding-agent
launchers and pairing with a runtime over the local network. Community dispatches one goal step at a time;
multi-step planning and scheduling remain planned Pro work. The launchers are tested with stand-in processes,
not qualified live coding-agent sessions. Workbench shows goals, asks and progress; saved paired connections
are used through the SDK, with no paired-runtime chooser in Workbench.

Remote, the mobile companion, is not implemented or released.

In 0.6.1 the command line is qualified on linux-x64, osx-arm64 and win-x64, where the release's tests ran; its
linux-arm64, osx-x64 and win-arm64 builds are provided but have not been run. Workbench is not qualified on any
platform. The release's documentation set lists its known limitations.

## Security

Report a vulnerability privately, never in a public issue: on the affected repository's **Security** tab, choose
**Report a vulnerability**, or email vericairn@jasonfurr.com. No response time is promised. The
[security policy](https://github.com/Vericairn/.github/blob/main/SECURITY.md) has the details.

## Help

Help is self-service. Start with the documentation set of the release you run: installation, the operator's
guide, the references and the known limitations. Bugs and feature requests go in the issues of the repository
concerned. Vericairn has no support commitment yet, so no response time is promised. Issues are welcome; outside
pull requests are not accepted yet (see [contributing](https://github.com/Vericairn/.github/blob/main/CONTRIBUTING.md)).

## Contact

vericairn@jasonfurr.com

## Sponsor

Vericairn is built by one person working with coding agents. If it is useful to you, you can
[sponsor Jason Furr on GitHub](https://github.com/sponsors/Jayson-Furr). Sponsorship supports the work and the AI usage
it takes; it includes no support, priority, features or license.
