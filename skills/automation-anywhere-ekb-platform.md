---
name: automationanywhere
description: Use when building AI agents, creating workflows, configuring knowledge bases, integrating third-party services, or automating business processes. Reach for this skill when agents need to query databases, search the web, execute code, manage documents, or interact with enterprise systems like Salesforce, Jira, or Microsoft 365.
metadata:
    mintlify-proj: automationanywhere
    version: "1.0"
---

# Automation Anywhere EKB Skill

## Product Summary

Automation Anywhere EKB is an enterprise AI agent platform that bridges large language models with business data and systems. Agents are AI assistants equipped with personality prompts, persistent memory, and toolkits that enable them to interact with databases, APIs, code execution environments, and third-party services. The platform abstracts authentication, API wiring, and error handling so you can focus on agent behavior and business logic.

**Key files and paths:**
- Agent configuration: `agents/agents.mdx` (personality prompts, model selection, toolkit setup)
- Workflows: `tools/workflows-v2.mdx` (automation triggers, nodes, execution)
- Knowledge Base: `knowledge-base/kb-overview.mdx` (document ingestion, RAG setup)
- Toolkits: 50+ pre-built integrations (Gmail, Jira, Salesforce, databases, Python, web search, etc.)
- API reference: `project-settings/api-keys.mdx` (authentication and programmatic access)

**Primary docs link:** https://ai-kb.automationanywhere.com

## When to Use

Reach for this skill when:

- **Building AI agents** — Creating custom agents with specific personalities, instructions, and tool access for customer support, sales, HR, finance, or IT workflows
- **Automating multi-step processes** — Designing workflows triggered by user input, file uploads, schedules, or emails that chain together agents, tools, and conditional logic
- **Integrating enterprise systems** — Connecting agents to Salesforce, Jira, ServiceNow, Microsoft 365, databases, or custom APIs
- **Implementing RAG (Retrieval Augmented Generation)** — Setting up knowledge bases so agents can reference proprietary documents, policies, or FAQs
- **Executing code dynamically** — Running Python or Node.js scripts in secure sandboxes for data transformation, analysis, or complex logic
- **Managing agent memory** — Configuring persistent user preferences and conversation context across sessions
- **Deploying chatbots** — Publishing agents to Slack, Teams, Discord, or public web interfaces
- **Troubleshooting agent behavior** — Debugging hallucinations, tool failures, or incorrect responses through prompt refinement and version history

## Quick Reference

### Agent Configuration Essentials

| Task | Steps |
|------|-------|
| **Create agent** | Dashboard → Create Agent → Choose "Create from Prompt" (AI-assisted) or "Create Custom Agent" (manual) |
| **Set personality prompt** | General Settings → Personality Prompt field → Write 200-500 word instructions covering role, mission, constraints, tool usage, output format, escalation triggers |
| **Select LLM model** | General Settings → Model dropdown → Choose GPT-5, Claude 4, Gemini 3, DeepSeek, or cost-optimized variants |
| **Add toolkits** | Toolkits tab → Browse by category → Click "Add to Agent" → Configure connections if required |
| **Reference tools in prompt** | Type `@` in Personality Prompt → Select toolkit → Describe when/how agent should use it |
| **Test agent** | Chat tab → Type queries → Observe tool invocation and responses → Iterate prompt if needed |
| **Enable memory** | Memory Settings → Toggle "Enable Memory" → Review pending memories → Approve/reject candidates |

### Workflow Builder V2 Essentials

| Component | Purpose |
|-----------|---------|
| **Trigger** | Start workflow: Manual Input, File Upload, Schedule, Email |
| **Tool Node** | Execute action: API call, database query, code execution, toolkit action |
| **Agent Node** | Invoke an agent within workflow |
| **Condition Node** | Branch logic: IF-THEN-ELSE |
| **Final Output** | Return result to user |
| **Variable passing** | Use `@` symbol to reference data from previous steps |
| **Execution logs** | Executions tab → Select run → Inspect each step's input/output |

### Toolkit Categories (50+ available)

| Category | Examples |
|----------|----------|
| **Knowledge & Content** | Knowledge Base, Web Search, Document Manager, PDF, Image Generation |
| **Data & Analytics** | Database, Smart Table Manager, Airtable, Databricks, New Relic, Datadog |
| **Code & Development** | Python, Node.js, GitHub, GitLab, Bitbucket, Agent Manager |
| **Planning & Productivity** | Todo Manager, Trello, Linear, Asana, Smartsheet |
| **Messaging & Communication** | Gmail, Slack, Teams, Discord, Telegram, WhatsApp, Twilio |
| **CRM & Business Apps** | Salesforce, HubSpot, Odoo ERP, ServiceNow, Jira, Confluence |
| **Cloud & Infrastructure** | Google Cloud Platform, AWS S3, Azure Active Directory |
| **Automation** | Workflow Manager, Agent Communication, Platform Actions |

