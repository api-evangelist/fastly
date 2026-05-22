# Fastly (fastly)

Fastly is an edge cloud platform that helps customers create great digital experiences quickly, securely, and reliably by processing, serving, and securing their applications closer to their users. The platform spans CDN, Edge Compute (WebAssembly), Object Storage, AI Accelerator (semantic caching for LLMs), AI Bot Management, Next-Gen WAF (Signal Sciences), DDoS Protection, Image Optimizer, Live & Video Streaming, Fanout real-time messaging, and an MCP Server for AI-driven control.

**APIs.json:** [apis.yml](https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/apis.yml)

## Scope

- **Type:** Company (commercial provider)
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

CDN, Edge Cloud, Edge Compute, WebAssembly, Security, AI, Observability

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-05-22

## APIs

### Fastly Services API
The Fastly Services API allows developers to create, configure, and manage Fastly CDN services and their versions programmatically. Services are the primary organizational unit in Fastly, representing a configuration that maps domains to backends.

**Docs:** https://www.fastly.com/documentation/reference/api/services/
**OpenAPI:** [openapi/fastly-services-openapi.yml](openapi/fastly-services-openapi.yml)

### Fastly Purging API
The Fastly Purging API enables developers to instantly remove cached content from Fastly's edge network. Surrogate-key and URL purges are limited to 100,000/hour per customer and do not count against the general API rate limit.

**Docs:** https://www.fastly.com/documentation/reference/api/purging/
**OpenAPI:** [openapi/fastly-purging-openapi.yml](openapi/fastly-purging-openapi.yml)

### Fastly Real-Time Logging API
Configure and manage logging endpoints that receive streamed log data from Fastly's edge — syslog, S3, GCS, BigQuery, Datadog, Splunk, HTTPS, and more.

**Docs:** https://www.fastly.com/documentation/reference/api/logging/
**OpenAPI:** [openapi/fastly-logging-openapi.yml](openapi/fastly-logging-openapi.yml)

### Fastly Metrics and Stats API
Access both real-time (rt.fastly.com) and historical analytics for Fastly services, plus Domain Inspector and Origin Inspector.

**Docs:** https://www.fastly.com/documentation/reference/api/metrics-stats/
**OpenAPI:** [openapi/fastly-metrics-and-stats-openapi.yml](openapi/fastly-metrics-and-stats-openapi.yml)

### Fastly TLS API
Manage TLS certificates, private keys, and domain configurations. Supports both platform TLS and custom (BYO) certificates, plus mutual TLS for origins.

**Docs:** https://www.fastly.com/documentation/reference/api/tls/
**OpenAPI:** [openapi/fastly-tls-openapi.yml](openapi/fastly-tls-openapi.yml)

### Fastly VCL Services API
Configure VCL objects — backends, conditions, cache settings, request/response settings, headers, snippets, and custom VCL — that power Fastly services.

**Docs:** https://www.fastly.com/documentation/reference/api/vcl-services/
**OpenAPI:** [openapi/fastly-vcl-services-openapi.yml](openapi/fastly-vcl-services-openapi.yml)

### Fastly Account API
Manage customer accounts, users, and identity/access management (IAM) resources including roles, service groups, and user groups.

**Docs:** https://www.fastly.com/documentation/reference/api/account/
**OpenAPI:** [openapi/fastly-account-openapi.yml](openapi/fastly-account-openapi.yml)

### Fastly Authentication Tokens API
Create and manage scoped API tokens — user tokens and automation tokens — for authenticating against api.fastly.com.

**Docs:** https://www.fastly.com/documentation/reference/api/auth-tokens/
**OpenAPI:** [openapi/fastly-authentication-tokens-openapi.yml](openapi/fastly-authentication-tokens-openapi.yml)

### Fastly Access Control Lists API
Manage ACL containers of IPs/CIDR ranges referenced from VCL, with bulk-update support for large allow/blocklists.

**Docs:** https://www.fastly.com/documentation/reference/api/acls/
**OpenAPI:** [openapi/fastly-acls-openapi.yml](openapi/fastly-acls-openapi.yml)

### Fastly Edge Dictionaries API
Key-value lookup tables accessible at the edge without a service version change. Useful for feature flags, redirect maps, and dynamic configuration.

**Docs:** https://www.fastly.com/documentation/reference/api/dictionaries/
**OpenAPI:** [openapi/fastly-dictionaries-openapi.yml](openapi/fastly-dictionaries-openapi.yml)

### Fastly Compute API
WebAssembly serverless platform. Build edge apps in Rust, JavaScript, TypeScript, Go, or Python, with KV stores, config stores, secret stores, and dynamic backends.

**Docs:** https://www.fastly.com/documentation/guides/compute/
**OpenAPI:** [openapi/fastly-compute-openapi.yml](openapi/fastly-compute-openapi.yml)

