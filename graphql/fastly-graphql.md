# Fastly GraphQL Schema

## Overview

This conceptual GraphQL schema represents the Fastly edge cloud platform API surface. Fastly does not currently expose a native GraphQL endpoint; this schema is a structured representation of the REST API resources available at https://developer.fastly.com/reference/api/ translated into GraphQL types and operations.

The schema covers the full breadth of Fastly's platform: CDN services and versioning, backend and origin management, VCL configuration, edge dictionaries, ACLs, TLS certificate management, real-time logging endpoints, metrics and statistics, WAF and security, compute, and account/token management.

## Schema Source

- Provider: Fastly
- REST API Reference: https://www.fastly.com/documentation/reference/api/
- GitHub Organization: https://github.com/fastly
- Schema Type: Conceptual GraphQL (derived from REST API)
- Schema File: fastly-schema.graphql

## Type Categories

### Service Management
- `Service` — top-level CDN service configuration unit
- `ServiceVersion` — immutable, activatable snapshot of a service configuration
- `ServiceDetail` — extended service metadata with version list

### Networking and Routing
- `Domain` — hostname mapped to a Fastly service version
- `Backend` — origin server or upstream target for a service
- `Director` — load balancing group over multiple backends
- `DirectorBackend` — backend membership in a director
- `OriginPool` — pool of origin servers for dynamic load balancing
- `OriginPoolMember` — individual server within an origin pool

### Cache Control
- `CacheRule` — cache TTL and behavior override rule (cache settings)
- `Condition` — logical expression gating rule application
- `Header` — request or response header manipulation rule
- `RequestSetting` — override for request-handling properties (force SSL, max stale age, etc.)
- `ResponseObject` — synthetic HTTP response returned at the edge
- `GZIPConfig` — gzip compression configuration for response types

### VCL and Edge Logic
- `VCLFile` — complete custom VCL program uploaded to a service version
- `Snippet` — reusable VCL snippet inserted at a specific subroutine
- `Healthcheck` — health probe configuration for a backend

### Access Control
- `ACL` — named IP access control list container attached to a service version
- `ACLEntry` — individual IP or CIDR entry within an ACL
- `ACLPermission` — permission metadata for ACL operations

### Edge Dictionaries
- `EdgeDictionary` — key-value store accessible in VCL without version lock
- `DictionaryItem` — individual key-value pair within an edge dictionary
- `DictionaryInfo` — metadata and digest for a dictionary's current state

### Logging Endpoints
- `LogEndpoint` — abstract logging destination interface
- `S3Logging` — Amazon S3 log streaming endpoint
- `GCSLogging` — Google Cloud Storage log streaming endpoint
- `BigQueryLogging` — Google BigQuery log streaming endpoint
- `SplunkLogging` — Splunk HEC log streaming endpoint
- `NewRelicLogging` — New Relic log streaming endpoint
- `DatadogLogging` — Datadog log streaming endpoint
- `PapertrailLogging` — Papertrail log streaming endpoint
- `HTTPLogging` — generic HTTPS log streaming endpoint
- `SFTPLogging` — SFTP log streaming endpoint
- `SyslogLogging` — syslog log streaming endpoint
- `SumoLogicLogging` — Sumo Logic log streaming endpoint
- `LogglyLogging` — Loggly log streaming endpoint
- `ElasticsearchLogging` — Elasticsearch log streaming endpoint

### TLS and Certificates
- `TLSCertificate` — custom TLS certificate uploaded by customer
- `TLSPrivateKey` — TLS private key associated with a certificate
- `TLSDomain` — domain configured for TLS termination
- `TLSSubscription` — platform-managed TLS certificate subscription
- `TLSActivation` — binding of a certificate to a domain on a configuration
- `CustomTLSConfig` — custom TLS configuration object

### Purging
- `Purge` — result of a single-URL or surrogate-key cache purge operation
- `Batch` — batch operation result for bulk cache invalidation

