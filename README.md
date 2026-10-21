# Awesome-Enterprise-Search

# Top Enterprise Search Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Workplace Knowledge Discovery, RAG-Powered Answers & Self-Hosted Search Infrastructure*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Enterprise Search**. These tools enable organizations to unify search across internal documents, SaaS applications, and knowledge bases—increasingly augmented with LLMs to deliver direct answers with citations rather than just links.

**Examples** include Glean, Coveo, Sinequa, Lucidworks Fusion, Elastic Enterprise Search, Algolia, Amazon Kendra, Google Cloud Search, AlphaSense, and Hebbia (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom connector development, and transparent search infrastructure—ideal for organizations that prioritize data sovereignty and avoid per-query or per-seat pricing. The open-source enterprise search landscape is anchored by **Onyx (formerly Danswer)** for AI-powered workplace Q&A, **Meilisearch** and **Typesense** for fast application search, and **Turing ES** for full RAG platforms, with **Fess** and **SeekStorm** serving specialized enterprise and performance-focused use cases.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Glean](https://www.glean.com/)**  
  Leading AI-powered workplace assistant that indexes connected SaaS systems and delivers grounded answers with citations. Connector-based deployments typically reach pilot in 2 to 6 weeks . Strong permission fidelity across indexed sources.

- **[Coveo](https://www.coveo.com/)**  
  AI-powered relevance platform serving both customer and employee experiences. Offers hybrid search combining keyword, vector, and generative answers. Custom pricing based on user count, connector scope, and indexed volume .

- **[Sinequa](https://www.sinequa.com/)**  
  Enterprise search and insight engine with deep governance and retrieval breadth. Positioned for organizations where compliance and entitlement controls are primary requirements .

- **[Lucidworks Fusion](https://lucidworks.com/)**  
  Search platform built on Apache Solr with strong engineering control over ranking, entitlements, and business rules. Suited for complex search programs requiring detailed customization .

- **[Elastic Enterprise Search](https://www.elastic.co/enterprise-search)**  
  Commercial offering built on Elasticsearch, the world's most downloaded vector database. Forrester Wave Leader for Cognitive Search Q4 2025, recognized for hybrid search, multimodal capabilities, and scaling from laptop to hundreds of nodes .

- **[Algolia](https://www.algolia.com/)**  
  Search-as-a-service API optimized for speed and developer experience. Best for application search (e-commerce, SaaS) rather than internal workplace knowledge discovery.

- **[Amazon Kendra](https://aws.amazon.com/kendra/)**  
  AWS's ML-powered enterprise search service with connectors to common repositories. Integrates with other AWS services but less flexible for non-AWS environments.

- **[Google Cloud Search](https://cloud.google.com/search)**  
  Google Workspace's native enterprise search, indexing Drive, Gmail, Calendar, and other Workspace content. Best for organizations standardized on Google Workspace.

- **[AlphaSense](https://www.alpha-sense.com/)**  
  Market intelligence and search platform focused on financial research, earnings calls, and expert content. Specialized vertical rather than general enterprise search.

- **[Hebbia](https://www.hebbia.ai/)**  
  AI-powered research and document analysis platform for financial and legal professionals. Specializes in extracting insights from large document sets.

## Open-Source GitHub Projects

- **[Onyx (formerly Danswer)](https://github.com/onyx-dot-app/onyx)**  
  The leading open-source Gen-AI + enterprise search platform. Connects to 40+ workplace tools (Google Drive, Slack, Confluence, SharePoint, Salesforce, GitHub, Jira, and more) and provides a Chat interface backed by any LLM. Features hybrid search (BM25 + embedding models), document-level access control, custom AI assistants, and Slack integration. Deployable on a laptop via Docker Compose or at scale on Kubernetes. Community Edition is MIT licensed; Enterprise adds SSO, RBAC, and analytics . Best for teams that want a self-hosted ChatGPT-like assistant over private company knowledge.

- **[Meilisearch](https://github.com/meilisearch/meilisearch)**  
  Lightning-fast, typo-tolerant search engine API with AI-powered hybrid search. 53k+ stars, MIT licensed. Zero-configuration deployment with sub-50ms response times. Supports semantic search, multi-modal search, geo-search, and federated search across multiple sources . Best for application search where speed and ease of use matter most.

- **[Typesense](https://github.com/typesense/typesense)**  
  Open-source alternative to Algolia + Pinecone and a more approachable alternative to Elasticsearch. 24k+ stars, GPL-3.0 licensed. In-memory fuzzy search with typo tolerance, designed for delightful search experiences . Best for developers who want Algolia-like DX without the hosting bill.

- **[Turing ES (Viglet)](https://github.com/openviglet/turing-ce)**  
  Open-source enterprise search + generative AI platform. Apache 2.0 licensed. Features faceted semantic search, hybrid BM25 + kNN ranking with Reciprocal Rank Fusion, RAG chat with inline citations, AI agents with MCP tools, and multi-engine support (Apache Solr, Elasticsearch, embedded Lucene). Connectors via Viglet Dumont for Adobe AEM, WordPress, databases, and filesystem. Runs fully offline for air-gapped deployments . Best for organizations that need a complete, self-hosted RAG platform with no per-query metering.

- **[Fess](https://github.com/codelibs/fess)**  
  Very powerful and easily deployable Enterprise Search Server. 1,000+ stars, Apache 2.0 licensed. Built on Elasticsearch with crawlers for web, file systems, and databases. Supports role-based search, LDAP/AD integration, and multi-language content . Best for traditional enterprise search deployments with structured crawl requirements.

- **[SeekStorm](https://github.com/SeekStorm/SeekStorm)**  
  Sub-millisecond full-text search library and multi-tenancy server written in Rust. 1,700+ stars. Designed for extreme performance and low resource usage . Best for latency-critical search workloads where Rust's performance advantages matter.

- **[Coco AI (Infinilabs)](https://github.com/infinilabs/coco-app)**  
  Search, connect, collaborate, and personal AI assistant in one space. 560+ stars . Best for teams exploring an integrated search + AI assistant experience.

### Additional Strong Open-Source Options

- **Gerev** — AI-powered enterprise search engine (2,800+ stars), though last updated in 2023 . Best for reference or legacy deployments.
- **PragmaSearch** — Local-first semantic search engine, an Algolia alternative for small-to-mid catalogs (≤50k items). Hybrid vector + BM25, $0 per search, self-hosted on a $5 VPS . Best for small teams that want semantic search without hosted costs.
- **Elasticsearch** — The foundational open-source search and analytics engine. While the commercial Enterprise Search offering is SaaS, the core engine remains Apache 2.0 licensed and powers many of the tools above.
- **Frameworks for building custom systems**: Pair **Onyx** for workplace Q&A with **Meilisearch** for fast application search. Use **Turing ES** when full RAG with citations and air-gapped deployment are required. For pure performance, **SeekStorm** or **Typesense** provide sub-50ms search without the operational overhead of Elasticsearch.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Enterprise search deployments vary significantly in connector complexity, permission mapping, and LLM integration requirements; evaluate based on your existing tool stack.
- Self-hosted solutions require proper authentication setup, connector maintenance, and index management.

---

**Made for IT leaders, knowledge managers, developers, and organizations building private, AI-augmented search infrastructure.**  
Let's make enterprise search more open, answer-driven, and accessible.
