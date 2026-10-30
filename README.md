# Kimetsu

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Kimetsu (kimetsu.dev) is Rodrigo Córdoba's open-source infrastructure for coding agents. Kimetsu itself is a local, model-free memory sidecar — one Rust binary and one SQLite brain per project — that Claude Code, Codex, Cursor, Pi and OpenClaw load as a local-stdio MCP server (~28 kimetsu_* tools), with a CLI, npm/cargo/PyPI packages, a self-hostable Kimetsu Remote HTTP MCP server and published benchmark numbers. The domain also operates agents.kimetsu.dev, a credential-free, read-only Agent Gateway with a published OpenAPI 3.1.0 (15 operations), an A2A Agent Card served at the RFC 8615 path (0.3 by default, 1.0 negotiated with the A2A-Version header) and a live JSON-RPC guide for Sidequest Commons — the maintainer's daily public project-selection loop run through GitHub issues and reactions — plus llms.txt on two hosts, a /.well-known/kimetsu-agents.json discovery pointer and JSON Schemas for its discovery documents. Everything is MIT OR Apache-2.0. Seeded from the A2A Registry listing dev.kimetsu.sidequest_commons_guide under the harvest name "Sidequest Commons".

**Areas:** Company · AI Agents · Agent Memory · Coding Agents · MCP · A2A · Developer Tools · Open Source · Rust · Agent Discovery · Public Goods

## Kimetsu on APIs.io

Everything profiled for Kimetsu is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/kimetsu-dev/](https://apis.io/providers/kimetsu-dev/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [Sidequest Commons Guide (A2A)](https://apis.io/apis/kimetsu-dev/sidequest-commons-guide/) — A2A agent (JSON-RPC; 0.3 message/send by default, 1.0 SendMessage with A2A-Version 1.0) that returns deterministic, credential-free guidance on discovering…
- [Kimetsu MCP Server (local stdio)](https://apis.io/apis/kimetsu-dev/kimetsu-mcp-server/) — The memory product's agent surface: `kimetsu mcp serve` exposes ~28 kimetsu_* tools (context retrieval, lesson recording, memory CRUD and curation,…
- [Kimetsu A2A API](https://apis.io/apis/kimetsu-dev/kimetsu-dev-a2a-api/) — Deterministic guidance; no delegated actions or writes.
- [Kimetsu Discovery API](https://apis.io/apis/kimetsu-dev/kimetsu-dev-discovery-api/) — Static, anonymous machine-discovery documents.
- [Kimetsu Sidequest API](https://apis.io/apis/kimetsu-dev/kimetsu-dev-sidequest-api/) — Read-only Sidequest Commons public data.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (1)

Multi-step workflows that chain operations into a business task.

- [Discover Sidequest Commons and ask the A2A guide](https://apis.io/arazzos/kimetsu-dev/kimetsu-dev-discover-and-ask-workflow/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [kimetsu](https://apis.io/servers/kimetsu-dev/kimetsu/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Kimetsu Dev Agentic Access](https://apis.io/agentic-access/kimetsu-dev/kimetsu-dev-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [kimetsu.dev agent directory](https://apis.io/schemas/kimetsu-dev/kimetsu-dev-agent-directory-v1.schema/)
- [Sidequest Commons machine proposal](https://apis.io/schemas/kimetsu-dev/kimetsu-dev-sidequest-proposal-v1.schema/)
- [kimetsu.dev well-known agent directory pointer](https://apis.io/schemas/kimetsu-dev/kimetsu-dev-well-known-agent-directory-v1.schema/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Kimetsu Dev Agent Gateway Overlay](https://apis.io/overlays/kimetsu-dev/kimetsu-dev-agent-gateway-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Kimetsu Dev Authentication](https://apis.io/security/kimetsu-dev/kimetsu-dev-authentication/)
- [Kimetsu Dev Domain Security](https://apis.io/security/kimetsu-dev/kimetsu-dev-domain-security/)
- [Kimetsu Dev Vulnerability Disclosure](https://apis.io/security/kimetsu-dev/kimetsu-dev-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Kimetsu Dev Plans Pricing](https://apis.io/plans/kimetsu-dev/kimetsu-dev-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Kimetsu Dev Rate Limits](https://apis.io/rate-limits/kimetsu-dev/kimetsu-dev-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://kimetsu.dev/)
- [Documentation](https://kimetsu.dev/docs/)
- [Getting started](https://kimetsu.dev/docs/install/)
- [API reference](https://agents.kimetsu.dev/openapi.json)
- [Support](https://github.com/RodCor/kimetsu/issues)
- [Changelog](https://kimetsu.dev/docs/changelog/)
- [Security](https://github.com/RodCor/kimetsu.dev/blob/main/SECURITY.md)
- [GitHub](https://github.com/RodCor)

## API Evangelist rating

**Kin Score 44.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 63.3 |
| Contract quality | 48.4 |
| Contract governance | 18.2 |
| Operational transparency | 63.2 |
| Developer ergonomics | 76.2 |
| Access clarity | 0.0 |

**Agent readiness 34.7** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | conformant |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 22.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/kimetsu-dev/](https://apis.io/providers/kimetsu-dev/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Kimetsu: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/kimetsu-dev/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
