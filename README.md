# Lightning.AI

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
