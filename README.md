# Lightning.AI

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Lightning AI is an AI development cloud from the creators of PyTorch Lightning — browser-based GPU
Studios, batch and multi-node training jobs, autoscaled deployments, ephemeral code-execution
Sandboxes, and an OpenAI-compatible LLM gateway (Model APIs) fronting hosted models from OpenAI,
Anthropic, Google and open-weights providers behind one key and one bill.

- Website: https://lightning.ai/
- Docs: https://lightning.ai/docs
- Developers: https://lightning.ai/docs/platform/developers
- GitHub: https://github.com/Lightning-AI
- Status: https://status.lightning.ai/

## APIs

| API | Base URL | Auth |
|---|---|---|
| Lightning AI Model APIs | `https://lightning.ai/v1` | Bearer (`lightning api-key get`) |
| Lightning AI Platform API | `https://lightning.ai/api/v1` | HTTP Basic (`LIGHTNING_USER_ID` : `LIGHTNING_API_KEY`) |

The public model catalog is served unauthenticated at `https://lightning.ai/api/v1/models`.

## Artifacts in this repo

| Directory | What |
|---|---|
| `llms/` | `llms.txt` saved verbatim from https://lightning.ai/llms.txt |
| `skills/` | Six Agent Skills saved verbatim from https://github.com/Lightning-AI/skills |
| `packages/` | First-party PyPI + npm client libraries and frameworks |
| `cli/` | The `lightning` CLI command surface |
| `authentication/` | The two auth schemes (Basic for the platform, Bearer for Model APIs) |
| `conventions/` | Cross-cutting request/response semantics and the gRPC-gateway error envelope |
| `rate-limits/` | Published per-plan Model API rate limits |
| `conformance/` | SOC 2 Type II, HIPAA, CPRA, DPA and technical-standards posture |
| `lifecycle/` | Versioning, status page, and what is not published |
| `sandbox/` | Free tier, console and ephemeral Sandbox environments |
| `well-known/` | `/.well-known/` probe results (all soft-404 behind the SPA) |
| `security/` | TLS/HSTS/DNSSEC/CAA/SPF/DMARC probe results |

## Not published by Lightning AI

No OpenAPI/Swagger, no AsyncAPI or webhook catalog, no gRPC `.proto`, no OAuth 2.0 / OpenID
Connect discovery (so no scopes), no `/.well-known/security.txt`, no vulnerability-disclosure or
bug-bounty program, no trust center, no MCP server, no dated platform changelog, no published
deprecation policy or SLA, and no idempotency contract.

Backed by: bain-capital-ventures
