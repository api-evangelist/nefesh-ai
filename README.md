# Nefesh AI

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

Nefesh AI (nefesh.ai) sells a B2B "human state" middleware API for AI agents: POST live biometric signals from any device — heart rate and HRV from a chest strap, webcam rPPG, voice tone, facial expression, text sentiment, plus accepted-but-not-yet-fused glucose, EEG, electrodermal, respiratory, movement and sleep fields — to one endpoint (api.nefesh.ai/v1/ingest) and get back a unified stress score (0-100) mapped to five states with a machine-readable suggested_action and a closed-loop adaptation_effectiveness signal. The same capability is exposed four ways: a REST API with webhooks and a device registry, a hosted Streamable-HTTP MCP server (6 tools, two of them keyless self-provisioning) listed on the official MCP Registry, an A2A agent (4 skills) discovered from a card on mcp.nefesh.ai, and a "Cognitive Compute Router" LLM gateway that rewrites system prompt and temperature from the live state for OpenAI- and Anthropic-shaped clients. It also maintains the open Human State Protocol (HSP 1.0) JSON Schema and an official npm CLI. Positioned as a General Wellness product, not a medical device. No OpenAPI is published for any surface.

**Areas:** Company · Biometrics · Human State · Stress Detection · Emotion AI · AI Agents · MCP · A2A · LLM Gateway · Wearables · Digital Health · Middleware

## Nefesh AI on APIs.io

Everything profiled for Nefesh AI is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/nefesh-ai/](https://apis.io/providers/nefesh-ai/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Nefesh Human State API](https://apis.io/apis/nefesh-ai/nefesh-human-state-api/) — REST API on api.nefesh.ai (FastAPI): POST /v1/ingest takes a session_id, an ISO 8601 timestamp and at least one of 35+ signal fields and returns the fused…
- [Nefesh Cognitive Compute Router](https://apis.io/apis/nefesh-ai/nefesh-cognitive-compute-router/) — LLM gateway on gateway.nefesh.ai that injects the caller's live human state into the request and adjusts temperature before forwarding to an upstream model.…
- [Nefesh MCP Server](https://apis.io/apis/nefesh-ai/nefesh-mcp-server/) — Hosted remote MCP server at https://mcp.nefesh.ai/mcp (Streamable HTTP, protocol 2025-06-18, session-id based; serverInfo nefesh 1.26.0). Anonymous…
- [Nefesh Human State Agent (A2A)](https://apis.io/apis/nefesh-ai/nefesh-human-state-agent-a2a/) — A2A agent served from the MCP host: card at https://mcp.nefesh.ai/.well-known/agent-card.json, JSON-RPC 2.0 endpoint at POST https://mcp.nefesh.ai/a2a…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Nefesh Ai Webhooks](https://apis.io/asyncapis/nefesh-ai/nefesh-ai-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Nefesh — Real-Time Human State Awareness for AI](https://apis.io/servers/nefesh-ai/nefesh/)

#### JSON Schema (1)

The data models the API reads and writes.

- [Human State Protocol v1.0](https://apis.io/schemas/nefesh-ai/nefesh-ai-hsp-1.0.schema/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Nefesh Ai Authentication](https://apis.io/security/nefesh-ai/nefesh-ai-authentication/)
- [Nefesh Ai Domain Security](https://apis.io/security/nefesh-ai/nefesh-ai-domain-security/)
- [Nefesh Ai Vulnerability Disclosure](https://apis.io/security/nefesh-ai/nefesh-ai-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Nefesh Ai Plans Pricing](https://apis.io/plans/nefesh-ai/nefesh-ai-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Nefesh Ai Rate Limits](https://apis.io/rate-limits/nefesh-ai/nefesh-ai-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://nefesh.ai/)
- [Documentation](https://nefesh.ai/docs)
- [Getting started](https://nefesh.ai/docs/quickstart)
- [API reference](https://nefesh.ai/docs/api)
- [Pricing](https://nefesh.ai/pricing)
- [Sign up](https://nefesh.ai/signup)
- [Security](https://nefesh.ai/.well-known/security.txt)
- [Compliance](https://nefesh.ai/docs/regulatory)
- [Terms of service](https://nefesh.ai/terms)
- [Privacy policy](https://nefesh.ai/docs/privacy)
- [GitHub](https://github.com/nefesh-ai)

## API Evangelist rating

**Kin Score 61.8** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 80.0 |
| Contract quality | 46.0 |
| Contract governance | 18.2 |
| Operational transparency | 55.3 |
| Developer ergonomics | 64.3 |
| Access clarity | 84.2 |

**Agent readiness 30.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | flavored (partial credit) |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 33.3** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/nefesh-ai/](https://apis.io/providers/nefesh-ai/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Nefesh AI: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/nefesh-ai/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