### API Key Management

| Key Type | Use Case |
|----------|----------|
| **Privileged Key** | Server-to-server automation, full project access (edit/delete agents, workflows, settings) |
| **Locked-Down Viewer Key** | Public-facing bots, channel integrations, read-only + chat runtime |

**Generate key:** Settings → API Keys → Create API Key → Select type → Name → Generate → Copy immediately

## Decision Guidance

### When to Use: Create from Prompt vs. Create Custom Agent

| Scenario | Use "Create from Prompt" | Use "Create Custom Agent" |
|----------|-------------------------|--------------------------|
| **Speed & simplicity** | New to prompt engineering, need prototype fast | Advanced user, need precise control |
| **Toolkit selection** | Let AI auto-select based on description | Manually choose specific toolkits |
| **Prompt engineering** | AI generates initial prompt | Write prompt from scratch |
| **Production readiness** | Good starting point, requires refinement | Ready for enterprise deployment |

### When to Use: Agent vs. Workflow

| Use Case | Choose Agent | Choose Workflow |
|----------|-------------|-----------------|
| **Conversational interaction** | ✅ Agent responds to user queries in chat | ❌ Workflows are deterministic, not conversational |
| **Multi-step automation** | ✅ Agent can chain tools intelligently | ✅ Workflow explicitly chains steps |
| **Flexible decision-making** | ✅ Agent uses reasoning to decide tool usage | ❌ Workflow requires explicit IF-THEN logic |
| **Scheduled/triggered execution** | ❌ Agents respond to user input | ✅ Workflows triggered by schedule, email, file upload |
| **Deterministic process** | ❌ Agent behavior varies by input | ✅ Workflow follows fixed logic |

### When to Use: Knowledge Base vs. Web Search vs. Database

| Data Source | Use Knowledge Base | Use Web Search | Use Database |
|-------------|-------------------|----------------|--------------|
| **Proprietary docs** | ✅ PDFs, policies, FAQs | ❌ | ❌ |
| **Real-time public data** | ❌ | ✅ Stock prices, news, competitor info | ❌ |
| **Structured business data** | ❌ | ❌ | ✅ Customer records, transactions, inventory |
| **Compliance/audit trail** | ✅ Versioned, searchable | ❌ | ✅ Queryable, logged |

## Workflow

### Typical Agent Development Workflow

1. **Understand the use case**
   - Define agent's primary responsibility (e.g., "IT support for password resets")
   - Identify required toolkits (e.g., Azure AD, Knowledge Base, Document Manager)
   - List constraints and escalation triggers

2. **Create the agent**
   - Dashboard → Create Agent → Choose "Create Custom Agent" for production
   - Name the agent descriptively (e.g., "IT Support Specialist")
   - Select appropriate LLM (GPT-5 for reasoning, Claude for coding, Gemini for multimodal)

3. **Configure personality prompt**
   - Write 200-500 word prompt covering: role, mission, user context, behavioral rules, tool usage, output format, escalation triggers, tone
   - Use the IT Support Agent example in best practices as a template
   - Include 2-3 concrete examples of desired behavior
   - Explicitly state what agent CANNOT do

4. **Add and configure toolkits**
   - Toolkits tab → Add required integrations
   - For each toolkit requiring auth (Gmail, Jira, Salesforce), go to Settings → Connections → Configure credentials
   - Return to agent and verify toolkit appears in Personality Prompt

5. **Reference tools in prompt**
   - In Personality Prompt, type `@` to insert toolkit references
   - Describe when and how agent should use each tool
   - Example: "Use the Azure AD Toolkit to verify user identity before resetting passwords"

6. **Test in Chat**
   - Chat tab → Test happy path (standard query with all info)
   - Test missing info (does agent ask clarifying questions?)
   - Test edge cases (out-of-scope requests, ambiguous queries)
   - Test tool triggers (verify specific toolkits activate)

7. **Iterate based on failures**
   - Review conversation logs in Chat
   - Identify where agent hallucinated, failed to use tools, or gave wrong answers
   - Update Personality Prompt to address specific scenarios
   - Use Version History to track changes and rollback if needed

8. **Deploy and monitor**
   - Set as Default Agent if appropriate
   - Deploy to Slack, Teams, or public chatbot if needed
   - Monitor agent interactions in Chat logs
   - Refine prompt monthly based on real usage patterns

### Typical Workflow Automation Workflow

1. **Define the process**
   - Identify trigger (manual input, file upload, schedule, email)
   - List steps (agent calls, tool invocations, conditionals)
   - Define output format

