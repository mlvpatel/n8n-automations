<div align="center">

# ⚡ n8n Automations

### 40 production-grade n8n workflows — every one import-tested in a live n8n instance

![Workflows](https://img.shields.io/badge/workflows-40-orange?style=flat-square)
![Import Tested](https://img.shields.io/badge/import%20tested-40%2F40%20passing-brightgreen?style=flat-square)
![n8n](https://img.shields.io/badge/n8n-latest-EA4B71?style=flat-square&logo=n8n&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen?style=flat-square)

*A hand-picked collection of automation workflows spanning AI agents, sales, DevOps, marketing, and more — each sanitized, modernized to current n8n, and verified to import into a running n8n instance.*

</div>

---

## Why this repo

Most n8n "collections" are thousand-file dumps scraped from the web, full of broken JSON, dead API references, and 2023-era model names. This is the opposite: **40 workflows, curated and engineered.** Every file here has been:

- ✅ **Import-tested** — loaded into a live `n8nio/n8n:latest` container; 40/40 pass
- 🧹 **Sanitized** — no credentials, no instance IDs, no personal data (see [SECURITY.md](SECURITY.md))
- 🔄 **Modernized** — current AI models (GPT-4o, Claude 4.x, Gemini 2.5), current node types, current expression syntax
- 📁 **Organized** — grouped by role so you can find what fits your work

## Quick start

```bash
# 1. Pick a workflow from the categories below
# 2. In n8n:  Workflows → ⋯ menu → Import from File
# 3. Open each node, add your own credentials (every credential slot is labeled)
# 4. Activate
```

> Every credential in these files is blanked and labeled `Add your <service> credential` — you supply your own. Nothing here contains secrets.

---

## 📂 Browse by category

| Category | Workflows | What's inside |
|---|:--:|---|
| [🤖 AI Agents & RAG](#ai-agents--rag) | 3 | Autonomous agents, retrieval-augmented chatbots, and multi-step LLM pipelines |
| [📈 Sales & CRM](#sales--crm) | 3 | Lead scraping, enrichment, meeting prep, and pipeline automation |
| [📣 Marketing](#marketing) | 3 | SEO research, content generation, and publishing pipelines |
| [🎬 Content & Social](#content--social) | 3 | Video summarization, image generation, and cross-platform posting |
| [💬 Customer Support](#customer-support) | 3 | AI triage, knowledge-base generation, and resolution automation |
| [⚙️ DevOps & IT](#devops--it) | 3 | Backups, deployment, and infrastructure health monitoring |
| [🛠️ Developer Tools](#developer-tools) | 3 | GitHub automation, dynamic data modeling, and visual testing |
| [📊 Data & Analytics](#data--analytics) | 2 | ETL into warehouses and natural-language SQL |
| [🔐 Security](#security) | 2 | Login-anomaly detection and certificate lifecycle bots |
| [💰 Finance](#finance) | 2 | Expense extraction and AI tax/document assistants |
| [🧑‍💼 HR & Recruiting](#hr--recruiting) | 3 | Resume screening, application intake, and policy chatbots |
| [✅ Productivity](#productivity) | 3 | Two-way syncs, inbox-to-Notion, and attachment routing |
| [🛒 E-commerce](#e-commerce) | 2 | AI store support and order synchronization |
| [🏢 Business Ops](#business-ops) | 3 | Document parsing, monitoring, and general SMB automation |
| [📋 Project Management](#project-management) | 1 | Task and time-tracking synchronization |
| [🎓 Education](#education) | 1 | Document-to-study-notes generation |

---

### 🤖 AI Agents & RAG
*Autonomous agents, retrieval-augmented chatbots, and multi-step LLM pipelines*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Host Your Own AI Deep Research Agent with n8n, Apify and OpenAI o3](workflows/ai-agents-rag/host-your-own-ai-deep-research-agent-with-n8n-apify-and-openai-o3.json) | Chain Llm, Execution Data, Lm Chat Google Gemini, Lm Chat Open Ai | 87 |
| [AI Powered RAG Chatbot for Your Docs + Google Drive + Gemini + Qdrant](workflows/ai-agents-rag/ai-powered-rag-chatbot-for-your-docs-google-drive-gemini-qdrant.json) | Google Docs, Google Drive, Telegram | 50 |
| [Send a ChatGPT email reply and save responses to Google Sheets](workflows/ai-agents-rag/send-a-chatgpt-email-reply-and-save-responses-to-google-sheets.json) | Gmail, Gmail Trigger, Google Sheets, Open Ai | 49 |

### 📈 Sales & CRM
*Lead scraping, enrichment, meeting prep, and pipeline automation*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [HDW Lead Gelndewagen](workflows/sales-crm/hdw-lead-gel-ndewagen.json) | Google Sheets, Hdw Linkedin, Hdw Linkedin Management, Hdw Web Parser Tool | 93 |
| [LinkedIn Leads Scraping & Enrichment (Main)](workflows/sales-crm/linkedin-leads-scraping-enrichment.json) | Google Sheets, Google Sheets Trigger | 66 |
| [Automate Sales Meeting Prep with AI & APIFY Sent To WhatsApp](workflows/sales-crm/automate-sales-meeting-prep-with-ai-apify-sent-to-whatsapp.json) | Chain Llm, Gmail, Google Calendar, Information Extractor | 61 |

### 📣 Marketing
*SEO research, content generation, and publishing pipelines*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [AI-Generated Summary Block for WordPress Posts - with OpenAI, WordPress, Google Sheets & Slack](workflows/marketing/ai-generated-summary-block-for-wordpress-posts-with-openai-wordpress-g.json) | Google Sheets, Slack, Wordpress | 32 |
| [Easy Wordpress Content Creation from PDF Document + Human In The Loop with Gmail Approval](workflows/marketing/easy-wordpress-content-creation-from-pdf-document-human-in-the-loop-wi.json) | Gmail, Telegram, Wordpress | 27 |
| [Ahrefs Keyword Research Workflow](workflows/marketing/ahrefs-keyword-research-workflow.json) | Agent, Chat Trigger, Lm Chat Google Gemini, Memory Buffer Window | 14 |

### 🎬 Content & Social
*Video summarization, image generation, and cross-platform posting*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [AI-Powered YouTube Playlist & Video Summarization and Analysis v2](workflows/content-social/ai-powered-youtube-playlist-video-summarization-and-analysis-v2.json) | Agent, Chain Llm, Chat Trigger, Document Default Data Loader | 72 |
| [AI-Powered Short-Form Video Generator with OpenAI, Flux, Kling, and ElevenLabs and upload to all ...](workflows/content-social/ai-powered-short-form-video-generator-with-openai-flux-kling-and-eleve.json) | Discord, Google Drive, Google Sheets | 51 |
| [Generate Instagram Content from Top Trends with AI Image Generation](workflows/content-social/generate-instagram-content-from-top-trends-with-ai-image-generation.json) | Facebook Graph Api, Open Ai, Postgres, Telegram | 44 |

### 💬 Customer Support
*AI triage, knowledge-base generation, and resolution automation*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Auto Knowledge Base Article Generator](workflows/customer-support/auto-knowledge-base-article-generator.json) | Agent, Chat Trigger, Lm Chat Open Ai, Tool Workflow | 23 |
| [OpenAI Assistant for Hubspot Chat](workflows/customer-support/openai-assistant-for-hubspot-chat.json) | Airtable | 34 |
| [Automate Customer Support Issue Resolution using AI Text Classifier](workflows/customer-support/automate-customer-support-issue-resolution-using-ai-text-classifier.json) | Agent, Chain Llm, Jira, Jira Tool | 36 |

### ⚙️ DevOps & IT
*Backups, deployment, and infrastructure health monitoring*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Automated Workflow Backups to Google Drive](workflows/devops-it/automated-workflow-backups-to-google-drive.json) | Google Drive, N8N, Telegram | 23 |
| [n8n workflow deployer](workflows/devops-it/n8n-workflow-deployer.json) | Google Drive, Google Drive Trigger | 21 |
| [MAIA - Health Check](workflows/devops-it/maia-health-check.json) | Google Sheets, Telegram | 7 |

### 🛠️ Developer Tools
*GitHub automation, dynamic data modeling, and visual testing*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Github Releases](workflows/developer-tools/github-releases.json) | Redis, Rss Feed Read, Slack | 25 |
| [Dynamically create tables in Airtable for your Webflow form submissions](workflows/developer-tools/dynamically-create-tables-in-airtable-for-your-webflow-form-submission.json) | Airtable, Webflow Trigger | 17 |
| [Visual Regression Testing with Apify and AI Vision Model](workflows/developer-tools/visual-regression-testing-with-apify-and-ai-vision-model.json) | Chain Llm, Google Drive, Google Sheets, Linear | 34 |

### 📊 Data & Analytics
*ETL into warehouses and natural-language SQL*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Import Productboard Notes, Companies and Features into Snowflake](workflows/data-analytics/import-productboard-notes-companies-and-features-into-snowflake.json) | Slack, Snowflake | 35 |
| [Translate questions about e-mails into SQL queries and run them](workflows/data-analytics/translate-questions-about-e-mails-into-sql-queries-and-run-them.json) | Agent, Chat Trigger, Lm Chat Ollama, Postgres | 26 |

### 🔐 Security
*Login-anomaly detection and certificate lifecycle bots*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Suspicious_login_detection](workflows/security/suspicious-login-detection.json) | Gmail, Postgres, Slack | 43 |
| [Venafi Cloud Slack Cert Bot](workflows/security/venafi-cloud-slack-cert-bot.json) | Open Ai, Slack, Venafi Tls Protect Cloud | 38 |

### 💰 Finance
*Expense extraction and AI tax/document assistants*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Extract spend details (template)](workflows/finance/extract-spend-details.json) | Gmail Trigger, Google Sheets | 25 |
| [Build a Tax Code Assistant with Qdrant, Mistral.ai and OpenAI](workflows/finance/build-a-tax-code-assistant-with-qdrant-mistral-ai-and-openai.json) | Agent, Chat Trigger, Compression, Document Default Data Loader | 38 |

### 🧑‍💼 HR & Recruiting
*Resume screening, application intake, and policy chatbots*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Handling Job Application Submissions with AI and n8n Forms](workflows/hr-recruiting/handling-job-application-submissions-with-ai-and-n8n-forms.json) | Airtable, Chain Llm, Lm Chat Open Ai, Output Parser Structured | 23 |
| [Resume Screening & Behavioral Interviews with Gemini, Elevenlabs, & Notion ATS copy](workflows/hr-recruiting/resume-screening-behavioral-interviews-with-gemini-elevenlabs-notion-a.json) | Google Drive, Google Sheets, Notion, Notion Tool | 67 |
| [BambooHR AI-Powered Company Policies and Benefits Chatbot](workflows/hr-recruiting/bamboohr-ai-powered-company-policies-and-benefits-chatbot.json) | Agent, Bamboo Hr, Chain Llm, Chat Trigger | 50 |

### ✅ Productivity
*Two-way syncs, inbox-to-Notion, and attachment routing*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Realtime Notion Todoist 2-way Sync Template](workflows/productivity/realtime-notion-todoist-2-way-sync.json) | Compare Datasets, Execution Data, Gmail, Notion | 246 |
| [mails2notion V2](workflows/productivity/mails2notion-v2.json) | Airtable, Gmail, Gmail Trigger | 38 |
| [Attachments Gmail to drive and google sheets](workflows/productivity/attachments-gmail-to-drive-and-google-sheets.json) | Gmail, Gmail Trigger, Google Drive, Google Sheets | 17 |

### 🛒 E-commerce
*AI store support and order synchronization*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [AI-powered WooCommerce Support-Agent](workflows/ecommerce/ai-powered-woocommerce-support-agent.json) | Agent, Chat Trigger, Dhl, Lm Chat Open Ai | 40 |
| [[n8n] - Shopify Orders to D365 Business Central Sales Orders / Sales Invoices](workflows/ecommerce/shopify-orders-to-d365-business-central-sales-orders-sales-invoices.json) | Shopify | 39 |

### 🏢 Business Ops
*Document parsing, monitoring, and general SMB automation*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Advanced AI Powered Document Parsing & Text Extraction with Llama Parse](workflows/business-ops/advanced-ai-powered-document-parsing-text-extraction-with-llama-parse.json) | Gmail, Gmail Trigger, Google Drive, Google Sheets | 54 |
| [Monthly Spotify Track Archiving and Playlist Classification](workflows/business-ops/monthly-spotify-track-archiving-and-playlist-classification.json) | Chain Llm, Google Sheets, Lm Chat Anthropic, Output Parser Structured | 37 |
| [AI-Powered Information Monitoring with OpenAI, Google Sheets, Jina AI and Slack](workflows/business-ops/ai-powered-information-monitoring-with-openai-google-sheets-jina-ai-an.json) | Chain Llm, Google Sheets, Lm Chat Open Ai, Rss Feed Read | 31 |

### 📋 Project Management
*Task and time-tracking synchronization*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Notion to Clockify Sync Template](workflows/project-management/notion-to-clockify-sync.json) | Clockify, Compare Datasets, Notion | 68 |

### 🎓 Education
*Document-to-study-notes generation*

| Workflow | Key integrations | Nodes |
|---|---|:--:|
| [Breakdown Documents into Study Notes using Templating MistralAI and Qdrant](workflows/education/breakdown-documents-into-study-notes-using-templating-mistralai-and-qd.json) | Chain Llm, Chain Retrieval Qa, Chain Summarization, Document Default Data Loader | 42 |

---

## How these were built

This collection was produced by a multi-stage engineering pipeline, not hand-copying:

1. **Aggregated** from 2,500+ community workflows across several open-source repos
2. **Audited** — each scored on structure (triggers, error handling, credentials, real integrations, documentation)
3. **Modernized** — deprecated nodes migrated, legacy AI models upgraded, expression syntax updated to current n8n
4. **Sanitized** — all secrets, credentials, and instance metadata stripped
5. **Import-tested** — validated against a live n8n container
6. **Curated** — the top 40 selected for range and quality

The full comprehensive library (2,400+ workflows across 16 categories) is maintained separately.

## License

[MIT](LICENSE) — free to use, modify, and build on. Attribution appreciated but not required.

## Security

No credentials or secrets are stored in this repository. See [SECURITY.md](SECURITY.md) for the sanitization standard and how to report a concern.

---

<div align="center">
<sub>Curated & engineered by <a href="https://github.com/mlvpatel">@mlvpatel</a> · Built with n8n</sub>
</div>
