# DataCrunch (datacrunch)

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
