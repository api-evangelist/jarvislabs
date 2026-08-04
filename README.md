# JarvisLabs (jarvislabs)

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

JarvisLabs.ai is a GPU cloud for AI development that lets you launch on-demand GPU and CPU instances (H100, H200, A100, RTX Pro 6000, A6000, A5000, L4, A30) from the terminal. Its Python SDK (jarvislabs / legacy jlclient) and jl CLI wrap an API for the full instance lifecycle - create, pause, resume, and destroy - plus GPU type discovery, framework templates, persistent filesystems, and managed runs for training and inference workloads, billed per minute of compute.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/apis.yml)

## Tags

- AI
- GPU
- Cloud
- Infrastructure
- Compute

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### JarvisLabs Instances API

On-demand GPU and CPU instance lifecycle - create, list, get, pause, resume, rename, and destroy instances - exposed through the jarvislabs Python SDK and jl CLI, with per-minute billing and persistent storage that survives pause and resume.

- **Human URL:** [https://docs.jarvislabs.ai/api](https://docs.jarvislabs.ai/api)
- **Base URL:** `https://api.jarvislabs.ai/v1`

#### Tags

- Instances
- GPU
- Lifecycle

#### Properties

- [Documentation](https://docs.jarvislabs.ai/api)
- [API Reference](https://docs.jarvislabs.ai/cli)
- [OpenAPI](openapi/jarvislabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/jarvislabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jarvislabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/jarvislabsai/JLClient)

### JarvisLabs GPU Types API

Lists available GPU types with real-time availability, region, VRAM, RAM, vCPU, and per-GPU-hour pricing (surfaced via the jl gpus command), used to pick hardware before launching an instance.

- **Human URL:** [https://jarvislabs.ai/pricing](https://jarvislabs.ai/pricing)
- **Base URL:** `https://api.jarvislabs.ai/v1`

#### Tags

- GPU Types
- Availability
- Catalog

#### Properties

- [Documentation](https://docs.jarvislabs.ai/cli)
- [API Reference](https://docs.jarvislabs.ai/api)
- [OpenAPI](openapi/jarvislabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/jarvislabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jarvislabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### JarvisLabs Templates API

Lists available framework templates (PyTorch, TensorFlow, JAX, VM) and persistent filesystems used to provision instances with a ready environment.

- **Human URL:** [https://docs.jarvislabs.ai/api](https://docs.jarvislabs.ai/api)
- **Base URL:** `https://api.jarvislabs.ai/v1`

#### Tags

- Templates
- Frameworks
- Images

#### Properties

- [Documentation](https://docs.jarvislabs.ai/cli)
- [API Reference](https://docs.jarvislabs.ai/api)
- [OpenAPI](openapi/jarvislabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/jarvislabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jarvislabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### JarvisLabs Inference & Deploy API

Managed runs that upload code, build a virtual environment, install dependencies, run a training or inference script on a fresh or existing instance, and auto-pause on completion - plus HTTP port exposure for serving Gradio or FastAPI inference apps.

- **Human URL:** [https://jarvislabs.ai/sdk](https://jarvislabs.ai/sdk)
- **Base URL:** `https://api.jarvislabs.ai/v1`

#### Tags

- Inference
- Deploy
- Managed Runs

#### Properties

- [Documentation](https://docs.jarvislabs.ai/)
- [API Reference](https://docs.jarvislabs.ai/cli)
- [OpenAPI](openapi/jarvislabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/jarvislabs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jarvislabs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### JarvisLabs SDK & CLI

The jarvislabs Python SDK and jl CLI (and the legacy jlclient library) wrap the JarvisLabs API for instance management, GPU discovery, templates, filesystems, SSH keys, startup scripts, and managed runs, with built-in support for AI coding agents like Claude Code, Cursor, and Codex.

- **Human URL:** [https://jarvislabs.ai/sdk](https://jarvislabs.ai/sdk)
- **Base URL:** `https://api.jarvislabs.ai/v1`

#### Tags

- SDK
- CLI
- Python

#### Properties

- [Documentation](https://jarvislabs.ai/sdk)
- [API Reference](https://docs.jarvislabs.ai/cli)
- [GitHub](https://github.com/jarvislabsai/JLClient)
- [OpenAPI](openapi/jarvislabs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/jarvislabsai)
- [LinkedIn](https://www.linkedin.com/company/jarvislabs-ai)
- [Website](https://jarvislabs.ai)
- [Documentation](https://docs.jarvislabs.ai)
- [Plans](plans/jarvislabs-plans-pricing.yml)
- [Rate Limits](rate-limits/jarvislabs-rate-limits.yml)
- [Fin Ops](finops/jarvislabs-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
