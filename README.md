# Hailo

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

Hailo Technologies Ltd. is an Israeli fabless semiconductor company, headquartered in Tel Aviv with offices in the United States, Germany, Japan, Taiwan, China and South Korea, that designs AI inference accelerators (the Hailo-8, Hailo-8L and Hailo-10 families) and AI vision processors (the Hailo-15 SoC family) for edge devices. Its developer surface is not a hosted web API: it is an on-device software stack published largely on GitHub under the hailo-ai organization — HailoRT, a C/C++/Python runtime library plus the hailortcli command line tool and a PCIe kernel driver; the Hailo Model Zoo of pre-compiled HEF models; TAPPAS and hailo-apps application pipelines; and the Hailo Media Library and Hailo Imaging stacks for the Hailo-15 vision processor. The machine-readable contracts Hailo publishes are Protocol Buffers — a 33-RPC gRPC MediaLibraryService, the HailoRT hRPC and GenAI message schemes, the HEF model-file format, and a WebSocket/ZMQ analytics metadata scheme. Hailo also publishes a first-party Agent Skills package (hailo15-agentic-coding) of twelve skills that drive board connection, pipeline editing, model swapping, cross-compilation and deployment on the Hailo-15 SBC.

**Areas:** Artificial Intelligence · Machine Learning · Semiconductors · Edge Computing · Computer Vision · Inference · Embedded Systems · Video Analytics · Hardware · Generative AI · Protocol Buffers · gRPC

## Hailo on APIs.io

Everything profiled for Hailo is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/hailo/](https://apis.io/providers/hailo/)** — or go straight to one of the APIs or properties below.

### APIs (2)

- [HailoRT](https://apis.io/apis/hailo/hailo-hailort/) — HailoRT is Hailo's production runtime library for the Hailo-8, Hailo-10 and Hailo-15 device families. It is a host-side, user-space C/C++ library with a…
- [Hailo Media Library Service](https://apis.io/apis/hailo/hailo-media-library/) — The Hailo Media Library is the C++ media and vision stack for the Hailo-15 AI vision processor. It exposes a real gRPC contract — service…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Hailo Authentication](https://apis.io/security/hailo/hailo-authentication/)
- [Hailo Domain Security](https://apis.io/security/hailo/hailo-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Hailo Plans Pricing](https://apis.io/plans/hailo/hailo-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Hailo Rate Limits](https://apis.io/rate-limits/hailo/hailo-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://hailo.ai/)
- [Documentation](https://hailo.ai/developer-zone/documentation/)
- [API reference](https://hailo.ai/developer-zone/documentation/hailort/latest/)
- [Support](https://community.hailo.ai/)
- [Blog](https://hailo.ai/blog/)
- [Terms of service](https://hailo.ai/terms-and-conditions/website-terms-of-use/)
- [Privacy policy](https://hailo.ai/terms-and-conditions/privacy-policy/)
- [GitHub](https://github.com/hailo-ai)

## API Evangelist rating

**Kin Score 32.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 24.0 |
| Contract governance | 4.5 |
| Operational transparency | 18.4 |
| Developer ergonomics | 66.7 |
| Access clarity | 21.1 |

**Agent readiness 20.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 22.7** — AI & Biometrics

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/hailo/](https://apis.io/providers/hailo/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Hailo: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/hailo/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
