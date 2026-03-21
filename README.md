# Automation Anywhere (automation-anywhere)
Automation Anywhere is an enterprise robotic process automation (RPA) platform that enables organizations to automate business processes using software bots. Their developer platform, centered around the Automation 360 Control Room, provides a comprehensive suite of REST APIs for managing bot deployment, workload queues, credentials, repositories, and analytics, as well as an SDK for building custom action packages.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - RPA, Automation, Bot Management, Enterprise, Workload, Analytics, Security, DevOps

## Timestamps

- **Created:** 2026-03-21
- **Modified:** 2026-03-21

## APIs

### Automation Anywhere Control Room API
The Automation Anywhere Control Room API is a comprehensive set of RESTful APIs that enable programmatic management and administration of the Automation 360 RPA platform. It provides endpoints across multiple versioned groups covering authentication, user management, credential vault, repository management, device pools, licensing, policy management, and scheduled automations. Developers can use these APIs to integrate Control Room operations into external applications, CI/CD pipelines, and enterprise systems. All requests require JWT-based authentication obtained through the Authentication API, and interactive API exploration is available via the Swagger UI at each Control Room instance.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html)


#### Tags:

 - RPA, Automation, Bot Management, Enterprise, REST

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html)
- [OpenAPI](openapi/automation-anywhere-control-room-openapi.yml)

### Automation Anywhere Bot Deploy API
The Automation Anywhere Bot Deploy API (v3/v4) enables external applications and workflows to programmatically trigger the deployment of bots to unattended Bot Runner devices. It supports deploying bots from the public workspace, specifying target devices or device pools, and passing input variables at runtime. This API is typically combined with the Authentication API to obtain a JWT token before invoking deployment endpoints. It is commonly used in DevOps pipelines, event-driven architectures, and third-party orchestration platforms to initiate RPA bot execution on demand.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html)


#### Tags:

 - RPA, Bot Deployment, Automation, Orchestration, Enterprise

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html)
- [OpenAPI](openapi/automation-anywhere-bot-deploy-openapi.yml)

### Automation Anywhere Workload Management API
The Automation Anywhere Workload Management API provides programmatic control over work item queues used to distribute high-volume automation workloads across multiple Bot Runner devices. Developers can create and manage work item models and queues, add or update individual work items, and retrieve queue status and processing results. This API enables enterprise systems such as ERP, CRM, and BPM platforms to feed structured data into RPA queues and track processing outcomes in real time. It is available in both v3 and v4 endpoint versions with enhanced capabilities in the latest version.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html)


#### Tags:

 - Workload Management, Queues, Work Items, RPA, Automation

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html)
- [OpenAPI](openapi/automation-anywhere-workload-management-openapi.yml)

### Automation Anywhere Bot Insight API
The Automation Anywhere Bot Insight API exposes real-time business process analytics and operational intelligence data collected during bot execution. It allows developers to retrieve KPIs, bot run histories, performance rankings, and failure analytics from the Control Room programmatically. Results are paginated in sets of 1000 records and can be filtered by date ranges in ISO 8601 format. This API is commonly used to feed bot performance data into external dashboards, BI tools such as Tableau, and data warehouses for enterprise reporting.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html](https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html)


#### Tags:

 - Analytics, Business Intelligence, Reporting, RPA, Bot Monitoring

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html)
- [OpenAPI](openapi/automation-anywhere-bot-insight-openapi.yml)

### Automation Anywhere API Task Execution API
The Automation Anywhere API Task Execution API enables developers to invoke API Tasks — a specialized type of bot designed to be called synchronously from external applications like a REST service. It generates execution URLs and tokens that allow applications to trigger a bot task, pass input parameters, and receive output values in a single request-response cycle. This pattern allows RPA automations to be exposed as callable microservices within application architectures, bridging the gap between traditional bot orchestration and API-first integration patterns.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html)


#### Tags:

 - API Task, Bot Execution, Integration, RPA, Automation

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html)
- [OpenAPI](openapi/automation-anywhere-api-task-execution-openapi.yml)

### Automation Anywhere Credential Vault API
The Automation Anywhere Credential Vault API provides programmatic access to the Control Room's centralized secrets management system. It supports creating, reading, updating, and deleting credentials, credential attributes, Lockers, and Locker Keys used by bots during execution. Credentials stored in the Vault are encrypted and access-controlled through role-based permissions, ensuring bots can retrieve sensitive values such as passwords and API keys without exposing them in automation scripts. This API is used by administrators to provision and manage bot credentials as part of enterprise security and governance workflows.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html)


#### Tags:

 - Credentials, Security, Secrets Management, RPA, Enterprise

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html)
- [OpenAPI](openapi/automation-anywhere-credential-vault-openapi.yml)

### Automation Anywhere Package SDK
The Automation Anywhere Package SDK is a Java-based development toolkit that enables developers to build custom action packages and triggers for the Automation 360 bot editor. Developers use the SDK in a Java IDE to implement custom actions, compile the code into a JAR file, and upload the resulting package to the Control Room for use in bot workflows. Custom packages extend the built-in action library to support proprietary systems, specialized data formats, or integrations not covered by pre-built connectors. Versioned SDK releases are distributed as ZIP archives and include Javadoc documentation and sample code.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html)


#### Tags:

 - SDK, Java, Custom Packages, Bot Development, Extensions

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html)

### Automation Anywhere Repository Management API
The Automation Anywhere Repository Management API provides programmatic access to the Control Room's bot and file repository. It allows developers and administrators to list, search, upload, and manage bots, folders, and dependent files stored in both the public and private workspaces. This API supports bot lifecycle management use cases including automated promotion of bots between environments, bulk file operations, and integration with source control systems. It is typically used alongside the BLM (Bot Lifecycle Management) API for exporting and importing bots with all their dependencies.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html)


#### Tags:

 - Repository, Bot Lifecycle, File Management, RPA, DevOps

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html)
- [OpenAPI](openapi/automation-anywhere-repository-management-openapi.yml)

## Common Properties

- [Portal](https://developer.automationanywhere.com/)
- [Documentation](https://docs.automationanywhere.com/)
- [Website](https://www.automationanywhere.com/)
- [PrivacyPolicy](https://www.automationanywhere.com/legal/privacy-policy)
- [TermsOfService](https://www.automationanywhere.com/legal/terms)
- [Support](https://support.automationanywhere.com/)
- [Blog](https://www.automationanywhere.com/blog)
- [Login](https://community.automationanywhere.com/s/login/)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
