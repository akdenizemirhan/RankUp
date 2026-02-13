<div align="center">

# RankUp

### All-in-one SEO toolkit for AI agents

The most comprehensive SEO MCP server for Claude, Cursor, Windsurf, and other AI assistants.\
26 tools for keyword research, content writing, SERP analysis, and multi-platform publishing.

[![npm version](https://img.shields.io/npm/v/rankup?style=flat-square&color=CB3837)](https://www.npmjs.com/package/rankup)
[![npm downloads](https://img.shields.io/npm/dm/rankup?style=flat-square&color=CB3837)](https://www.npmjs.com/package/rankup)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)
![Tools](https://img.shields.io/badge/tools-26-6366f1?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-compatible-8b5cf6?style=flat-square)

[Website](https://rankup.tools) · [npm](https://www.npmjs.com/package/rankup) · [Issues](https://github.com/akdenizemirhan/rankup/issues)

</div>

---

## Why RankUp?

Most SEO tools are built for humans clicking through dashboards. **RankUp is built for AI agents.** It gives your AI assistant direct access to keyword data, SERP analysis, content generation, and publishing — all through a single MCP server.

- **One command setup** — `npx rankup setup` and you're ready
- **Works everywhere** — Claude Code, Claude Desktop, Cursor, Windsurf, any MCP client
- **Full pipeline** — Research → Write → Optimize → Publish, all in one session
- **No browser needed** — Your AI agent handles everything
- **100% free** — All 26 tools available at no cost

---

## Quick Start

### 1. Get your API key

Sign up at **[rankup.tools](https://rankup.tools)** — completely free.

### 2. Install & configure

```bash
npx rankup setup
```

### 3. Add to your AI client

<details>
<summary><b>Claude Code</b></summary>

```bash
claude mcp add rankup -- npx -y rankup
```

</details>

<details>
<summary><b>Claude Desktop</b></summary>

Add to `~/Library/Application Support/Claude/claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "rankup": {
      "command": "npx",
      "args": ["-y", "rankup"]
    }
  }
}
```

</details>

<details>
<summary><b>Cursor / Windsurf</b></summary>

Add to MCP server settings:

```json
{
  "mcpServers": {
    "rankup": {
      "command": "npx",
      "args": ["-y", "rankup"]
    }
  }
}
```

</details>

### 4. Configure integrations (optional)

```bash
npx rankup secrets
```

Set up image generation (fal.ai), WordPress, Ghost, or webhook integrations through an interactive wizard.

---

## Tools

### SEO Research

| Tool | Description |
|------|-------------|
| `keyword_research` | Keywords with SERP analysis, related searches, People Also Ask |
| `serp_tracker` | Track domain rankings for any keyword |
| `page_speed` | PageSpeed Insights performance metrics |
| `on_page_seo` | On-page SEO audit — title, meta, headings, images |
| `site_crawl` | Crawl site structure following internal links |

### Strategy & Planning

| Tool | Description |
|------|-------------|
| `seo_strategy` | Comprehensive SEO strategies with action items |
| `topical_map` | Topic clusters for topical authority |
| `content_calendar` | Content schedules with prioritized keywords |

### Content Creation

| Tool | Description |
|------|-------------|
| `content_brief` | Detailed briefs with outline and competitor analysis |
| `content_write` | Full SEO-optimized articles with SERP research |
| `image_prompt` | AI image prompts — hero, section, diagram |
| `generate_image` | Image generation with FLUX Schnell via fal.ai |

### Content Optimization

| Tool | Description |
|------|-------------|
| `quality_check` | Pre-publish QA — SEO, grammar, content quality scoring |
| `geo_optimize` | Optimize for AI search engines (ChatGPT, Perplexity, SGE) |
| `internal_links` | Internal linking opportunities with anchor text suggestions |
| `schema_generate` | JSON-LD schema markup (Article, FAQ, HowTo, Product) |

### Publishing

| Tool | Description |
|------|-------------|
| `save_content` | Save content to session for later use |
| `publish_content` | Publish to all configured platforms at once |
| `publish_wordpress` | Direct WordPress publishing via REST API |
| `publish_ghost` | Direct Ghost publishing via Admin API |
| `send_webhook` | Send to Make, n8n, Zapier, Slack |

### Session Management

| Tool | Description |
|------|-------------|
| `full_pipeline` | Complete content workflow guide |
| `get_session` | View current session state |
| `clear_session` | Clear all session data |
| `list_content` | List all saved content |
| `load_content` | Load specific content by ID |

---

## CLI

| Command | Description |
|---------|-------------|
| `npx rankup` | Start MCP server |
| `npx rankup setup` | Setup wizard |
| `npx rankup secrets` | Configure API keys & integrations |
| `npx rankup test` | Test connection & view usage |
| `npx rankup session` | View current session |
| `npx rankup clear` | Clear session or config data |
| `npx rankup update` | Update to latest version |

---

## License

[MIT](LICENSE)
