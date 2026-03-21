# Fastly (fastly)
Fastly is an edge cloud platform that provides content delivery network (CDN), serverless compute, security, and observability services. Their developer platform offers a comprehensive suite of APIs for programmatically managing CDN services, edge configurations, caching, TLS certificates, web application firewalls, and real-time analytics across Fastly's global edge network.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - CDN, Edge Cloud, Security, Serverless, Caching, Performance, Observability

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-03-20

## APIs

### Fastly Services API
The Fastly Services API allows developers to create, configure, and manage Fastly CDN services and their versions programmatically. Services are the primary organizational unit in Fastly, representing a configuration that maps domains to backends. The API supports creating service versions, activating and deactivating configurations, cloning versions, and managing the complete lifecycle of a CDN service deployment.

**Human URL:** [https://www.fastly.com/documentation/reference/api/services/](https://www.fastly.com/documentation/reference/api/services/)


#### Tags:

 - CDN, Services, Edge Cloud, Configuration

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/services/)

### Fastly Purging API
The Fastly Purging API enables developers to instantly remove cached content from Fastly's edge network so it can be refreshed from origin servers. It supports single URL purges, surrogate key purges for invalidating groups of related objects, and purge-all operations to clear an entire service cache. Surrogate key and URL purges are separately limited to an average of 100,000 purges per hour per customer and are not counted against the general API rate limit.

**Human URL:** [https://www.fastly.com/documentation/reference/api/purging/](https://www.fastly.com/documentation/reference/api/purging/)


#### Tags:

 - Purging, Cache, CDN, Content Delivery

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/purging/)

### Fastly Real-Time Logging API
The Fastly Real-Time Logging API allows developers to configure and manage logging endpoints that receive streamed log data from Fastly's edge network. Fastly supports logging to a variety of formats and platforms including syslog, Amazon S3, Google Cloud Storage, BigQuery, Datadog, Splunk, Elasticsearch, and many other providers. Developers can create, update, and delete logging configurations per service version, controlling the format, placement, and conditions under which log entries are generated.

**Human URL:** [https://www.fastly.com/documentation/reference/api/logging/](https://www.fastly.com/documentation/reference/api/logging/)


#### Tags:

 - Logging, Observability, Monitoring, Analytics

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/logging/)

### Fastly Metrics and Stats API
The Fastly Metrics and Stats API provides access to both real-time and historical analytics data for Fastly services. The real-time analytics endpoint, served on rt.fastly.com, delivers second-by-second stats including request counts, bandwidth, cache hit ratios, and error rates. Historical stats provide aggregated data over longer time periods. The API also includes the Domain Inspector for per-domain metrics and the Origin Inspector for origin-level performance data.

**Human URL:** [https://www.fastly.com/documentation/reference/api/metrics-stats/](https://www.fastly.com/documentation/reference/api/metrics-stats/)


#### Tags:

 - Analytics, Metrics, Statistics, Real-Time, Monitoring

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/metrics-stats/)

### Fastly TLS API
The Fastly TLS API enables developers to manage TLS certificates, private keys, and domain configurations for securing traffic delivered through Fastly's edge network. It supports both platform TLS (managed certificates) and custom TLS configurations where customers bring their own certificates. The API allows uploading certificates, managing bulk certificate operations, configuring TLS activations, and managing mutual TLS authentication for origin connections.

**Human URL:** [https://www.fastly.com/documentation/reference/api/tls/](https://www.fastly.com/documentation/reference/api/tls/)


#### Tags:

 - TLS, SSL, Certificates, Security, Encryption

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/tls/)

### Fastly VCL Services API
The Fastly VCL Services API provides programmatic access to configure Varnish Configuration Language (VCL) objects that power most Fastly services. Developers can upload custom VCL code or use the API to generate VCL through configuration objects including backends, conditions, cache settings, request settings, response objects, headers, and VCL snippets. This API is central to defining how Fastly processes, routes, and caches HTTP requests at the edge.

**Human URL:** [https://www.fastly.com/documentation/reference/api/vcl-services/](https://www.fastly.com/documentation/reference/api/vcl-services/)


#### Tags:

 - VCL, Configuration, Edge Logic, CDN, Caching

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/vcl-services/)

### Fastly Account API
The Fastly Account API provides endpoints for managing customer accounts, users, and identity and access management (IAM) resources. Developers can programmatically manage user invitations, roles, permissions, and service groups to control access to Fastly resources. The API supports retrieving and updating customer information, managing user profiles, and configuring organizational settings for enterprise accounts.

**Human URL:** [https://www.fastly.com/documentation/reference/api/account/](https://www.fastly.com/documentation/reference/api/account/)


#### Tags:

 - Account, Users, IAM, Administration

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/account/)

### Fastly Authentication Tokens API
The Fastly Authentication Tokens API enables developers to create and manage API tokens used to authenticate requests to the Fastly API. Tokens can be scoped to specific services and permissions, allowing fine-grained access control for users and automated systems. The API supports creating user tokens, automation tokens for CI/CD pipelines, and managing token lifecycle including listing, revoking, and expiring tokens.

