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

- The current published release is [0.7.1](https://github.com/Vericairn/vericairn/releases/tag/v0.7.1), published
  on October 17, 2026: self-contained archives of the command line and of Workbench for Linux, macOS and Windows,
  on x64 and arm64, with `SHA256SUMS`, a software bill of materials, the third-party notices and its
  documentation set.
- Its [install guide](https://github.com/Vericairn/vericairn/blob/v0.7.1/docs/releases/0.7.1/install.md) covers
  Linux, macOS and Windows, checking a download, Workbench, the MCP server and NuGet installation.
- The [documentation sets](https://github.com/Vericairn/vericairn/blob/main/docs/releases/README.md) of the
  releases from 0.2.0 on are kept in the repository.

0.7.0 was withdrawn before publication. 0.7.1 carries that candidate's features with FIX-12's corrections,
as described in its [documentation set](https://github.com/Vericairn/vericairn/blob/v0.7.1/docs/releases/0.7.1/README.md).

The command-line tool and SDK packages at 0.7.1 are also available on nuget.org. With the .NET 10 SDK:

```sh
dotnet tool install --global dotnet-vc --version 0.7.1
dotnet vc version
```

In a .NET 10 project, `dotnet add package Vericairn --version 0.7.1` adds the SDK front door and its client,
protocol and record dependencies. The NuGet tool is framework-dependent and includes neither Workbench nor
the macOS Secure Enclave helper; use the archives for those components.

## Status

Released, in the Community edition:

- **The command line**, `vericairn`, for people and scripts. It includes `vericairn mcp serve`, a Model Context
  Protocol server through which coding agents work in an estate; no agent harness has been qualified with it.
- **The daemon**, which owns an estate's live state and serves it to clients on the same machine.
- **The SDK**, the typed .NET client of the daemon's API.
- **Workbench**, the desktop application, a client of the daemon.

0.7.1 adds hand-over and resume from retained records, observations of agent runs, personal communication
settings and delegation, measured context packages with pinned source retrieval, and explicit model, effort
and environment admission for each run. Workbench adds local communication settings and hand-over/resume
views. Context tokens remain unknown without a qualified local tokenizer; the efficiency Adapter is planned.

Community retains goals and independent evaluations, roster routing and asks, progress reporting, coding-agent
launchers and local-network pairing. It dispatches one goal step at a time; multi-step planning and scheduling
remain planned Pro work. The launchers are tested with stand-in processes, with no qualified live coding-agent
session. Native runs require machine-local configuration and an admitted exact harness version; generic dispatch
is refused. Saved paired connections are used through the SDK, with no paired-runtime chooser in Workbench.

Remote, the mobile companion, is not implemented or released.

In 0.7.1 the command line is qualified on linux-x64, osx-arm64 and win-x64, where the release's tests ran; its
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
