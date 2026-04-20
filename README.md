# Automation Anywhere (automation-anywhere)

Automation Anywhere is an enterprise robotic process automation (RPA) platform that enables organizations to automate business processes using software bots. Their developer platform, centered around the Automation 360 Control Room, provides a comprehensive suite of REST APIs for managing bot deployment, workload queues, credentials, repositories, and analytics, as well as an SDK for building custom action packages.

**URL:** [https://developer.automationanywhere.com](https://developer.automationanywhere.com)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - RPA, Automation, Bot Management, Enterprise, Workload, Analytics, Security, DevOps

## Timestamps

- **Created:** 2026-03-21
- **Modified:** 2026-04-19

## APIs

### Automation Anywhere Control Room API

The Automation Anywhere Control Room API is a comprehensive set of RESTful APIs that enable programmatic management and administration of the Automation 360 RPA platform. It provides endpoints across multiple versioned groups covering authentication, user management, credential vault, repository management, device pools, licensing, policy management, and scheduled automations.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html)

#### Tags

 - RPA, Automation, Bot Management, Enterprise, REST

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-control-room-apis.html)
- [OpenAPI](openapi/automation-anywhere-control-room-openapi.yml)

### Automation Anywhere Bot Deploy API

The Automation Anywhere Bot Deploy API (v3/v4) enables external applications and workflows to programmatically trigger the deployment of bots to unattended Bot Runner devices. It supports deploying bots from the public workspace, specifying target devices or device pools, and passing input variables at runtime.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html)

#### Tags

 - RPA, Bot Deployment, Automation, Orchestration, Enterprise

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/deploy-api-supported-v4.html)
- [OpenAPI](openapi/automation-anywhere-bot-deploy-openapi.yml)
- [JSONSchema](json-schema/automation-anywhere-deployment-schema.json)

### Automation Anywhere Workload Management API

The Automation Anywhere Workload Management API provides programmatic control over work item queues used to distribute high-volume automation workloads across multiple Bot Runner devices.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html)

#### Tags

 - Workload Management, Queues, Work Items, RPA, Automation

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/wlm-api-supported-v4.html)
- [OpenAPI](openapi/automation-anywhere-workload-management-openapi.yml)
- [JSONSchema](json-schema/automation-anywhere-work-item-schema.json)

### Automation Anywhere Bot Insight API

The Automation Anywhere Bot Insight API exposes real-time business process analytics and operational intelligence data collected during bot execution. It allows developers to retrieve KPIs, bot run histories, performance rankings, and failure analytics from the Control Room programmatically.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html](https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html)

#### Tags

 - Analytics, Business Intelligence, Reporting, RPA, Bot Monitoring

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v11.3/page/enterprise/topics/bot-insight/user/bot-insight-apis.html)
- [OpenAPI](openapi/automation-anywhere-bot-insight-openapi.yml)

### Automation Anywhere API Task Execution API

The Automation Anywhere API Task Execution API enables developers to invoke API Tasks — a specialized type of bot designed to be called synchronously from external applications like a REST service. It generates execution URLs and tokens that allow applications to trigger a bot task, pass input parameters, and receive output values in a single request-response cycle.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html)

#### Tags

 - API Task, Bot Execution, Integration, RPA, Automation

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/api-task-real-time-endpoint.html)
- [OpenAPI](openapi/automation-anywhere-api-task-execution-openapi.yml)

### Automation Anywhere Credential Vault API

The Automation Anywhere Credential Vault API provides programmatic access to the Control Room's centralized secrets management system. It supports creating, reading, updating, and deleting credentials, credential attributes, Lockers, and Locker Keys used by bots during execution.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html)

#### Tags

 - Credentials, Security, Secrets Management, RPA, Enterprise

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/cv-api-supported.html)
- [OpenAPI](openapi/automation-anywhere-credential-vault-openapi.yml)

### Automation Anywhere Package SDK

The Automation Anywhere Package SDK is a Java-based development toolkit that enables developers to build custom action packages and triggers for the Automation 360 bot editor.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html)

#### Tags

 - SDK, Java, Custom Packages, Bot Development, Extensions

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/developer/cloud-create-package-overview.html)

### Automation Anywhere Repository Management API

The Automation Anywhere Repository Management API provides programmatic access to the Control Room's bot and file repository. It allows developers and administrators to list, search, upload, and manage bots, folders, and dependent files stored in both the public and private workspaces.

**Human URL:** [https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html)

#### Tags

 - Repository, Bot Lifecycle, File Management, RPA, DevOps

