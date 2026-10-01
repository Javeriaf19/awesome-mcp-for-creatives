# Awesome MCP for Creatives & Freelancers ⚡

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Model Context Protocol](https://img.shields.io/badge/MCP-Compatible-blue.svg)](https://modelcontextprotocol.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> **A curated, quality-filtered directory of Model Context Protocol (MCP) servers** — built for designers, freelancers, indie builders, video creators, and solo founders who just want to know: *"Which 5 servers should I actually connect first?"*

---

Most existing MCP lists are dev-infra-heavy (databases, Kubernetes, cloud ops). This list is strictly filtered for **real creative and freelance workflows** — client communication, design tools, content pipelines, and solo-founder operations.

If this saved you time, please drop a ⭐ **Star** — it helps more creators discover it!

---

## 💡 Why This List is Different

* 🎯 **Curated, not comprehensive:** Every entry here is picked because it solves a real creative workflow problem, not just because it exists.
* 🚫 **No infra bloat:** No assumption that you're running Kubernetes, writing SQL, or managing an enterprise data warehouse.
* 💼 **Categorized by Job-to-be-Done:** Grouped by what you are trying to accomplish (Design, Client Ops, Content, Storage, Research).
* 🧐 **Honest notes:** If a server is overkill, hard to configure, or better replaced by an alternative, we say so upfront.

---

## 📑 Table of Contents

- [🎨 Design & Creative Tools](#-design--creative-tools)
- [💼 Client & Freelance Ops](#-client--freelance-ops)
- [📱 Content, Media & Social](#-content-media--social)
- [📁 Docs, Files & Knowledge Base](#-docs-files--knowledge-base)
- [🔍 Search & Inspiration Research](#-search--inspiration-research)
- [🛠️ Dev Tools (for Designers & Builders)](#️-dev-tools-for-designers--builders)
- [🏛️ Official & Reference Servers](#️-official--reference-servers)
- [⚡ Quick Start: Recommended 5-Server Stacks](#-quick-start-recommended-5-server-stacks)
- [🧭 How to Use This List & Best Practices](#-how-to-use-this-list--best-practices)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 🎨 Design & Creative Tools

| Server | What it does | Honest Notes & Recommendation |
| :--- | :--- | :--- |
| **[Figma MCP](https://github.com/GLips/Figma-Context-MCP)** | Lets AI read Figma files, extract design tokens/components, generate code from design frames, and inspect layouts. | **Must-have for UI/UX designers:** Closes the design-to-code gap without manual handoff specs. |
| **[Canva MCP](https://github.com/modelcontextprotocol/servers)** | Connects AI agents to Canva to create, edit, and export graphics, manage brand kits, and draft assets. | Great for freelancers doing high-volume social/content design who want AI to draft initial visual templates. |
| **[ComfyUI / Stable Diffusion MCP](https://github.com/yannick-cw/comfyui-mcp)** | Triggers local or remote ComfyUI workflows, generating AI imagery, upscaling, and background removal on command. | Best for visual creators who already use Stable Diffusion / Flux and want conversational image generation in their agent chat. |
| **[Blender MCP](https://github.com/ahujasid/blender-mcp)** | Controls Blender via natural language to generate 3D primitives, apply materials, adjust lighting, and trigger renders. | Powerful for 3D illustrators and motion designers wanting procedural scene setups. |
| **[Cloudflare MCP](https://github.com/cloudflare/mcp-server-cloudflare)** | Manage Workers, KV, R2 asset storage, and DNS via natural language. | Useful once you are hosting client assets, portfolios, or landing pages. Slight learning curve if you come purely from a design background. |

---

## 💼 Client & Freelance Ops

| Server | What it does | Honest Notes & Recommendation |
| :--- | :--- | :--- |
| **[Gmail MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive)** | Read, search, draft, and send emails directly through your AI assistant. | Pairs perfectly with Calendar MCP for automated client communication and meeting follow-ups. |
| **[Google Calendar MCP](https://github.com/modelcontextprotocol/servers)** | Check availability, create/update events, and reason over client schedules in natural language. | Essential for auto-drafting *"Here is my availability for a discovery call"* responses. |
| **[Google Drive MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive)** | Search, read, and manage files, folders, and client assets stored on Google Drive. | Pull client briefs, PDF proposals, and brand assets directly into conversations instead of manual uploading. |
| **[Stripe MCP](https://github.com/stripe/agent-toolkit)** | Query payments, customer invoices, subscription status, and invoice summaries via natural language. | Only worth connecting once you are invoicing clients directly through Stripe; otherwise skip. |
| **[Airtable MCP](https://github.com/domdomegg/airtable-mcp)** | Read, update, and search Airtable bases — client CRM, project pipelines, and asset registries. | Ideal if your freelance client portal or creative job pipeline is organized in Airtable. |

---

## 📱 Content, Media & Social

| Server | What it does | Honest Notes & Recommendation |
| :--- | :--- | :--- |
| **[Zapier Central / MCP](https://github.com/zapier/zapier-mcp)** | Gives AI access to 6,000+ app actions (social scheduling, Slack notifications, form triggers, Webhooks). | **The ultimate Swiss Army knife:** The fastest way to connect niche apps without custom code. Use when no dedicated MCP exists. |
| **[Notion MCP](https://github.com/suekou/mcp-notion-server)** | Read and write to Notion databases, content calendars, project trackers, and moodboards. | If your creative roadmaps and client deliverables live in Notion, this completes the feedback loop seamlessly. |
| **[Media Toolkit / FFmpeg MCP](https://github.com/modelcontextprotocol/servers)** | Slice videos, convert audio/video formats, compress assets, and extract audio tracks locally. | A lifesaver for video creators, podcasters, and motion designers needing fast batch file transformations. |

---

## 📁 Docs, Files & Knowledge Base

| Server | What it does | Honest Notes & Recommendation |
| :--- | :--- | :--- |
| **[Filesystem MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem)** *(Official)* | Secure, permission-scoped read and write access to local directories and project folders. | **Top Essential Default:** Allows your AI agent to read project files, write code, and organize assets on your computer. |
| **[Fetch MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch)** *(Official)* | Fetches and converts web pages to clean markdown for conversational reference. | Lightweight alternative to heavy browser automation when you just need to summarize web copy or articles. |
| **[Hyperconsciousness](https://github.com/louis030195/hyperconsciousness)** | Stores notes and reference material as encrypted, append-only records, with device sync and grant-scoped MCP search for an AI assistant. | **When to use:** For technical solo builders who want a separate, self-managed knowledge store for project notes. **When to skip:** Developer alpha with CLI setup, not a ready-made notes app; no independent security audit. Grants do not isolate the owner process, and hosted models can see returned plaintext. |
| **[Obsidian MCP](https://github.com/calclavia/mcp-obsidian)** | Direct read/write access to your local Obsidian markdown vault, notes, and backlinks. | Superb for creators using Obsidian as a "Second Brain" for creative concepts, client notes, and article drafts. |

---

## 🔍 Search & Inspiration Research

| Server | What it does | Honest Notes & Recommendation |
| :--- | :--- | :--- |
| **[Brave Search MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search)** *(Official)* | High-speed web and local search directly through your AI client. | Maintained directly by Brave. Fast and reliable for quick fact-checking and looking up documentation. |
| **[Tavily MCP](https://github.com/tavily-ai/tavily-mcp)** | Search engine built specifically for AI agents — returns clean, pre-summarized, hallucination-reduced facts. | Better than standard search when you want the AI to synthesize research rather than link-dump. |
| **[Exa MCP](https://github.com/exa-labs/exa-mcp-server)** | Neural/semantic search ("Find me pages conceptually similar to this"). | Unmatched for finding design inspiration, competitor portfolios, case studies, and aesthetic references. |

---

## 🛠️ Dev Tools (for Designers & Builders)

*Included because most designers-turned-builders end up needing exactly these, and nothing heavier:*

| Server | What it does | Honest Notes & Recommendation |
| :--- | :--- | :--- |
| **[GitHub MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/github)** *(Official)* | Search repositories, manage issues, read pull requests, and push code changes. | Essential once you start publishing web apps, portfolio templates, or open-source resources. |
| **[Playwright MCP](https://github.com/executeautomation/mcp-playwright)** | Full browser automation — navigate pages, click buttons, fill forms, and take screenshots. | Useful for visual regression testing of landing pages, capturing screenshots, and dynamic web scraping. |
| **[Git MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/git)** *(Official)* | Read, search, diff, and manipulate local Git repositories. | Pairs with GitHub MCP for seamless local-to-remote version control. |

---

## 🏛️ Official & Reference Servers

Maintained directly by the **[Model Context Protocol](https://github.com/modelcontextprotocol/servers)** steering group as battle-tested baseline servers:

* **[Filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem)** — Secure local directory read/write.
* **[Fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch)** — Clean web content scraper & converter.
* **[Git](https://github.com/modelcontextprotocol/servers/tree/main/src/git)** — Local Git repository operations.
* **[Memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory)** — Graph-based persistent memory across chat sessions.
* **[Sequential Thinking](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking)** — Structured multi-step reasoning for complex problem solving.
* **[Time](https://github.com/modelcontextprotocol/servers/tree/main/src/time)** — Timezone calculations and time conversion tools.

---

## ⚡ Quick Start: Recommended 5-Server Stacks

Don't overload your AI client. Start with one of these battle-tested stacks:

### 🎨 The UI/UX Designer Stack
1. **Figma MCP** (Extract design tokens & inspect components)
2. **Filesystem MCP** (Save assets & write component code)
3. **Exa MCP** (Semantic search for design patterns & inspiration)
4. **Playwright MCP** (Screenshot live web builds & inspect UI)
5. **Google Drive MCP** (Pull client briefs & brand assets)

### 💼 The Solo Freelancer / Agency Stack
1. **Gmail MCP** (Draft & triage client emails)
2. **Google Calendar MCP** (Schedule calls & manage availability)
3. **Notion MCP** or **Airtable MCP** (Manage client CRM & project milestones)
4. **Filesystem MCP** (Local proposal and deliverable management)
5. **Tavily MCP** (Quick client discovery & industry research)

### ✍️ The Content Creator / Marketer Stack
1. **Notion MCP** (Content calendar & draft database)
2. **Canva MCP** or **ComfyUI MCP** (Generate and adapt graphic assets)
3. **Zapier MCP** (Publish to social channels & trigger alerts)
4. **Fetch MCP** (Scrape competitor blogs & references)
5. **Media Toolkit / FFmpeg MCP** (Convert and trim media files)

---

## 🧭 How to Use This List & Best Practices

1. **Keep it lean (Rule of 5-6):** Do not connect more than 5–6 servers simultaneously. Every connected server adds tool descriptions to your AI's system context, which can slow down response times and degrade tool-selection accuracy.
2. **Start with what hurts most:** If client scheduling eats your hours, set up Calendar/Gmail MCP first. If coding design tokens takes too long, set up Figma MCP.
3. **Prefer Official & Actively Maintained Repos:** When both official and community versions exist, prefer the official/vendor-maintained repository for security and stability.
4. **Guard your API Keys:** Never hardcode secrets in public configuration files. Use environment variables (e.g., in Claude Desktop `claude_desktop_config.json` or Cursor config).

---

## 🤝 Contributing

Contributions are welcome! However, this directory **only stays useful if it remains strictly curated**.

Please read our **[Contributing Guidelines](CONTRIBUTING.md)** before submitting a Pull Request.

### Quick Submission Checklist:
- [x] Solves a **real creative, freelance, or small-team workflow** problem.
- [x] Is **actively maintained** (commits/PRs merged within the last 6 months).
- [x] Includes a clear 1-sentence description and an **honest "When to use / When to skip" note**.
- [x] Not a duplicate of existing functionality unless it offers a massive improvement.

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE). Feel free to use, fork, and remix!

---

<div align="center">
  <sub>Curated with ❤️ by <a href="https://github.com/Javeriaf19">Javeria Farhan</a> and the open-source community.</sub>
</div>