2. **Create workflow**
   - Tools → + New Flow → Create Tool
   - Add Trigger block (Manual Input, File Upload, Schedule, Email)
   - Configure trigger properties (input names, schedule timing, etc.)

3. **Build the flow**
   - Drag Tool/Agent/Condition nodes onto canvas
   - Connect trigger to first node
   - Chain nodes by dragging from `+` connector to next node's input
   - Configure each node (select agent, tool, parameters)

4. **Pass data between steps**
   - Use `@` symbol to reference variables from previous steps
   - Example: In Web Search node, search for `@company_name` from Manual Input trigger

5. **Test the workflow**
   - Run Flow button → Execute with test data
   - Executions tab → Select run → Inspect each step's input/output
   - Identify failures and fix node configuration

6. **Publish and deploy**
   - Publish button → Workflow becomes available to project
   - Share with team or integrate into chat interface

## Common Gotchas

- **Personality prompt too short** — "You are a helpful assistant" is insufficient. Write 200-500 words covering role, constraints, tool usage, output format, and escalation triggers. Vague prompts cause hallucinations and tool misuse.

- **Agent not using tools** — Agent responds "I don't have access" even though toolkit is enabled. Fix: Verify toolkit is added, description is clear, and Personality Prompt explicitly encourages usage with `@` references.

- **Hallucinating data** — Agent invents information instead of saying "I don't know." Fix: Add explicit instruction to Personality Prompt: "If information is not found, say: 'I cannot verify that. Please check [source].'"

- **Tool authentication failures** — Toolkit returns "Unauthorized" error. Fix: Verify credentials in Settings → Connections, check token expiry, confirm required OAuth scopes are granted.

- **Slow responses (>10 seconds)** — Queries timeout or feel sluggish. Fix: Check context window size, optimize Knowledge Base (remove outdated docs), use parallel execution where possible, consider simpler model.

- **Memory not persisting** — Agent doesn't recall user preferences in next conversation. Fix: Verify "Enable Memory" is toggled ON in Memory Settings, check that memories are in "approved" status (not pending), confirm memory is enabled for the agent.

- **Workflow variable passing fails** — Data doesn't flow between steps. Fix: Use `@` symbol to reference variable names exactly as defined in previous steps, check variable type matches expected input.

- **Knowledge Base not retrieving documents** — Agent says "I don't have that information" even though document is uploaded. Fix: Verify sync completed successfully (check KB Settings → Sync & Schedule), ensure document structure is clear (good chunking), remove outdated conflicting documents.

- **Deprecated V1 workflows** — Old workflows still work but can't be edited in V2 interface. Fix: Use V2 Workflow Builder for new automations; migration tool coming in future release.

- **API key exposure** — Accidentally committed API key to version control. Fix: Immediately delete key in Settings → API Keys, regenerate new key, rotate in any external systems using it.

## Verification Checklist

Before deploying an agent or workflow to production:

- ✅ **Personality Prompt**: 200+ words, covers role/mission/constraints/tool usage/output format/escalation
- ✅ **Toolkits configured**: All required integrations added and authenticated (check Settings → Connections)
- ✅ **Tool references**: Personality Prompt includes `@` references to each toolkit with usage instructions
- ✅ **Happy path tested**: Standard query with all required info produces correct response
- ✅ **Edge cases tested**: Missing info, out-of-scope requests, ambiguous queries handled correctly
- ✅ **Tool triggers verified**: Each toolkit activates when expected
- ✅ **Error handling**: Agent gracefully handles tool failures and says "I don't know" instead of hallucinating
- ✅ **Memory enabled** (if needed): Toggle ON, pending memories reviewed and approved
- ✅ **Version history**: Initial version saved, ready to iterate
- ✅ **Security**: Least privilege applied (only required toolkits enabled), approval workflows set for high-risk actions
- ✅ **Documentation**: User guide prepared, troubleshooting steps documented

## Resources

**Comprehensive page-by-page navigation:** https://ai-kb.automationanywhere.com/llms.txt

**Critical documentation pages:**
1. [Agent Overview & Configuration](https://ai-kb.automationanywhere.com/agents/agents) — Complete guide to agent creation, personality prompts, model selection, and advanced features
2. [Best Practices & Prompt Engineering](https://ai-kb.automationanywhere.com/agents/best-practices) — Detailed personality prompt anatomy, examples, testing strategies, and troubleshooting
3. [Workflow Builder V2](https://ai-kb.automationanywhere.com/tools/workflows-v2) — Step-by-step workflow creation, data passing, debugging, and version history

---

> For additional documentation and navigation, see: https://ai-kb.automationanywhere.com/llms.txt