### Fastly Next-Gen WAF API
Manage NGWAF (Signal Sciences) workspaces, requests, events, redactions, signals, virtual patches, and rules.

**Docs:** https://www.fastly.com/documentation/reference/api/ngwaf/
**OpenAPI:** [openapi/fastly-waf-openapi.yml](openapi/fastly-waf-openapi.yml)

### Fastly Domain Management API
Programmatically associate domains with Fastly services; validate DNS targeting Fastly.

**Docs:** https://www.fastly.com/documentation/reference/api/domain-management/
**OpenAPI:** [openapi/fastly-domain-management-openapi.yml](openapi/fastly-domain-management-openapi.yml)

### Fastly Products API
Enable and configure Fastly add-on products on services: Bot Management, **AI Bot Management**, DDoS Protection, Image Optimizer, API Discovery, **AI Accelerator**, **Object Storage**, and more.

**Docs:** https://www.fastly.com/documentation/reference/api/products/
**OpenAPI:** [openapi/fastly-products-openapi.yml](openapi/fastly-products-openapi.yml)

### Fastly Observability API
"The Fastly Observability APIs enable you to setup and manage Fastly's Observability features on your site, product or service across all our Network Services, Compute and Security product lines." Sub-resources include Alerts, Custom Dashboards, Insights, Log Aggregations, Log Explorer, Notification Service, and Timeseries.

**Docs:** https://www.fastly.com/documentation/reference/api/observability/
**OpenAPI:** [openapi/fastly-observability-openapi.yml](openapi/fastly-observability-openapi.yml)

### Fastly API Security API
"The API Security product builds a continuously updated, searchable catalog of all your API endpoints." Manage discovered Operations.

**Docs:** https://www.fastly.com/documentation/reference/api/api-security/
**OpenAPI:** [openapi/fastly-api-security-openapi.yml](openapi/fastly-api-security-openapi.yml)

### Fastly DDoS Protection Events API
"The Fastly DDoS Protection Events API allows you to configure Fastly DDoS Protection and view attack insights including events, rules, and traffic statistics."

**Docs:** https://www.fastly.com/documentation/reference/api/ddos-protection/
**OpenAPI:** [openapi/fastly-ddos-protection-openapi.yml](openapi/fastly-ddos-protection-openapi.yml)

### Fastly Client-Side Protection API
"Client-Side Protection (CSP) provides visibility and control over third-party scripts running on your web pages." Defends against Magecart and formjacking via script inventory, authorization, and security-header policies.

**Docs:** https://www.fastly.com/documentation/reference/api/client-side-protection/
**OpenAPI:** [openapi/fastly-client-side-protection-openapi.yml](openapi/fastly-client-side-protection-openapi.yml)

### Fastly Publishing (Fanout) API
"Publishing sends messages to Fanout subscribers. Fanout is designed to be GRIP-compatible, such that https://api.fastly.com/service/{service_id} can be used as a GRIP URL in application configurations."

**Docs:** https://www.fastly.com/documentation/reference/api/publishing/
**OpenAPI:** [openapi/fastly-publishing-openapi.yml](openapi/fastly-publishing-openapi.yml)

### Fastly Load Balancing API
"Spread traffic across multiple backends automatically." Manage Directors bound to VCL versions and Dynamic Server Pools that update without a new version.

**Docs:** https://www.fastly.com/documentation/reference/api/load-balancing/
**OpenAPI:** [openapi/fastly-load-balancing-openapi.yml](openapi/fastly-load-balancing-openapi.yml)

### Fastly Utilities API
"Various utilities and extra functionality we provide in addition to the configuration services" — Content Status, Diff, Docs, POPs, Public IP List, and Sudo Mode.

**Docs:** https://www.fastly.com/documentation/reference/api/utils/
**OpenAPI:** [openapi/fastly-utilities-openapi.yml](openapi/fastly-utilities-openapi.yml)

### Fastly AI Accelerator
A semantic caching solution that "boosts the performance of popular LLMs like OpenAI and Google Gemini by 9x." Exposed at `https://api.fastly.ai` with OpenAI- and Gemini-compatible endpoints. Free tier: 20,000 requests/month; PAYG $0.28–$0.40 per 1,000 requests.

**Docs:** https://www.fastly.com/products/ai
**OpenAPI:** [openapi/fastly-ai-accelerator-openapi.yml](openapi/fastly-ai-accelerator-openapi.yml)

### Fastly Object Storage
S3-compatible edge object storage with 99.999999999% durability and **zero egress fees**. Free tier: 5 GB/month; storage $0.017–$0.02/GB; Class A ops $0.0025/1K; Class B ops $0.0004/1K.

**Docs:** https://www.fastly.com/products/object-storage
**OpenAPI:** [openapi/fastly-object-storage-openapi.yml](openapi/fastly-object-storage-openapi.yml)

## Naftiko Capabilities