### Metrics and Statistics
- `Stats` — aggregated service-level traffic statistics
- `Historical` — historical analytics data over a time range
- `Realtime` — second-resolution real-time analytics data
- `DomainInspector` — per-domain metrics breakdown
- `OriginInspector` — per-origin performance metrics

### Security
- `WAF` — Web Application Firewall configuration attached to a service
- `WAFRuleExclusion` — exclusion rule suppressing a WAF signal
- `RateLimiter` — edge rate limiting rule configuration
- `IPFilter` — IP filtering rule at the service level
- `NGWAFWorkspace` — Next-Gen WAF (Signal Sciences) workspace
- `NGWAFRule` — signal-based rule within a Next-Gen WAF workspace
- `NGWAFEvent` — WAF event record captured by the Next-Gen WAF
- `DDoSEvent` — DDoS protection event record
- `DDoSRule` — mitigation rule associated with a DDoS event

### Account and Authentication
- `User` — Fastly account user with role and permissions
- `APIToken` — API authentication token scoped to services and permissions
- `Customer` — Fastly customer account metadata
- `ServiceGroup` — IAM group organizing services for role-based access

### Compute
- `ComputePackage` — Wasm package deployed to the Fastly Compute platform
- `KVStore` — key-value store accessible from Compute services
- `KVStoreItem` — individual key-value pair in a KV store
- `ConfigStore` — read-only config store for Compute services
- `SecretStore` — encrypted secret store for Compute services

### Utilities
- `POPLocation` — Fastly point-of-presence location with region and coordinates
- `PublicIPRange` — public IP CIDR block assigned to Fastly infrastructure

## Query Operations

- `service(id: ID!)` — fetch a single service by ID
- `services` — list all services for the authenticated customer
- `serviceVersion(serviceId: ID!, version: Int!)` — fetch a specific service version
- `backend(serviceId: ID!, version: Int!, name: String!)` — fetch a backend
- `backends(serviceId: ID!, version: Int!)` — list backends on a version
- `domain(serviceId: ID!, version: Int!, name: String!)` — fetch a domain
- `domains(serviceId: ID!, version: Int!)` — list domains on a version
- `acl(serviceId: ID!, version: Int!, name: String!)` — fetch an ACL
- `aclEntries(serviceId: ID!, aclId: ID!)` — list ACL entries
- `dictionary(serviceId: ID!, version: Int!, name: String!)` — fetch a dictionary
- `dictionaryItems(serviceId: ID!, dictionaryId: ID!)` — list dictionary items
- `tlsCertificates` — list uploaded TLS certificates
- `tlsSubscriptions` — list platform TLS subscriptions
- `stats(serviceId: ID!, from: String!, to: String!)` — fetch historical stats
- `realtime(serviceId: ID!)` — fetch real-time analytics
- `user(id: ID!)` — fetch a user account
- `tokens` — list API tokens for the current user
- `pops` — list Fastly points of presence

## Mutation Operations

- `createService` — create a new CDN service
- `cloneServiceVersion` — clone an existing service version into a draft
- `activateServiceVersion` — activate a draft version into production
- `createBackend` — add a backend to a service version
- `updateBackend` — modify backend settings
- `deleteBackend` — remove a backend
- `createDomain` — add a domain to a service version
- `deleteDomain` — remove a domain
- `createACL` — create an ACL container
- `createACLEntry` — add an IP entry to an ACL
- `bulkUpdateACLEntries` — batch create/update/delete ACL entries
- `createDictionary` — create an edge dictionary
- `upsertDictionaryItem` — set a key-value pair in a dictionary
- `bulkUpdateDictionaryItems` — batch update dictionary items
- `uploadVCL` — upload a custom VCL file
- `createSnippet` — add a VCL snippet
- `purgeURL` — purge a single URL from cache
- `purgeSurrogateKey` — purge all objects with a surrogate key tag
- `purgeAll` — purge all cached content for a service
- `uploadTLSCertificate` — upload a custom TLS certificate
- `createTLSActivation` — activate TLS for a domain
- `createToken` — create an API authentication token
- `revokeToken` — revoke an API token
- `createUser` — invite a new user to the account
