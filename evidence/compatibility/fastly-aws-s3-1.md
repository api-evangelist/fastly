<!-- fetched 2026-10-13 from https://docs.fastly.com/products/object-storage by sweep-shape-compat.py; text extracted from the provider's own page -->

Object Storage | Fastly Products 
 Guides Network services
 Customize your content delivery.
 Full-Site Delivery (CDN)
 Streaming Delivery
 Purging
 Image Optimizer
 Security
 Protect your services and applications.
 Next-Gen WAF
 Edge Rate Limiting
 Access Control Lists
 TLS
 Compute
 Experiment with Fastly's edge computing platform.
 Compute services
 Testing and debugging
 Edge Data Storage
 Quick start
 Go from zero to Fastly with these step-by-step guides and tutorials.
 CDN getting started guide
 Compute getting started guide
 Building blocks
 Start with the basics and learn how Fastly lets you take advantage of the modern internet.
 Services
 Core concepts
 Web interface guides
 Integrations
 Find out how Fastly services interoperate with non-Fastly services.
 Streaming logs
 Logging endpoints
 Non-Fastly services
 See all guides 
 Reference VCL platform
 Compute platform
 Fastly API
 Next-Gen WAF API
 Fastly CLI
 Image Optimizer
 HTTP reference
 Tools
 Glossary
 Changelog
 Solutions Tutorials
 Step-by-step guides to developing with Fastly
 Deliver a site with Fastly
 Enhance your UX with Compute
 Edge deploy Next-Gen WAF
 See all tutorials
 Demos
 Discover how Fastly can enhance your user experience.
 Passwordless auth
 Fanout chat
 Social sharing cards
 See all demos
 Use Cases
 Get solutions to specific problems with curated topics.
 Authentication
 Geolocation
 Personalization
 See all use cases
 Code Examples
 Try out Fastly code in the browser and easily remix it for your own project.
 Geolocation at the edge
 Optimize images on the fly
 Redirect URLs at the edge
 See all code examples
 Starter Kits
 Start developing your project immediately with Fastly from a functional template.
 Rust default starter
 JavaScript default starter
 Go default starter
 See all starter kits
 Products Network services
 Security
 Observability
 Compute
 Support solutions
 Developers Developers home
 Community
 Events
 Open source
 Blog
 Labs
 Search 
 Log in Try Fastly free 
 Menu 
 Products
 Network Services Cache Reservation 
 Capacity Reservation 
 Cloud Optimizer 
 Dedicated IP addresses 
 Domain Research API 
 Fastly DNS 
 Fastly’s Full-Site Delivery 
 Fastly's On-the-Fly Packager service 
 Fastly’s Streaming Delivery 
 HIPAA-Compliant Caching and Delivery 
 Image Optimizer 
 Media Shield for Live 
 Media Shield for VOD 
 Object Storage 
 Oblivious HTTP Relay 
 Origin Connect 
 PCI-Compliant Caching and Delivery 
 Subscriber Provided Prefix 
 WebSockets 
 Security 
 Observability 
 Compute 
 Support 
 Resources 
 Platform features 
 Legacy offerings 
 Third-party information 
 Compliance 
 Security measures 
 Home 
 Products 
 Network Services 
 Object Storage
 Last updated 2026-09-08
 Fastly Object Storage is an Amazon S3-compatible large object storage solution that works seamlessly with both Deliver and Compute services. Using Fastly Object Storage, you can store larger file sizes with Fastly, improving latency, increasing cache hit ratios, and reducing egress charges. Objects stored in Fastly Object Storage are accessible via an S3 compatible interface.
 Fastly Object Storage might be useful if you want to:
 replace an existing storage solution with one that’s part of Fastly’s network.
 store data in a neutral location to be used across different vendors.
 access data at the edge to reduce overall costs.
 automatically expire data you no longer need using bucket lifecycle rules.
 Limitations and considerations
 Use of Fastly Object Storage is subject to the following limitations:
 Data is stored in containers called buckets, which are limited to 100 per region. There is no limit to the amount of data storage per bucket.
 Object keys are limited to 1024 bytes.
 Objects are limited to 5 TB per object. Object metadata is limited to 1,000 bytes per object.
 No more than 5 GB of data may be included in a single upload, but multipart upload is supported.
 The minimum size of any part of a multipart upload, except the last one, is 5 MB. The maximum number of parts in a multipart upload is 10,000.
 Uploads must complete within 120 seconds or you'll receive a 408 Request Timeout error. One way to decrease the likelihood of timeouts is to upload objects in smaller parts, making sure to meet the requirements for multipart upload above.
 Metadata set on objects using x-amz-meta- headers is limited to 1000 bytes, including the length of the header name, and must not begin with x-amz-meta-fst or x-amz-meta-fastly .
 Data accessed from public, Amazon S3-compatible endpoints are subject to a maximum speed of ~150Mbps and limited to a total of 100 requests per second per bucket. Data accessed from within Fastly’s network is not subject to these limits. If your needs exceed these limits, reach out to sales@fastly.com .
 The following limitations and considerations also apply when using the S3-compatible API with Object Storage:
 Access keys created through the control panel grant access to Fastly Object Storage at the account-level, not the bucket-level. If you want to create access keys with bucket-level access, use the Fastly API.
 Bucket names cannot start with fst or fastly .
 Public access (i.e., unauthenticated access to buckets or objects) is not supported.
 Chunked uploads are not supported. Payloads must be transferred in a single chunk per request.
 Fastly Object Storage automatically encrypts uploaded objects. Uploaded objects have ETags that aren't an MD5 digest of their object data, which may require configuration changes to S3-compatible tooling in order to interact with the objects.
 Bucket lifecycle rules support a single prefix filter per rule, a maximum of 25 rules per bucket, and a minimum expiration of 1 day. Storage class transitions are not supported.
 Billing
 Fastly Object Storage is an add-on and is priced in addition to Fastly services.
 Billing for Fastly Object Storage is based on a combination of total storage charges and data processing operations for the month. Fastly uses The International System of Units (SI Units) to measure storage. In our calculations, 1 gigabyte (GB) = 10 9 (1,000,000,000) bytes and 1 terabyte (TB) = 10 12 bytes (or 1,000 GB). Storage is calculated using GB-month, rounded to the nearest hour, and processing operations are categorized into two groups, each with differing prices:
 Class A Operations are write operations and include CreateMultipartUpload , CompleteMultipartUpload , PutObject , and UploadPart .
 Class B Operations are read operations and include GetObject and HeadObject .
 A full list of supported operations are available in our documentation .
 You will be charged for storage as long as your data is present in Fastly Object Storage. You are responsible for removing data you no longer need. Bucket lifecycle rules can automate this removal. Consider setting a spend alert for your account to automatically be notified when your month-to-date bill approaches or meets a specific dollar amount. 
 For more details about this product, contact your customer success manager or email sales@fastly.com .
 Some Fastly products can be purchased directly in the web interface on the Products page by an account Superuser or User Admin. Be sure to review all limitations, considerations, and pricing information before purchase. Alternatively, contact your customer success manager or email sales@fastly.com for product purchase or pricing information. 
 Products
 Edge Cloud Platform 
 DDoS Protection 
 Next-Gen WAF 
 Pricing 
 Try Fastly Free 
 Network Map 
 Services
 Professional Services 
 Managed CDN 
 Support Plans 
 Talk to an Expert 
 Learn
 Documentation 
 Developers 
 Resource Library 
 Blog 
 Events 
 Support
 Support Center 
 Network Status 
 Contact Us 
 Company
 About Us 
 Careers 
 Customer Stories 
 Partners 
 News 
 Investor Relations 
 Trust 
 © Fastly 2026 Archives 
 Changelog 
 Translations 
 Terms of Service 
 Policy FAQ