#### Properties

- [Documentation](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/repository-management-api.html)
- [OpenAPI](openapi/automation-anywhere-repository-management-openapi.yml)
- [JSONSchema](json-schema/automation-anywhere-bot-schema.json)

## Common Properties

- [Developer Portal](https://developer.automationanywhere.com)
- [Website](https://www.automationanywhere.com)
- [Documentation](https://docs.automationanywhere.com)
- [Authentication](https://docs.automationanywhere.com/bundle/enterprise-v2019/page/enterprise-cloud/topics/control-room/control-room-api/cloud-authentication.html)
- [Terms of Service](https://www.automationanywhere.com/legal/terms)
- [Privacy Policy](https://www.automationanywhere.com/legal/privacy-policy)
- [Support](https://support.automationanywhere.com)
- [Blog](https://www.automationanywhere.com/blog)

## Features

| Name | Description |
|------|-------------|
| JWT Authentication | All Control Room APIs use JWT-based authentication. Tokens are obtained via the Authentication API and passed in the X-Authorization or Authorization Bearer header. OAuth 2.0 is supported from v.27 onwards. |
| Versioned API Endpoints | APIs are versioned (v1, v2, v3, v4) with backwards compatibility maintained for at least two years. Deprecated endpoints are announced with at least one additional year of availability. |
| Swagger UI Explorer | Each Control Room instance exposes a Swagger UI at /swagger/ for interactive API exploration and testing with live credentials. |
| API Task Execution | API Tasks allow RPA bots to be exposed as synchronous REST endpoints, enabling external applications to call bots as microservices with input/output parameter exchange. |
| Workload Queuing | Work item queues allow high-volume data to be fed into RPA pipelines from ERP, CRM, and BPM systems with status tracking and result retrieval. |

## Use Cases

| Name | Description |
|------|-------------|
| DevOps Bot Pipeline | Automate bot deployment across dev, test, and production environments using the Bot Deploy and Repository Management APIs in CI/CD pipelines. |
| Enterprise System Integration | Connect ERP, CRM, and BPM systems to RPA workload queues to distribute and process high-volume transactional data with Automation Anywhere bots. |
| Bot Performance Monitoring | Feed Bot Insight API data into Tableau, Power BI, or Splunk for real-time RPA operational dashboards and business KPI tracking. |
| Credential Governance | Programmatically provision and rotate bot credentials in the Credential Vault from enterprise secrets management systems like CyberArk or HashiCorp Vault. |
| Custom Action Packages | Build proprietary Java action packages using the Package SDK to extend Automation 360 with custom connectors for legacy or specialized systems. |

## Integrations

| Name | Description |
|------|-------------|
| SAP | Pre-built SAP integration package for Automation 360 enabling bots to interact with SAP GUI, SAP BAPIs, and S/4HANA REST APIs. |
| Salesforce | Automation Anywhere connector for Salesforce CRM enabling bots to create, update, and query Salesforce records via REST APIs. |
| ServiceNow | Integration with ServiceNow for IT service automation including incident creation, ticket routing, and CMDB updates from RPA bots. |
| Microsoft Office 365 | Action packages for interacting with Microsoft 365 services including Outlook, SharePoint, Teams, and Excel via Microsoft Graph API. |
| Blue Prism and UiPath | Migration APIs for moving automations from other RPA platforms to Automation 360 with bot conversion and compatibility tooling. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Automation Anywhere Control Room](openapi/automation-anywhere-control-room-openapi.yml)
- [Automation Anywhere Bot Deploy](openapi/automation-anywhere-bot-deploy-openapi.yml)
- [Automation Anywhere Workload Management](openapi/automation-anywhere-workload-management-openapi.yml)
- [Automation Anywhere Bot Insight](openapi/automation-anywhere-bot-insight-openapi.yml)
- [Automation Anywhere API Task Execution](openapi/automation-anywhere-api-task-execution-openapi.yml)
- [Automation Anywhere Credential Vault](openapi/automation-anywhere-credential-vault-openapi.yml)
- [Automation Anywhere Repository Management](openapi/automation-anywhere-repository-management-openapi.yml)

### JSON Schema

- [Bot Schema](json-schema/automation-anywhere-bot-schema.json)
- [Deployment Schema](json-schema/automation-anywhere-deployment-schema.json)
- [Work Item Schema](json-schema/automation-anywhere-work-item-schema.json)

### JSON-LD

- [Automation Anywhere Context](json-ld/automation-anywhere-context.jsonld)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
