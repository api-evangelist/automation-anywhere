# automation-anywhere (automation-anywhere)

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

Automation Anywhere is an enterprise robotic process automation (RPA) platform that enables organizations to automate business processes using software bots. Their developer platform, centered around the Automation 360 Control Room, provides a comprehensive suite of REST APIs for managing bot deployment, workload queues, credentials, repositories, and analytics, as well as an SDK for building custom action packages.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/apis.yml)

## Timestamps

- **Modified:** 2026-05-19

## APIs

### Automation Anywhere Control Room API

The Automation Anywhere Control Room API is a comprehensive set of RESTful APIs that enable programmatic management and administration of the Automation 360 RPA platform. It provides endpoints across multiple versioned groups covering authentication, user management, credential vault, repository management, device pools, licensing, policy management, and scheduled automations.

- **Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html)
- **Base URL:** `https://automationanywhere-be-prod.automationanywhere.com`

#### Tags

- Automation
- Bot Management
- Enterprise
- REST
- RPA

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html)
- [OpenAPI](openapi/automation-anywhere-control-room-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/automation-anywhere-control-room.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-control-room.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Automation Anywhere Bot Deploy API

The Automation Anywhere Bot Deploy API (v3/v4) enables external applications and workflows to programmatically trigger the deployment of bots to unattended Bot Runner devices. It supports deploying bots from the public workspace, specifying target devices or device pools, and passing input variables at runtime. This API is typically combined with the Authentication API to obtain a JWT token before invoking deployment endpoints.

- **Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html)
- **Base URL:** `https://automationanywhere-be-prod.automationanywhere.com`

#### Tags

- Automation
- Bot Deployment
- Enterprise
- Orchestration
- RPA

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html)
- [OpenAPI](openapi/automation-anywhere-bot-deploy-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/automation-anywhere-bot-deploy.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-bot-deploy.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/automation-anywhere-deployment-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Automation Anywhere Workload Management API

The Automation Anywhere Workload Management API provides programmatic control over work item queues used to distribute high-volume automation workloads across multiple Bot Runner devices. Developers can create and manage work item models and queues, add or update individual work items, and retrieve queue status and processing results. This API enables enterprise systems such as ERP, CRM, and BPM platforms to feed structured data into RPA queues and track processing outcomes in real time.

- **Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html)
- **Base URL:** `https://automationanywhere-be-prod.automationanywhere.com`

#### Tags

- Automation
- Queues
- RPA
- Work Items
- Workload Management

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html)
- [OpenAPI](openapi/automation-anywhere-workload-management-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/automation-anywhere-workload-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-workload-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/automation-anywhere-work-item-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Automation Anywhere Bot Insight API

The Automation Anywhere Bot Insight API exposes real-time business process analytics and operational intelligence data collected during bot execution. It allows developers to retrieve KPIs, bot run histories, performance rankings, and failure analytics from the Control Room programmatically. Results are paginated in sets of 1000 records and can be filtered by date ranges in ISO 8601 format.

- **Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html](https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html)
- **Base URL:** `https://automationanywhere-be-prod.automationanywhere.com`

#### Tags

- Analytics
- Bot Monitoring
- Business Intelligence
- Reporting
- RPA

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html)
- [OpenAPI](openapi/automation-anywhere-bot-insight-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/automation-anywhere-bot-insight.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-bot-insight.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Automation Anywhere API Task Execution API

The Automation Anywhere API Task Execution API enables developers to invoke API Tasks — a specialized type of bot designed to be called synchronously from external applications like a REST service. It generates execution URLs and tokens that allow applications to trigger a bot task, pass input parameters, and receive output values in a single request-response cycle.

- **Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html)
- **Base URL:** `https://automationanywhere-be-prod.automationanywhere.com`

#### Tags

- API Task
- Automation
- Bot Execution
- Integration
- RPA

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html)
- [OpenAPI](openapi/automation-anywhere-api-task-execution-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/automation-anywhere-api-task-execution.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-api-task-execution.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Automation Anywhere Credential Vault API

The Automation Anywhere Credential Vault API provides programmatic access to the Control Room's centralized secrets management system. It supports creating, reading, updating, and deleting credentials, credential attributes, Lockers, and Locker Keys used by bots during execution. Credentials stored in the Vault are encrypted and access-controlled through role-based permissions, ensuring bots can retrieve sensitive values such as passwords and API keys without exposing them in automation scripts.

- **Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html)
- **Base URL:** `https://automationanywhere-be-prod.automationanywhere.com`

#### Tags

- Credentials
- Enterprise
- RPA
- Secrets Management
- Security

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html)
- [OpenAPI](openapi/automation-anywhere-credential-vault-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/automation-anywhere-credential-vault.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-credential-vault.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Automation Anywhere Package SDK

The Automation Anywhere Package SDK is a Java-based development toolkit that enables developers to build custom action packages and triggers for the Automation 360 bot editor. Developers use the SDK in a Java IDE to implement custom actions, compile the code into a JAR file, and upload the resulting package to the Control Room for use in bot workflows.

- **Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html)
- **Base URL:** `https://api.example.com`

#### Tags

- Bot Development
- Custom Packages
- Extensions
- Java
- SDK

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html)
- [Postman Collection](collections/automation-anywhere-api-task-execution.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-api-task-execution.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/automation-anywhere-bot-deploy.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-bot-deploy.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/automation-anywhere-bot-insight.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-bot-insight.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/automation-anywhere-control-room.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-control-room.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/automation-anywhere-credential-vault.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-credential-vault.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/automation-anywhere-repository-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-repository-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/automation-anywhere-workload-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-workload-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Automation Anywhere Repository Management API

The Automation Anywhere Repository Management API provides programmatic access to the Control Room's bot and file repository. It allows developers and administrators to list, search, upload, and manage bots, folders, and dependent files stored in both the public and private workspaces. This API supports bot lifecycle management use cases including automated promotion of bots between environments, bulk file operations, and integration with source control systems.

- **Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html)
- **Base URL:** `https://automationanywhere-be-prod.automationanywhere.com`

#### Tags

- Bot Lifecycle
- DevOps
- File Management
- Repository
- RPA

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html)
- [OpenAPI](openapi/automation-anywhere-repository-management-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/automation-anywhere-repository-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/automation-anywhere-repository-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/automation-anywhere-bot-schema.json) — [JSON Schema](https://json-schema.org/specification)

## Common Properties

- [GitHub Organization](https://github.com/AutomationAnywhere)
- [LinkedIn](https://www.linkedin.com/company/automation-anywhere)
- [Portal](https://developer.automationanywhere.com)
- [Website](https://www.automationanywhere.com)
- [Documentation](https://docs.automationanywhere.com)
- [Authentication](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-authentication.html)
- [Terms of Service](https://www.automationanywhere.com/legal/terms)
- [Privacy Policy](https://www.automationanywhere.com/legal/privacy-policy)
- [Support](https://support.automationanywhere.com)
- [Blog](https://www.automationanywhere.com/blog)
- [JSON-LD](json-ld/automation-anywhere-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/automation-anywhere-bot-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/automation-anywhere-deployment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/automation-anywhere-work-item-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Integrations](https://www.automationanywhere.com/integrations)