**Human URL:** [https://www.fastly.com/documentation/reference/api/auth-tokens/](https://www.fastly.com/documentation/reference/api/auth-tokens/)


#### Tags:

 - Authentication, Tokens, Security, API Keys

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/auth-tokens/)

### Fastly Access Control Lists API
The Fastly Access Control Lists API allows developers to create and manage ACLs that can be used to control access to content at the edge. ACLs contain entries of IP addresses or CIDR ranges that can be referenced in VCL to allow or deny requests. The API supports creating ACL containers, adding and removing individual entries, and performing bulk updates to efficiently manage large IP allowlists or blocklists without requiring a new service version deployment.

**Human URL:** [https://www.fastly.com/documentation/reference/api/acls/](https://www.fastly.com/documentation/reference/api/acls/)


#### Tags:

 - Access Control, Security, IP Filtering, Edge Security

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/acls/)

### Fastly Edge Dictionaries API
The Fastly Edge Dictionaries API provides endpoints for creating and managing key-value lookup tables that are accessible at the edge without requiring a service version change. Dictionaries can store configuration data, feature flags, redirect mappings, and other dynamic values that VCL or Compute services can reference during request processing. The API supports CRUD operations on both dictionary containers and their individual items, as well as bulk updates for efficient management of large datasets.

**Human URL:** [https://www.fastly.com/documentation/reference/api/dictionaries/](https://www.fastly.com/documentation/reference/api/dictionaries/)


#### Tags:

 - Dictionaries, Key-Value, Edge Configuration, Dynamic Configuration

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/dictionaries/)

### Fastly Compute API
The Fastly Compute platform enables developers to build and deploy serverless applications that run on Fastly's global edge network using WebAssembly. Compute services support custom application logic written in Rust, JavaScript, or Go using official Fastly SDKs. The platform provides access to edge primitives including KV stores, config stores, secret stores, dynamic backends, and real-time messaging, enabling developers to build full-featured applications that execute close to end users with sub-millisecond startup times.

**Human URL:** [https://www.fastly.com/documentation/guides/compute/](https://www.fastly.com/documentation/guides/compute/)


#### Tags:

 - Serverless, Edge Computing, WebAssembly, Compute

#### Properties

- [Documentation](https://www.fastly.com/documentation/guides/compute/)

### Fastly Next-Gen WAF API
The Fastly Next-Gen WAF API provides programmatic access to configure and manage web application firewall rules that protect applications delivered through Fastly's edge network. It enables developers to manage WAF firewall configurations, rule sets, and exclusions to defend against common web attacks including SQL injection, cross-site scripting, and other OWASP Top 10 vulnerabilities. The API supports managing active rules, reviewing firewall events, and configuring response behaviors for detected threats.

**Human URL:** [https://www.fastly.com/documentation/reference/api/waf/](https://www.fastly.com/documentation/reference/api/waf/)


#### Tags:

 - WAF, Web Application Firewall, Security, DDoS Protection

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/waf/)

### Fastly Domain Management API
The Fastly Domain Management API allows developers to programmatically associate domain names with Fastly services. Domains serve as the entry point for traffic routed through Fastly's edge network. The API supports adding, listing, and removing domains from service versions, checking domain DNS configurations, and validating that domains are correctly pointed to Fastly. It is essential for managing the routing configuration that connects end-user requests to the appropriate Fastly service.

**Human URL:** [https://www.fastly.com/documentation/reference/api/services/domain/](https://www.fastly.com/documentation/reference/api/services/domain/)


#### Tags:

 - Domains, DNS, Configuration, CDN

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/services/domain/)

### Fastly Products API
The Fastly Products API provides endpoints for enabling and managing Fastly product features on services, including Bot Management, DDoS Protection, Image Optimizer, API Discovery, and other add-on capabilities. Developers can use this API to check which products are enabled for a service, enable or disable product features, and configure product-specific settings. The API Discovery product, for example, allows automated identification and cataloging of API endpoints in traffic flowing through Fastly services.

**Human URL:** [https://www.fastly.com/documentation/reference/api/products/](https://www.fastly.com/documentation/reference/api/products/)


#### Tags:

 - Products, Features, Configuration, Platform

#### Properties

- [Documentation](https://www.fastly.com/documentation/reference/api/products/)

## Common Properties

- [Developer Portal](https://developer.fastly.com/)
- [Documentation](https://www.fastly.com/documentation/)
- [API Reference](https://www.fastly.com/documentation/reference/api/)
- [Website](https://www.fastly.com/)
- [PrivacyPolicy](https://www.fastly.com/privacy/)
- [TermsOfService](https://www.fastly.com/terms/)
- [Blog](https://www.fastly.com/blog/)
- [Login](https://manage.fastly.com/account/company)
- [Support](https://support.fastly.com/)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
