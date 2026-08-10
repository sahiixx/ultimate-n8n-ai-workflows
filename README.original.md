# 🤖 Ultimate n8n AI Workflows

[![Stars](https://img.shields.io/github/stars/oxbshw/ultimate-n8n-ai-workflows?style=social)](https://github.com/oxbshw/ultimate-n8n-ai-workflows/stargazers)
[![Forks](https://img.shields.io/github/forks/oxbshw/ultimate-n8n-ai-workflows?style=social)](https://github.com/oxbshw/ultimate-n8n-ai-workflows/network/members)
[![Workflows](https://img.shields.io/badge/Workflows-3,400%2B-blue?style=flat-square)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/oxbshw/ultimate-n8n-ai-workflows/blob/main/LICENSE)
[![Issues](https://img.shields.io/github/issues/oxbshw/ultimate-n8n-ai-workflows)](https://github.com/oxbshw/ultimate-n8n-ai-workflows/issues)
[![Last Commit](https://img.shields.io/github/last-commit/oxbshw/ultimate-n8n-ai-workflows)](https://github.com/oxbshw/ultimate-n8n-ai-workflows)

> **The definitive AI workflow library for n8n:** 3,400+ modular, production‑grade automations—plug-and-play for any LLM, integration, or use case.

---

## 🚀 Why This Project Exists

In the era of AI-first development, automation should be:

1. **Accessible**: Visual nodes + low/no-code for rapid prototyping
2. **Scalable**: Enterprise-grade reliability, error handling, and scheduling
3. **Flexible**: Modular JSON workflows, custom modules, and script hooks
4. **Community‑Driven**: Open-source, constantly evolving templates

**Ultimate n8n AI Workflows** brings all of this in a single repo, so you can:

* 🎯 **Jumpstart** AI bots, RAG pipelines, content factories, and data enrichers
* 🔄 **Compose** complex workflows by chaining JSON imports and modules
* 🔒 **Control** your data: run locally (Docker/Kubernetes) or in n8n Cloud
* 🤝 **Collaborate**: submit PRs, vote on issues, and grow together

---

## 📦 Repository Layout

```bash
ultimate-n8n-ai-workflows/
├── workflows/          # 3,400+ ready-to-import .json workflows
├── modules/            # Node.js & Python modules for custom logic
├── data/               # Sample inputs: datasets, prompts, embeddings
├── utils/              # CLI & helper scripts (validation, conversion)
├── docs/               # Guides, architecture diagrams, best practices
├── .github/            # CI workflows, issue/pr templates, contributing guide
└── README.md           # ← You’re here
```

---

## 📚 Core Capabilities

| Feature                         | Description                                                                                 |
| ------------------------------- | ------------------------------------------------------------------------------------------- |
| **Multi‑Model Support**         | GPT-4/4.5, Claude 3.5, LLaMA, Mistral, Gemini, Alpaca, and custom deployments               |
| **Retrieval & Memory**          | RAG pipelines, vector store integration, agent memory nodes                                 |
| **Content Automation**          | SEO-optimized articles, video scripts, social posts, email newsletters                      |
| **Data Extraction**             | RSS/News scraping, X/Twitter collectors, email finders, PDF/OCR Q\&A                        |
| **Conversational Agents**       | Stateful chatbots, auto-reply bots, persona-driven dialogs                                  |
| **Integrations**                | Webhooks, REST APIs, Google Sheets, Databases, Cloud Storage                                |
| **Error Handling & Monitoring** | Built-in retry logic, timeouts, error nodes; integrate with Prometheus/Grafana or n8n Cloud |

---

## 🧩 Quickstart in 5 Minutes

1. **Clone the repo**

   ```bash
   git clone https://github.com/oxbshw/ultimate-n8n-ai-workflows.git
   cd ultimate-n8n-ai-workflows
   ```

2. **Launch n8n** (Docker recommended)

   ```bash
   docker-compose up -d
   ```

3. **Import a Workflow**

   * Open `http://localhost:5678`
   * Select **Import** → **File** → choose a workflow from `/workflows`

4. **Configure Credentials**

   * Add your LLM keys (OpenAI, Anthropic, etc.)
   * Configure API tokens for X/Twitter, Firecrawl, CMS, etc.

5. **Customize & Run**

   * Adjust node parameters, schedule triggers, or chain workflows
   * Monitor execution via logs and error-handling nodes

---

## 🌟 Real‑World Use Cases

* **AI Chatbots & Assistants**: `chatbot_memory_agent.json`
* **SEO Content Pipelines**: `write_seo_listicle_article.json`
* **Email Automation**: `smart_inbox_router.json`
* **Data Enrichment**: `news_to_vector_store.json`
* **Document Q\&A**: `pdf_ocr_agent.json`
* **Social Media Bots**: `twitter_auto_responder.json`

---

## ⚙️ Best Practices

* **Secrets Management**: Store sensitive keys in `.env` or vaults
* **Rate Limiting**: Use n8n’s built-in throttling or external proxies
* **Input Validation**: Pre‑validate with JSON Schema or custom scripts
* **Error Isolation**: Leverage “Error” and “Timeout” nodes for resilience
* **Observability**: Plug into Grafana/Prometheus or n8n Cloud monitoring

---

## 🤝 How to Contribute

1. ⭐ **Star** this project
2. 🐛 **Report Issues** for bugs or enhancement ideas
3. 🔀 **Fork & Pull Request** your workflows or modules
4. 📝 **Improve Docs** in `/docs` with new tutorials or diagrams

Read [CONTRIBUTING.md](.github/CONTRIBUTING.md) for details.

---

## 📜 License

Distributed under the **MIT License**.

See [LICENSE](https://github.com/oxbshw/ultimate-n8n-ai-workflows/blob/main/LICENSE) for full terms.

---

## 📬 Stay Connected

* 🌐 Portfolio: [sayedev.framer.ai](https://sayedev.framer.ai)
* 💻 GitHub: [@oxbshw](https://github.com/oxbshw)
* 🐦 X (Twitter): [@Sayedevv](https://x.com/Sayedevv)
* 🌌 Bluesky: [sayedev.bsky.social](https://bsky.app/profile/sayedev.bsky.social)

---

> **Let’s build the future of AI-driven automation together!** 🚀
