# JarvisLabs (jarvislabs)

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
