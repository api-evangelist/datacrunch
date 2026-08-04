# DataCrunch (datacrunch)

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

DataCrunch is a European (Finland-based) GPU cloud offering on-demand and reserved NVIDIA GPU instances (H200, H100, B200, A100, L40S, V100) plus a serverless inference and container deployment platform. Its REST API at https://api.datacrunch.io/v1 uses OAuth2 client-credentials to issue Bearer tokens and exposes instances, instance types, availability, images, SSH keys, startup scripts, volumes, balance, and serverless containers, with an OpenAI-compatible inference endpoint for deployed models.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/apis.yml)

## Tags

- GPU Cloud
- Infrastructure
- Compute
- Inference
- Serverless
- Europe

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### DataCrunch Instances API

Deploy, list, inspect, and act on GPU/CPU instances. Actions (boot, shutdown, hibernate, restore, delete, force-shutdown) are issued via PUT against one or more instance IDs.

- **Human URL:** [https://api.datacrunch.io/v1/docs](https://api.datacrunch.io/v1/docs)
- **Base URL:** `https://api.datacrunch.io/v1`

#### Tags

- Instances
- Compute
- GPU

#### Properties

- [Documentation](https://docs.datacrunch.io/)
- [API Reference](https://api.datacrunch.io/v1/docs)
- [OpenAPI](openapi/datacrunch-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datacrunch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datacrunch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataCrunch Instance Types & Availability API

Lists available instance types with GPU/CPU/RAM/storage specs and per-hour pricing, and reports real-time availability across datacenter locations.

- **Human URL:** [https://api.datacrunch.io/v1/docs](https://api.datacrunch.io/v1/docs)
- **Base URL:** `https://api.datacrunch.io/v1`

#### Tags

- Instance Types
- Availability
- Catalog

#### Properties

- [Documentation](https://docs.datacrunch.io/)
- [API Reference](https://api.datacrunch.io/v1/docs)
- [OpenAPI](openapi/datacrunch-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datacrunch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datacrunch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataCrunch Images & Startup Scripts API

Lists available OS images for instances and clusters, and manages startup (cloud-init) scripts used to provision instances at deploy time.

- **Human URL:** [https://api.datacrunch.io/v1/docs](https://api.datacrunch.io/v1/docs)
- **Base URL:** `https://api.datacrunch.io/v1`

#### Tags

- Images
- Startup Scripts
- Provisioning

#### Properties

- [Documentation](https://docs.datacrunch.io/)
- [API Reference](https://api.datacrunch.io/v1/docs)
- [OpenAPI](openapi/datacrunch-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datacrunch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datacrunch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataCrunch SSH Keys API

Add, list, retrieve, and delete the SSH public keys injected into instances at deploy time for secure access.

- **Human URL:** [https://api.datacrunch.io/v1/docs](https://api.datacrunch.io/v1/docs)
- **Base URL:** `https://api.datacrunch.io/v1`

#### Tags

- SSH Keys
- Access
- Security

#### Properties

- [Documentation](https://docs.datacrunch.io/)
- [API Reference](https://api.datacrunch.io/v1/docs)
- [OpenAPI](openapi/datacrunch-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datacrunch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datacrunch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataCrunch Volumes API

Create, list, inspect, and delete block storage volumes and run volume actions (attach, detach, resize, clone, rename), including a trash listing for soft-deleted volumes and a volume-types catalog.

- **Human URL:** [https://api.datacrunch.io/v1/docs](https://api.datacrunch.io/v1/docs)
- **Base URL:** `https://api.datacrunch.io/v1`

#### Tags

- Volumes
- Storage
- Block Storage

#### Properties

- [Documentation](https://docs.datacrunch.io/)
- [API Reference](https://api.datacrunch.io/v1/docs)
- [OpenAPI](openapi/datacrunch-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datacrunch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datacrunch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataCrunch Serverless Inference & Containers API

Deploy and manage autoscaling serverless container deployments (create, list, get, update, delete, scaling, status, pause, resume, purge-queue) running vLLM/TGI/SGLang, and invoke deployed models through an OpenAI-compatible inference endpoint.

- **Human URL:** [https://docs.datacrunch.io/inference/overview](https://docs.datacrunch.io/inference/overview)
- **Base URL:** `https://api.datacrunch.io/v1`

#### Tags

- Serverless
- Inference
- Containers

#### Properties

- [Documentation](https://docs.datacrunch.io/containers/overview)
- [API Reference](https://api.datacrunch.io/v1/docs)
- [OpenAPI](openapi/datacrunch-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datacrunch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datacrunch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DataCrunch Balance API

Retrieves the project account balance and currency for the authenticated client.

- **Human URL:** [https://api.datacrunch.io/v1/docs](https://api.datacrunch.io/v1/docs)
- **Base URL:** `https://api.datacrunch.io/v1`

#### Tags

- Balance
- Billing
- Account

#### Properties

- [Documentation](https://docs.datacrunch.io/)
- [API Reference](https://api.datacrunch.io/v1/docs)
- [OpenAPI](openapi/datacrunch-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/datacrunch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/datacrunch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/DataCrunch-io)
- [LinkedIn](https://www.linkedin.com/company/datacrunch-oy)
- [Website](https://datacrunch.io)
- [Documentation](https://docs.datacrunch.io/)
- [Plans](plans/datacrunch-plans-pricing.yml)
- [Rate Limits](rate-limits/datacrunch-rate-limits.yml)
- [Fin Ops](finops/datacrunch-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