Per-API shared capabilities are generated under [`capabilities/`](capabilities/). Notable 2026 additions: AI Accelerator chat completions, AI Bot Management product, Object Storage bucket & object, Observability alerts/dashboards/log-explorer/notification-service/timeseries, API Security operations, DDoS Protection events & rules, Client-Side Protection websites/scripts/policies, Fanout publishing, Load Balancing directors & pools, Utilities POPs & public IP list.

## Plans, Rate Limits, FinOps

- **Plans:** [plans/fastly-plans-pricing.yml](plans/fastly-plans-pricing.yml) — CDN Free + PAYG, Compute, Object Storage, AI Accelerator, Image Optimizer, Domain Research, Basic ($1,500/mo) / Starter ($6,000/mo) / Advantage / Ultimate packages, plus security add-on bundle.
- **Rate Limits:** [rate-limits/fastly-rate-limits.yml](rate-limits/fastly-rate-limits.yml) — 1,000 req/hr per token; 100,000/hour separate purge quota; free-tier ceilings per product.
- **FinOps:** [finops/fastly-finops.yml](finops/fastly-finops.yml) — FOCUS-aligned billing surface across CDN, Compute, Object Storage, AI Accelerator, and Image Optimizer.

## Semantics

- **JSON-LD:** [json-ld/fastly-context.jsonld](json-ld/fastly-context.jsonld)
- **JSON Schema:** [json-schema/](json-schema/) — Service, Backend, ACLEntry, DictionaryItem, TLSCertificate, AI Accelerator Request, Object Storage Object, DDoS Event.
- **Vocabulary:** [vocabulary/fastly-vocabulary.yml](vocabulary/fastly-vocabulary.yml)
- **Spectral Rules:** [rules/fastly-rules.yml](rules/fastly-rules.yml)
- **Examples:** [examples/](examples/)

## Common Properties

- [Developer Portal](https://www.fastly.com/documentation/)
- [API Reference](https://www.fastly.com/documentation/reference/api/)
- [Pricing](https://www.fastly.com/pricing)
- [Blog](https://www.fastly.com/blog/)
- [Status](https://www.fastlystatus.com/)
- [Support](https://support.fastly.com/)
- [Login](https://manage.fastly.com/account/company)
- [Signup](https://www.fastly.com/signup)
- [Privacy Policy](https://www.fastly.com/privacy/)
- [Terms of Service](https://www.fastly.com/terms/)
- [GitHub Org](https://github.com/fastly) (287 public repos)
- [LinkedIn](https://www.linkedin.com/company/fastly)

## SDKs, CLIs, Tools (from github.com/fastly)

- **CLI:** [fastly/cli](https://github.com/fastly/cli) (Go)
- **API clients:** [fastly-py](https://github.com/fastly/fastly-py), [fastly-rust](https://github.com/fastly/fastly-rust), [fastly-go](https://github.com/fastly/fastly-go), [fastly-ruby](https://github.com/fastly/fastly-ruby), [fastly-js](https://github.com/fastly/fastly-js), [fastly-php](https://github.com/fastly/fastly-php), [fastly-perl](https://github.com/fastly/fastly-perl), [go-fastly](https://github.com/fastly/go-fastly)
- **Compute SDKs/runtimes:** [compute-sdk-go](https://github.com/fastly/compute-sdk-go), [js-compute-runtime](https://github.com/fastly/js-compute-runtime), [compute-sdk-python](https://github.com/fastly/compute-sdk-python)
- **Local testing:** [Viceroy](https://github.com/fastly/Viceroy)
- **IaC:** [terraform-provider-fastly](https://github.com/fastly/terraform-provider-fastly)
- **AI:** [mcp](https://github.com/fastly/mcp) (Model Context Protocol server, ~37 stars), [fastly-agent-toolkit](https://github.com/fastly/fastly-agent-toolkit) (skills for AI agents)
- **Observability:** [fastly-exporter](https://github.com/fastly/fastly-exporter) (Prometheus exporter)
- **IDE:** [vscode-fastly-vcl](https://github.com/fastly/vscode-fastly-vcl)
- **Integrations:** [WordPress-Plugin](https://github.com/fastly/WordPress-Plugin), [fastly-magento2](https://github.com/fastly/fastly-magento2)
- **Fanout core:** [pushpin](https://github.com/fastly/pushpin) (3,844 stars)

## Notable 2026 Product Lines

- **CDN, Compute, Live/Video Streaming, Image Optimizer, Object Storage** (delivery + storage)
- **Next-Gen WAF, Bot Management, AI Bot Management, DDoS Protection, API Security, Client-Side Protection** (security)
- **AI Accelerator, MCP Server** (AI)
- **Observability suite** — Alerts, Dashboards, Log Explorer, Notification Service, Insights, Timeseries
- **Fanout / Publishing** real-time WebSocket / HTTP-stream fan-out

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
