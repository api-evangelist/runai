# NVIDIA Run:ai

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

NVIDIA Run:ai (formerly run.ai) is an AI operations and GPU orchestration platform for Kubernetes that pools, schedules, and governs GPU compute across clusters for training, fine-tuning, and inference workloads. It provides fractional GPU sharing, dynamic scheduling, quota and policy management, multi-tenant projects and departments, and workload lifecycle control across SaaS, self-hosted, and multi-tenant deployments. run.ai was founded in Israel, backed by Insight Partners and other investors, and acquired by NVIDIA in 2024; the product is now delivered as NVIDIA Run:ai. Its control-plane REST API exposes programmatic management of clusters, node pools, projects, departments, workloads (workspaces, trainings, inferences, distributed), assets, policies, permissions, service accounts, and audit logs, authenticated with bearer JWT access tokens obtained from client-credentials access keys.

**Areas:** Company · Artificial Intelligence · GPU · Machine Learning · Kubernetes · MLOps · Compute · Scheduling · Infrastructure · Container Orchestration

## NVIDIA Run:ai on APIs.io

Everything profiled for NVIDIA Run:ai is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/runai/](https://apis.io/providers/runai/)** — or go straight to one of the APIs or properties below.

### APIs (62)

- [NVIDIA Run:ai Access Keys API](https://apis.io/apis/runai/runai-access-keys-api/) — Access Keys allow users to authenticate and interact programmatically with the NVIDIA Run:ai API. Each access key consists of a client ID and secret that…
- [NVIDIA Run:ai Access rules API](https://apis.io/apis/runai/runai-access-rules-api/) — Access rules provide user authorization to system resources and entities. It is managed using Role-based access control (RBAC) which is a policy-neutral…
- [NVIDIA Run:ai Administrator Command Line Interface API](https://apis.io/apis/runai/runai-administrator-command-line-interface-api/) — Information specific to the Administrator Command Line Interface.
- [NVIDIA Run:ai AI Applications API](https://apis.io/apis/runai/runai-ai-applications-api/) — AI Applications.
- [NVIDIA Run:ai Applications API](https://apis.io/apis/runai/runai-applications-api/) — **DEPRECATED:** Applications have been renamed to Service Accounts. Please use the [Service Accounts](/latest/#tag/Service-Accounts) endpoints instead.…
- [NVIDIA Run:ai Clusters API](https://apis.io/apis/runai/runai-clusters-api/) — Use these endpoints to create, manage and delete NVIDIA Run:ai Kubernetes clusters.
- [NVIDIA Run:ai Compute API](https://apis.io/apis/runai/runai-compute-api/) — A compute resource is a building block that represents compute resources such as GPUs, CPU cores, and CPU memory. The compute resources may consist of…
- [NVIDIA Run:ai ConfigMap API](https://apis.io/apis/runai/runai-configmap-api/) — Use a ConfigMap as a data source location for data sets that are relevant to the workload being submitted.
- [NVIDIA Run:ai Credentials API](https://apis.io/apis/runai/runai-credentials-api/) — Credentials are used to unlock protected resources such as applications, containers, and other assets. For more information, see…
- [NVIDIA Run:ai Departments API](https://apis.io/apis/runai/runai-departments-api/) — Departments, in the hierarchy of resource allocation, are above Projects. A Department can contain multiple Projects, and has its own quotas. A Department's…
- [NVIDIA Run:ai Distributed API](https://apis.io/apis/runai/runai-distributed-api/) — Distributed Training, is the ability to split the training of a model among multiple processors. It is often a necessity when multi-GPU training no longer…
- [NVIDIA Run:ai Distributed Inferences API](https://apis.io/apis/runai/runai-distributed-inferences-api/) — Distributed inference enables running inference workloads across multiple pods, typically to scale model serving beyond a single container or node. This…
- [NVIDIA Run:ai Environment API](https://apis.io/apis/runai/runai-environment-api/) — An environment resource designates the container image, the image pull policy, working directory, security parameters, and others. It exposes all the…
- [NVIDIA Run:ai Events API](https://apis.io/apis/runai/runai-events-api/) — Workload events that occurred while the workload was running. Use to diagnose issue around workload scheduling.
- [NVIDIA Run:ai Git API](https://apis.io/apis/runai/runai-git-api/) — Use Git as a data source location for data sets that are relevant to the workload being submitted.
- [NVIDIA Run:ai HostPath API](https://apis.io/apis/runai/runai-hostpath-api/) — Use a HostPath as a data source location for data sets that are relevant to the workload being submitted.
- [NVIDIA Run:ai Idps API](https://apis.io/apis/runai/runai-idps-api/) — The Idps API from NVIDIA Run:ai — 3 operation(s) for idps.
- [NVIDIA Run:ai Inferences API](https://apis.io/apis/runai/runai-inferences-api/) — Inference workloads deploy trained models into a production environment to generate predictions from live data. These workloads are prioritized over…
- [NVIDIA Run:ai Logo API](https://apis.io/apis/runai/runai-logo-api/) — Use to manage tenant logo files.
- [NVIDIA Run:ai Me API](https://apis.io/apis/runai/runai-me-api/) — "Me" returns the authenticated user's permissions within the system. It provides a comprehensive view of access rules (roles, subjects and scope) assigned…
- [NVIDIA Run:ai Network Topologies API](https://apis.io/apis/runai/runai-network-topologies-api/) — The Network Topologies API enables administrators to reflect the hierarchical network topology connectivity of nodes in a data center, such as racks,…
- [NVIDIA Run:ai NFS API](https://apis.io/apis/runai/runai-nfs-api/) — Use NFS as a data source location for data sets that are relevant to the workload being submitted.
- [NVIDIA Run:ai Nodes API](https://apis.io/apis/runai/runai-nodes-api/) — Nodes are worker machines in Kubernetes and may be either a virtual or a physical machine, depending on the cluster. Each Node is managed by the NVIDIA…
- [NVIDIA Run:ai Notification State API](https://apis.io/apis/runai/runai-notification-state-api/) — Use to manage notification state.
- [NVIDIA Run:ai Notification Types API](https://apis.io/apis/runai/runai-notification-types-api/) — Use to get notification types.
- [NVIDIA Run:ai NVIDIA NIM API](https://apis.io/apis/runai/runai-nvidia-nim-api/) — The NVIDIA NIM API provides endpoints to create and manage workloads that deploy NVIDIA Inference Microservices (NIM) through the NIM Operator. These…
- [NVIDIA Run:ai Org unit API](https://apis.io/apis/runai/runai-org-unit-api/) — Org unit.
- [NVIDIA Run:ai Permissions API](https://apis.io/apis/runai/runai-permissions-api/) — The Permissions API from NVIDIA Run:ai — 2 operation(s) for permissions.
- [NVIDIA Run:ai Pods API](https://apis.io/apis/runai/runai-pods-api/) — Retrieve data about workload pods from your NVIDIA Run:ai platform.
- [NVIDIA Run:ai Policy API](https://apis.io/apis/runai/runai-policy-api/) — Policies allow administrators to impose restrictions and set default values for researcher workloads. Restrictions and default values can be placed on CPUs,…
- [NVIDIA Run:ai Projects API](https://apis.io/apis/runai/runai-projects-api/) — Projects implement resource allocation policies and create segregation between different initiatives. It can represent a team, an individual, or an…
- [NVIDIA Run:ai PVC API](https://apis.io/apis/runai/runai-pvc-api/) — Use a PVC as a data source location for data sets that are relevant to the workload being submitted.
- [NVIDIA Run:ai Registry API](https://apis.io/apis/runai/runai-registry-api/) — Use an images registry to enable the listting of repositories and tags that can be used as a data source location for data sets that are relevant to the…
- [NVIDIA Run:ai Reports API](https://apis.io/apis/runai/runai-reports-api/) — The Reports API from NVIDIA Run:ai — 5 operation(s) for reports.
- [NVIDIA Run:ai Researcher Command Line Interface API](https://apis.io/apis/runai/runai-researcher-command-line-interface-api/) — The Researcher Command Line Interface API from NVIDIA Run:ai — 9 operation(s) for researcher command line interface.
- [NVIDIA Run:ai Researcher Command Line Interface Deprecated API](https://apis.io/apis/runai/runai-researcher-command-line-interface-deprecated-api/) — The Researcher Command Line Interface Deprecated API from NVIDIA Run:ai — 9 operation(s) for researcher command line interface deprecated.
- [NVIDIA Run:ai Revisions API](https://apis.io/apis/runai/runai-revisions-api/) — Revisions are associated with an inference workload and represent a snapshot of its configuration. A revision is created on each change to the inference…
- [NVIDIA Run:ai Roles API](https://apis.io/apis/runai/runai-roles-api/) — A role is a group of permissions that can be granted. Permissions are a set of actions that can be applied to entities. For more information, see…
- [NVIDIA Run:ai S3 API](https://apis.io/apis/runai/runai-s3-api/) — Use an S3 simple storage service as a data source location for data sets that are relevant to the workload being submitted.
- [NVIDIA Run:ai Secret API](https://apis.io/apis/runai/runai-secret-api/) — Use a credentials as a data source location for data sets that are relevant to the workload being submitted.
- [NVIDIA Run:ai Service Accounts API](https://apis.io/apis/runai/runai-service-accounts-api/) — Service accounts enable programmatic access to the NVIDIA Run:ai API, allowing applications or automated systems to authenticate and interact securely. Each…
- [NVIDIA Run:ai Settings API](https://apis.io/apis/runai/runai-settings-api/) — View and manage configuration settings for your organization.
- [NVIDIA Run:ai Storage Class Configuration API](https://apis.io/apis/runai/runai-storage-class-configuration-api/) — The storage class configuration API enables administrators to define, manage, and customize how storage classes are used across the NVIDIA Run:ai platform.…
- [NVIDIA Run:ai Storage Classes API](https://apis.io/apis/runai/runai-storage-classes-api/) — The Storage Classes API retrieves a list of available, pre-defined storage classes in the system.
- [NVIDIA Run:ai Subscriptions API](https://apis.io/apis/runai/runai-subscriptions-api/) — Use to manage notifications subscriptions.
- [NVIDIA Run:ai Template API](https://apis.io/apis/runai/runai-template-api/) — Templates are a pre-set configuration used to quickly configure and submit workloads using existing assets.
- [NVIDIA Run:ai Tenant API](https://apis.io/apis/runai/runai-tenant-api/) — Manage tenant settings.
- [NVIDIA Run:ai Tokens API](https://apis.io/apis/runai/runai-tokens-api/) — Use tokens to facilitate authentication to the NVIDIA Run:ai API. The API server must be configured to use the NVIDIA Run:ai identity service to validate…
- [NVIDIA Run:ai Trainings API](https://apis.io/apis/runai/runai-trainings-api/) — Trainings are dedicated workloads that are specifically used for training models. They are by design preemptible workloads because they are used in…
- [NVIDIA Run:ai User Applications API](https://apis.io/apis/runai/runai-user-applications-api/) — **DEPRECATED:** User Applications have been renamed to Access Keys. Please use the [Access Keys](/latest/#tag/Access-Keys) endpoints instead. User…
- [NVIDIA Run:ai Users API](https://apis.io/apis/runai/runai-users-api/) — The Users API from NVIDIA Run:ai — 6 operation(s) for users.
- [NVIDIA Run:ai Workload properties API](https://apis.io/apis/runai/runai-workload-properties-api/) — Workload properties define the behavioral and scheduling characteristics of a workload submitted to the NVIDIA Run:ai platform. These properties such as…
- [NVIDIA Run:ai Workload templates API](https://apis.io/apis/runai/runai-workload-templates-api/) — This set of endpoints manages workload templates used to define reusable workload configurations across various workload types in the NVIDIA Run:ai…
- [NVIDIA Run:ai Workloads API](https://apis.io/apis/runai/runai-workloads-api/) — Workloads are both native platform workloads, Workspaces, Training and Inference, as well as workloads that originate from third-party ML frameworks, tools,…
- [NVIDIA Run:ai Workloads batch API](https://apis.io/apis/runai/runai-workloads-batch-api/) — The Workloads batch API from NVIDIA Run:ai — 1 operation(s) for workloads batch.
- [NVIDIA Run:ai Workloads V2 API](https://apis.io/apis/runai/runai-workloads-v2-api/) — The Workloads V2 API allows you to create, retrieve, and delete workloads that originate from third-party ML frameworks, tools, or the broader Kubernetes…
- [NVIDIA Run:ai Workspaces API](https://apis.io/apis/runai/runai-workspaces-api/) — A Workspace is a simplified tool for researchers to conduct experiments, build AI models, access standard MLOps tools, and collaborate with their peers.…
- [NVIDIA Run:ai Audit Logs API](https://apis.io/apis/runai/runai-audit-logs-api/) — The audit log provides audit trail information for user activity, changes to business objects and other important information. For more information, see…
- [NVIDIA Run:ai Data Sources API](https://apis.io/apis/runai/runai-data-sources-api/) — Data source assets.
- [NVIDIA Run:ai Data Volumes API](https://apis.io/apis/runai/runai-data-volumes-api/) — The Data Volumes API from NVIDIA Run:ai — 5 operation(s) for data volumes.
- [NVIDIA Run:ai Node Pools API](https://apis.io/apis/runai/runai-node-pools-api/) — Node pools assist in managing heterogeneous resources effectively. A node pool is a set of nodes grouped into a bucket of resources using a predefined (for…
- [NVIDIA Run:ai Notification Channels API](https://apis.io/apis/runai/runai-notification-channels-api/) — Notification Channels are the medium through which notifications are sent.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [runai](https://apis.io/servers/runai/runai/)

#### Collections (62)

Postman and Open Collection request collections.

- [NVIDIA Run:ai Access Keys API](https://apis.io/collections/runai/open-runai-access-keys-api/)
- [NVIDIA Run:ai Access Keys Access rules API](https://apis.io/collections/runai/open-runai-access-rules-api/)
- [NVIDIA Run:ai Access Keys Administrator Command Line Interface API](https://apis.io/collections/runai/open-runai-administrator-command-line-interface-api/)
- [NVIDIA Run:ai Access Keys AI Applications API](https://apis.io/collections/runai/open-runai-ai-applications-api/)
- [NVIDIA Run:ai Access Keys Applications API](https://apis.io/collections/runai/open-runai-applications-api/)
- [NVIDIA Run:ai Access Keys Audit Logs API](https://apis.io/collections/runai/open-runai-auditlogs-api/)
- [NVIDIA Run:ai Access Keys Clusters API](https://apis.io/collections/runai/open-runai-clusters-api/)
- [NVIDIA Run:ai Access Keys Compute API](https://apis.io/collections/runai/open-runai-compute-api/)
- [NVIDIA Run:ai Access Keys Config Map API](https://apis.io/collections/runai/open-runai-configmap-api/)
- [NVIDIA Run:ai Access Keys Credentials API](https://apis.io/collections/runai/open-runai-credentials-api/)
- [NVIDIA Run:ai Access Keys Datasources API](https://apis.io/collections/runai/open-runai-datasources-api/)
- [NVIDIA Run:ai Access Keys Datavolumes API](https://apis.io/collections/runai/open-runai-datavolumes-api/)
- [NVIDIA Run:ai Access Keys Departments API](https://apis.io/collections/runai/open-runai-departments-api/)
- [NVIDIA Run:ai Access Keys Distributed API](https://apis.io/collections/runai/open-runai-distributed-api/)
- [NVIDIA Run:ai Access Keys Distributed Inferences API](https://apis.io/collections/runai/open-runai-distributed-inferences-api/)
- [NVIDIA Run:ai Access Keys Environment API](https://apis.io/collections/runai/open-runai-environment-api/)
- [NVIDIA Run:ai Access Keys Events API](https://apis.io/collections/runai/open-runai-events-api/)
- [NVIDIA Run:ai Access Keys Git API](https://apis.io/collections/runai/open-runai-git-api/)
- [NVIDIA Run:ai Access Keys Host Path API](https://apis.io/collections/runai/open-runai-hostpath-api/)
- [NVIDIA Run:ai Access Keys Idps API](https://apis.io/collections/runai/open-runai-idps-api/)
- [NVIDIA Run:ai Access Keys Inferences API](https://apis.io/collections/runai/open-runai-inferences-api/)
- [NVIDIA Run:ai Access Keys Logo API](https://apis.io/collections/runai/open-runai-logo-api/)
- [NVIDIA Run:ai Access Keys Me API](https://apis.io/collections/runai/open-runai-me-api/)
- [NVIDIA Run:ai Access Keys Network Topologies API](https://apis.io/collections/runai/open-runai-network-topologies-api/)
- [NVIDIA Run:ai Access Keys NFS API](https://apis.io/collections/runai/open-runai-nfs-api/)
- …and 37 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Runai Openapi Overlay](https://apis.io/overlays/runai/runai-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Runai Authentication](https://apis.io/security/runai/runai-authentication/)
- [Runai Domain Security](https://apis.io/security/runai/runai-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.nvidia.com/en-us/software/run-ai/)
- [Documentation](https://run-ai-docs.nvidia.com/)
- [Getting started](https://run-ai-docs.nvidia.com/saas/getting-started/quick-starts.md)
- [API reference](https://run-ai-docs.nvidia.com/api/readme.md)
- [Terms of service](https://www.nvidia.com/en-us/about-nvidia/terms-of-service/)
- [Privacy policy](https://www.nvidia.com/en-us/about-nvidia/privacy-policy/)
- [GitHub](https://github.com/run-ai)

## API Evangelist rating

**Kin Score 43.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 52.5 |
| Contract governance | 4.5 |
| Operational transparency | 26.3 |
| Developer ergonomics | 66.1 |
| Access clarity | 27.6 |

**Agent readiness 27.0** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | yes |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | mostly (partial credit) |

**Regulatory alignment 22.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/runai/](https://apis.io/providers/runai/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for NVIDIA Run:ai: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/runai/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
