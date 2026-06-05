# Fastly (fastly)

Fastly is an edge cloud platform that helps customers create great digital experiences quickly, securely, and reliably by processing, serving, and securing their applications closer to their users. The platform spans CDN, Edge Compute (WebAssembly), Object Storage, AI Accelerator (semantic caching for LLMs), AI Bot Management, Next-Gen WAF (Signal Sciences), DDoS Protection, Image Optimizer, Live & Video Streaming, Fanout real-time messaging, and an MCP Server for AI-driven control.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/apis.yml)

## Tags

- CDN
- Edge Cloud
- Edge Compute
- WebAssembly
- Security
- AI
- Observability
- AsyncAPI
- Streaming
- Webhooks
- Logging

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-05-30

## APIs

### Fastly Services API

The Fastly Services API allows developers to create, configure, and manage Fastly CDN services and their versions programmatically. Services are the primary organizational unit in Fastly, representing a configuration that maps domains to backends. The API supports creating service versions, activating and deactivating configurations, cloning versions, and managing the complete lifecycle of a CDN service deployment.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/services/](https://www.fastly.com/documentation/reference/api/services/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- CDN
- Configuration
- Edge Cloud
- Services

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/services/)
- [OpenAPI](openapi/fastly-services-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-services.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-services.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Purging API

The Fastly Purging API enables developers to instantly remove cached content from Fastly's edge network so it can be refreshed from origin servers. It supports single URL purges, surrogate key purges for invalidating groups of related objects, and purge-all operations to clear an entire service cache. Surrogate key and URL purges are separately limited to an average of 100,000 purges per hour per customer and are not counted against the general API rate limit.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/purging/](https://www.fastly.com/documentation/reference/api/purging/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Cache
- CDN
- Content Delivery
- Purging

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/purging/)
- [OpenAPI](openapi/fastly-purging-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-purging.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-purging.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Real-Time Logging API

The Fastly Real-Time Logging API allows developers to configure and manage logging endpoints that receive streamed log data from Fastly's edge network. Fastly supports logging to a variety of formats and platforms including syslog, Amazon S3, Google Cloud Storage, BigQuery, Datadog, Splunk, Elasticsearch, and many other providers.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/logging/](https://www.fastly.com/documentation/reference/api/logging/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Analytics
- Logging
- Monitoring
- Observability

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/logging/)
- [OpenAPI](openapi/fastly-logging-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-logging.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-logging.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/fastly-streaming-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Fastly Metrics and Stats API

The Fastly Metrics and Stats API provides access to both real-time and historical analytics data for Fastly services. The real-time analytics endpoint, served on rt.fastly.com, delivers second-by-second stats including request counts, bandwidth, cache hit ratios, and error rates. Historical stats provide aggregated data over longer time periods. The API also includes the Domain Inspector for per-domain metrics and the Origin Inspector for origin-level performance data.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/metrics-stats/](https://www.fastly.com/documentation/reference/api/metrics-stats/)
- **Base URL:** `https://rt.fastly.com`

#### Tags

- Analytics
- Metrics
- Monitoring
- Real-Time
- Statistics

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/metrics-stats/)
- [OpenAPI](openapi/fastly-metrics-and-stats-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-metrics-and-stats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-metrics-and-stats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/fastly-streaming-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Fastly TLS API

The Fastly TLS API enables developers to manage TLS certificates, private keys, and domain configurations for securing traffic delivered through Fastly's edge network. It supports both platform TLS (managed certificates) and custom TLS configurations where customers bring their own certificates. The API allows uploading certificates, managing bulk certificate operations, configuring TLS activations, and managing mutual TLS authentication for origin connections.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/tls/](https://www.fastly.com/documentation/reference/api/tls/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Certificates
- Encryption
- Security
- SSL
- TLS

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/tls/)
- [OpenAPI](openapi/fastly-tls-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-tls.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-tls.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly VCL Services API

The Fastly VCL Services API provides programmatic access to configure Varnish Configuration Language (VCL) objects that power most Fastly services. Developers can upload custom VCL code or use the API to generate VCL through configuration objects including backends, conditions, cache settings, request settings, response objects, headers, and VCL snippets. This API is central to defining how Fastly processes, routes, and caches HTTP requests at the edge.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/vcl-services/](https://www.fastly.com/documentation/reference/api/vcl-services/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Caching
- CDN
- Configuration
- Edge Logic
- VCL

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/vcl-services/)
- [OpenAPI](openapi/fastly-vcl-services-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-vcl-services.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-vcl-services.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Account API

The Fastly Account API provides endpoints for managing customer accounts, users, and identity and access management (IAM) resources. Developers can programmatically manage user invitations, roles, permissions, and service groups to control access to Fastly resources. The API supports retrieving and updating customer information, managing user profiles, and configuring organizational settings for enterprise accounts.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/account/](https://www.fastly.com/documentation/reference/api/account/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Account
- Administration
- IAM
- Users

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/account/)
- [OpenAPI](openapi/fastly-account-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-account.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-account.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Authentication Tokens API

The Fastly Authentication Tokens API enables developers to create and manage API tokens used to authenticate requests to the Fastly API. Tokens can be scoped to specific services and permissions, allowing fine-grained access control for users and automated systems. The API supports creating user tokens, automation tokens for CI/CD pipelines, and managing token lifecycle including listing, revoking, and expiring tokens.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/auth-tokens/](https://www.fastly.com/documentation/reference/api/auth-tokens/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- API Keys
- Authentication
- Security
- Tokens

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/auth-tokens/)
- [OpenAPI](openapi/fastly-authentication-tokens-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-authentication-tokens.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-authentication-tokens.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Access Control Lists API

The Fastly Access Control Lists API allows developers to create and manage ACLs that can be used to control access to content at the edge. ACLs contain entries of IP addresses or CIDR ranges that can be referenced in VCL to allow or deny requests. The API supports creating ACL containers, adding and removing individual entries, and performing bulk updates to efficiently manage large IP allowlists or blocklists without requiring a new service version deployment.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/acls/](https://www.fastly.com/documentation/reference/api/acls/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Access Control
- Edge Security
- IP Filtering
- Security

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/acls/)
- [OpenAPI](openapi/fastly-acls-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-acls.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-acls.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Edge Dictionaries API

The Fastly Edge Dictionaries API provides endpoints for creating and managing key-value lookup tables that are accessible at the edge without requiring a service version change. Dictionaries can store configuration data, feature flags, redirect mappings, and other dynamic values that VCL or Compute services can reference during request processing.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/dictionaries/](https://www.fastly.com/documentation/reference/api/dictionaries/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Dictionaries
- Dynamic Configuration
- Edge Configuration
- Key-Value

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/dictionaries/)
- [OpenAPI](openapi/fastly-dictionaries-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-dictionaries.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-dictionaries.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Compute API

The Fastly Compute platform enables developers to build and deploy serverless applications that run on Fastly's global edge network using WebAssembly. Compute services support custom application logic written in Rust, JavaScript, or Go using official Fastly SDKs, with access to KV stores, config stores, secret stores, dynamic backends, and real-time messaging.

- **Human URL:** [https://www.fastly.com/documentation/guides/compute/](https://www.fastly.com/documentation/guides/compute/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Compute
- Edge Computing
- Serverless
- WebAssembly

#### Properties

- [Documentation](https://www.fastly.com/documentation/guides/compute/)
- [OpenAPI](openapi/fastly-compute-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-compute.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-compute.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Next-Gen WAF API

The Fastly Next-Gen WAF (formerly Signal Sciences) API allows you to manage workspaces, requests, events, redactions, tags, and rules. Resources include Agent Keys, Agents, Custom Dashboards, Custom Signals, Events, Header Links, Lists, Rate Limited Sources, Redactions, Reports, Requests, Rules, Simulate, Thresholds, Time Series, Virtual Patches, Workspace Alerts, and Workspaces.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/ngwaf/](https://www.fastly.com/documentation/reference/api/ngwaf/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- DDoS Protection
- Security
- Signal Sciences
- WAF
- Web Application Firewall

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/ngwaf/)
- [OpenAPI](openapi/fastly-waf-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-waf.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-waf.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Domain Management API

The Fastly Domain Management API allows developers to programmatically associate domain names with Fastly services. Domains serve as the entry point for traffic routed through Fastly's edge network. The API supports adding, listing, and removing domains from service versions, checking domain DNS configurations, and validating that domains are correctly pointed to Fastly.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/domain-management/](https://www.fastly.com/documentation/reference/api/domain-management/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- CDN
- Configuration
- DNS
- Domains

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/domain-management/)
- [OpenAPI](openapi/fastly-domain-management-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-domain-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-domain-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Products API

The Fastly Products API provides endpoints for enabling and managing Fastly product features on services, including Bot Management, AI Bot Management, DDoS Protection, Image Optimizer, API Discovery, AI Accelerator, Object Storage, and other add-on capabilities. Developers use this API to check which products are enabled for a service, enable or disable product features, and configure product-specific settings.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/products/](https://www.fastly.com/documentation/reference/api/products/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Configuration
- Features
- Platform
- Products

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/products/)
- [OpenAPI](openapi/fastly-products-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-products.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-products.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Observability API

The Fastly Observability APIs enable you to setup and manage Fastly's Observability features on your site, product or service across all our Network Services, Compute and Security product lines. Sub-resources include Alerts, Custom Dashboards, Insights, Log Aggregations, Log Explorer, Notification Service, and Timeseries.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/observability/](https://www.fastly.com/documentation/reference/api/observability/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Alerts
- Dashboards
- Insights
- Logging
- Notifications
- Observability

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/observability/)
- [OpenAPI](openapi/fastly-observability-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-observability.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-observability.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/fastly-streaming-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Fastly API Security API

The Fastly API Security product builds a continuously updated, searchable catalog of all your API endpoints. The API exposes Operations sub-resources for managing discovered API operations through listing, creation, updates, deletion, and tag-based organization capabilities. It supports the broader API Security product that maps API landscape and enables targeted abuse mitigation decisions.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/api-security/](https://www.fastly.com/documentation/reference/api/api-security/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- API Discovery
- API Security
- Catalog
- Security

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/api-security/)
- [OpenAPI](openapi/fastly-api-security-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Fastly DDoS Protection Events API

The Fastly DDoS Protection Events API allows you to configure Fastly DDoS Protection and view attack insights including events, rules, and traffic statistics. Endpoints are exposed under /ddos-protection/v1/ and cover Get events, Get event by ID, Get all rules for an event, Get a rule by ID, Update rule, and Get traffic stats for a rule.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/ddos-protection/](https://www.fastly.com/documentation/reference/api/ddos-protection/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Attack Mitigation
- DDoS Protection
- Events
- Security

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/ddos-protection/)
- [OpenAPI](openapi/fastly-ddos-protection-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-ddos-protection.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-ddos-protection.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/fastly-streaming-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Fastly Client-Side Protection API

Fastly Client-Side Protection (CSP) provides visibility and control over third-party scripts running on your web pages. The API monitors script behavior, manages authorization status, and configures security policies to defend against client-side attacks like Magecart and formjacking. It exposes Website, Page, Script, Policy, Policy Report, Security Header, and Header Event sub-resources.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/client-side-protection/](https://www.fastly.com/documentation/reference/api/client-side-protection/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Client-Side Protection
- CSP
- Magecart
- Script Monitoring
- Security

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/client-side-protection/)
- [OpenAPI](openapi/fastly-client-side-protection-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-client-side-protection.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-client-side-protection.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Publishing (Fanout) API

The Fastly Publishing API sends messages to Fanout subscribers. Fanout is designed to be GRIP-compatible, such that https://api.fastly.com/service/{service_id} can be used as a GRIP URL in application configurations. It delivers messages to subscribers across HTTP responses, HTTP streams, and WebSocket connections for real-time, edge-scale fan-out messaging.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/publishing/](https://www.fastly.com/documentation/reference/api/publishing/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Fanout
- GRIP
- Messaging
- Publish-Subscribe
- Real-Time
- WebSockets

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/publishing/)
- [OpenAPI](openapi/fastly-publishing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-publishing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-publishing.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/fastly-streaming-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Fastly Load Balancing API

The Fastly Load Balancing API spreads traffic across multiple backends automatically. It exposes two primary mechanisms - Directors bound to VCL service versions for locked configurations with multiple director groups, and Dynamic Server Pools that allow servers to be added or removed without activating new service versions.

- **Human URL:** [https://www.fastly.com/documentation/reference/api/load-balancing/](https://www.fastly.com/documentation/reference/api/load-balancing/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Backends
- Directors
- Load Balancing
- Routing

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/load-balancing/)
- [OpenAPI](openapi/fastly-load-balancing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-load-balancing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-load-balancing.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Utilities API

The Fastly Utilities API covers various utilities and extra functionality provided in addition to the configuration services. Endpoints include Content Status (which version of a URL is cached on each edge server), Diff (compare configuration changes between versions), Docs, POPs (Points of Presence), Public IP List (Fastly's assigned IP ranges), and Sudo Mode (privileged actions through re-authentication).

- **Human URL:** [https://www.fastly.com/documentation/reference/api/utils/](https://www.fastly.com/documentation/reference/api/utils/)
- **Base URL:** `https://api.fastly.com`

#### Tags

- Content Status
- Diff
- POPs
- Public IP List
- Sudo Mode
- Utilities

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/utils/)
- [OpenAPI](openapi/fastly-utilities-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-utilities.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-utilities.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly AI Accelerator

Fastly AI Accelerator is a semantic caching solution that "boosts the performance of popular LLMs like OpenAI and Google Gemini by 9x" with minimal implementation effort. Semantic caching maps queries to concepts as vectors so the system can cache answers to similar questions regardless of exact wording, identifying and reusing similar or equivalent AI responses rather than caching only exact matches. The free tier is 20,000 requests/month with pricing from $0.40-$0.28 per 1,000 requests by volume.

- **Human URL:** [https://www.fastly.com/products/ai](https://www.fastly.com/products/ai)
- **Base URL:** `https://api.fastly.ai`

#### Tags

- AI
- LLM
- Semantic Caching
- OpenAI
- Google Gemini

#### Properties

- [Documentation](https://www.fastly.com/products/ai)
- [OpenAPI](openapi/fastly-ai-accelerator-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-ai-accelerator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-ai-accelerator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fastly Object Storage

Fastly Object Storage is an S3-compatible cloud storage solution designed as a drop-in replacement for traditional object storage services, featuring zero egress fees and 99.999999999% (11 9's) data durability. It maintains API compatibility with Amazon S3, allowing developers to use existing code and tools without modifications. Pricing starts at 5 GB free, $0.017-$0.02/GB storage, $0.0025 per 1,000 Class A ops, and $0.0004 per 1,000 Class B ops.

- **Human URL:** [https://www.fastly.com/products/object-storage](https://www.fastly.com/products/object-storage)
- **Base URL:** `https://storage.fastly.com`

#### Tags

- Object Storage
- S3 Compatible
- Storage
- Zero Egress

#### Properties

- [Documentation](https://www.fastly.com/products/object-storage)
- [OpenAPI](openapi/fastly-object-storage-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fastly-object-storage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fastly-object-storage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Website](https://www.fastly.com/)
- [Developer Portal](https://www.fastly.com/documentation/)
- [API Reference](https://www.fastly.com/documentation/reference/api/)
- [Documentation](https://www.fastly.com/documentation/)
- [Pricing](https://www.fastly.com/pricing)
- [Blog](https://www.fastly.com/blog/)
- [Status Page](https://www.fastlystatus.com/)
- [Support](https://support.fastly.com/)
- [Login](https://manage.fastly.com/account/company)
- [Signup](https://www.fastly.com/signup)
- [Privacy Policy](https://www.fastly.com/privacy/)
- [Terms of Service](https://www.fastly.com/terms/)
- [GitHub Organization](https://github.com/fastly)
- [LinkedIn](https://www.linkedin.com/company/fastly)
- [Twitter](https://twitter.com/fastly)
- [C L I](https://github.com/fastly/cli)
- [SDK](https://github.com/fastly/fastly-py)
- [SDK](https://github.com/fastly/fastly-go)
- [SDK](https://github.com/fastly/fastly-rust)
- [SDK](https://github.com/fastly/fastly-ruby)
- [SDK](https://github.com/fastly/fastly-js)
- [SDK](https://github.com/fastly/fastly-php)
- [SDK](https://github.com/fastly/fastly-perl)
- [SDK](https://github.com/fastly/go-fastly)
- [SDK](https://github.com/fastly/compute-sdk-go)
- [SDK](https://github.com/fastly/js-compute-runtime)
- [SDK](https://github.com/fastly/compute-sdk-python)
- [Tools](https://github.com/fastly/terraform-provider-fastly)
- [Tools](https://github.com/fastly/Viceroy)
- [Tools](https://github.com/fastly/mcp)
- [Tools](https://github.com/fastly/fastly-agent-toolkit)
- [Tools](https://github.com/fastly/fastly-exporter)
- [Tools](https://github.com/fastly/vscode-fastly-vcl)
- [Integration](https://github.com/fastly/WordPress-Plugin)
- [Integration](https://github.com/fastly/fastly-magento2)
- [JSON-LD](json-ld/fastly-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/fastly-vocabulary.yml)
- [Plans](plans/fastly-plans-pricing.yml)
- [Rate Limits](rate-limits/fastly-rate-limits.yml)
- [Fin Ops](finops/fastly-finops.yml)
- [JSON Schema](json-schema/fastly-service-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fastly-backend-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fastly-acl-entry-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fastly-dictionary-item-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fastly-tls-certificate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fastly-ai-accelerator-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fastly-object-storage-object-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fastly-ddos-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Spectral Ruleset](rules/fastly-rules.yml)
- [Examples](examples/fastly-ai-accelerator-chat-completion-example.json)
- [Examples](examples/fastly-object-storage-put-object-example.json)
- [Examples](examples/fastly-ddos-protection-list-events-example.json)
- [Examples](examples/fastly-observability-alert-definition-example.json)
- [Features](undefined)
