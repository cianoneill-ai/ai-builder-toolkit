# Skills & connectors, sorted by job

Free and open-source AI skills (SKILL.md) and MCP connectors, grouped by use case. Most work across Claude, ChatGPT/Codex, Gemini CLI and Cursor. Browsable version with filters: https://cianoneill.ai/skills/

Links checked September 2026. Cost notes are honest: "free" means the tool is free, though some need a free account with the underlying service.

## Built by me

Ten Shopify skills in [`/skills`](skills/). Drop a folder into your agent's skills directory and connect the Shopify MCP.

- [shopify-cro-agent](skills/shopify-cro-agent/SKILL.md): Walk Shopify funnel from PDP to checkout, pinpoint drop-offs, and suggest prioritized fixes
- [shopify-cross-sell-recommender](skills/shopify-cross-sell-recommender/SKILL.md): Build PDP-ready cross-sell recommendations from Shopify co-purchase data
- [shopify-customer-segmentation](skills/shopify-customer-segmentation/SKILL.md): Build behavioral customer segments from Shopify data for retention and re-engagement
- [shopify-inventory-ad-spend-check](skills/shopify-inventory-ad-spend-check/SKILL.md): Find Shopify products approaching OOS while still receiving heavy paid ad spend
- [shopify-ltv-cohort-view](skills/shopify-ltv-cohort-view/SKILL.md): Compute 30/60/90-day LTV by Shopify acquisition channel, ranked by margin and LTV/CAC
- [shopify-pricing-margin-audit](skills/shopify-pricing-margin-audit/SKILL.md): Audit Shopify pricing and discounts to find SKUs sold below margin floor
- [shopify-product-description-rewriter](skills/shopify-product-description-rewriter/SKILL.md): Rewrite Shopify product descriptions in brand voice, 60-90 words each, with consistent structure
- [shopify-refund-pattern-analysis](skills/shopify-refund-pattern-analysis/SKILL.md): Analyze Shopify refunds by product, reason, and cohort to find SKUs unfit for paid ads
- [shopify-seo-meta-generator](skills/shopify-seo-meta-generator/SKILL.md): Generate intent-matched meta titles and descriptions for Shopify PDPs using Search Console queries
- [shopify-theme-tweaks](skills/shopify-theme-tweaks/SKILL.md): Write Liquid and CSS for small Shopify theme changes without a developer

## Build your own

Start here. Tools that help you make skills and connectors of your own.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [skill-creator](https://github.com/anthropics/skills/tree/main/skills/skill-creator) | Skill | Interviews you, then writes, tests and tunes a new skill for you. | Free |
| [mcp-builder](https://github.com/anthropics/skills/tree/main/skills/mcp-builder) | Skill | Guides your AI through building a working MCP server for any API. | Free |
| [Agent Skills standard](https://agentskills.io) | Spec | The open SKILL.md format. One skill works in Claude, ChatGPT/Codex, Gemini CLI, Cursor and Copilot. | Free |
| [MCP reference servers](https://github.com/modelcontextprotocol/servers) | MCP server | The official starter servers: Fetch, Filesystem, Git, Memory, Time. | Free |

## Coding

For building and shipping software, even if you don't write it yourself.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [GitHub MCP Server](https://github.com/github/github-mcp-server) | MCP server | Lets your AI read repos, open issues and pull requests, and check build results. | Free, needs GitHub account |
| [Context7](https://github.com/upstash/context7) | MCP server | Feeds your AI current library docs so it stops writing outdated code. | Free |
| [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) | MCP server | Opens your site in Chrome, reads the errors and measures page speed. | Free |
| [Superpowers](https://github.com/obra/superpowers) | Skill collection | Makes coding agents plan, test and debug before they write code. | Free |
| [frontend-design + webapp-testing](https://github.com/anthropics/skills/tree/main/skills) | Skill | Polished web interfaces, then tests them in a real browser. | Free |
| [Vercel Agent Skills](https://github.com/vercel-labs/agent-skills) | Skill collection | Best-practice skills for building and deploying React and Next.js apps. | Free |

## Design

Visuals, diagrams, 3D and audio.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [canvas-design, theme-factory, brand-guidelines](https://github.com/anthropics/skills/tree/main/skills) | Skill | Posters, generative art and consistent colour and font themes. | Free |
| [Framelink Figma MCP](https://github.com/GLips/Figma-Context-MCP) | MCP server | Gives your AI the layout and styles of a Figma file so it can build it. | Free, needs Figma (free tier works) |
| [Excalidraw MCP](https://github.com/excalidraw/excalidraw-mcp) | MCP server | Draws editable hand-sketched diagrams right in the chat. | Free |
| [AntV Chart MCP](https://github.com/antvis/mcp-server-chart) | MCP server | Turns your numbers into ready-made charts. | Free |
| [Blender MCP](https://github.com/ahujasid/blender-mcp) | MCP server | Builds and edits 3D scenes in Blender from plain instructions. | Free, needs Blender (free) |
| [ElevenLabs MCP](https://github.com/elevenlabs/elevenlabs-mcp) | MCP server | Voiceovers, sound effects and transcripts from text or audio. | Free tier, needs account |

## Documents

Word, Excel, PowerPoint and PDF without opening Office.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [MarkItDown](https://github.com/microsoft/markitdown) | MCP server | Turns PDFs, Word, Excel and PowerPoint into clean text your AI can read. | Free |
| [Docling MCP](https://github.com/docling-project/docling-mcp) | MCP server | Pulls text and tables out of messy PDFs and scans. | Free |
| [Excel MCP](https://github.com/haris-musa/excel-mcp-server) | MCP server | Reads and writes Excel files, formulas and charts, no Excel needed. | Free |
| [Office Word MCP](https://github.com/GongRzhe/Office-Word-MCP-Server) | MCP server | Creates and edits .docx files with headings, tables and comments. | Free |
| [Office PowerPoint MCP](https://github.com/GongRzhe/Office-PowerPoint-MCP-Server) | MCP server | Builds and edits .pptx decks. | Free |
| [docx, xlsx, pptx, pdf skills](https://github.com/anthropics/skills/tree/main/skills) | Skill | Anthropic's document skills. Excellent, but source-available, not open source. | Free to use in Claude; check licence to reuse |

## Research & web

Search, read and drive the web.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [Fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) | MCP server | Reads any web page and hands your AI the text. | Free |
| [Playwright MCP](https://github.com/microsoft/playwright-mcp) | MCP server | Drives a real browser: click, type, fill forms, screenshot. | Free |
| [SearXNG MCP](https://github.com/ihor-sokoliuk/mcp-searxng) | MCP server | Private web search through your own search instance. No API keys. | Free, self-hosted |
| [Browser Use](https://github.com/browser-use/browser-use) | MCP server | A browser agent that completes multi-step web tasks. | Free if you run it; cloud is paid |
| [Firecrawl MCP](https://github.com/firecrawl/firecrawl-mcp-server) | MCP server | Scrapes and crawls sites into clean text. | Free tier or self-host; crawling needs a key |
| [Exa MCP](https://github.com/exa-labs/exa-mcp-server) | MCP server | Searches the web by meaning. Good for companies, papers and code. | Free tier, needs account |

## Social media & content

Plan, write and publish. Read the cost notes: X and Medium are no longer free to automate.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [Postiz](https://github.com/gitroomhq/postiz-app) | MCP server | Schedules posts to around 28 networks from your AI. | Free self-hosted; X needs paid API |
| [Marketing Skills](https://github.com/coreyhaines31/marketingskills) | Skill collection | Copywriting, SEO, launch plans and content strategy skills. | Free |
| [YouTube Transcript MCP](https://github.com/jkawamoto/mcp-youtube-transcript) | MCP server | Pulls video transcripts so your AI can summarise or repurpose them. | Free |
| [Bluesky MCP](https://github.com/brianellin/bsky-mcp-server) | MCP server | Reads your feeds and publishes posts. | Free, needs app password |
| [WordPress MCP Adapter](https://github.com/WordPress/mcp-adapter) | MCP server | Manages posts and pages on a WordPress site. | Free |
| [Ghost MCP](https://github.com/MFYDev/ghost-mcp) | MCP server | Drafts and publishes posts on a Ghost blog. | Free |

## E-commerce

Run a store with an agent. My own Shopify skills are at the top of this page.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [Shopify Dev MCP](https://shopify.dev/docs/apps/build/devmcp) | MCP server | Answers Shopify API and theme questions from the official docs. | Free |
| [Shopify AI Toolkit](https://github.com/Shopify/shopify-ai-toolkit) | Skill collection | Skills and docs search for building Shopify apps and running stores. | Free (turn off usage data with OPT_OUT_INSTRUMENTATION) |
| [WooCommerce MCP](https://developer.woocommerce.com/docs/features/mcp/) | MCP server | Manages WooCommerce products and orders (developer preview). | Free |
| [Stripe Agent Toolkit](https://github.com/stripe/agent-toolkit) | MCP server | Payment links, customers, invoices and refunds in Stripe. | Free, needs Stripe account |
| [PayPal Agent Toolkit](https://github.com/paypal/agent-toolkit) | MCP server | PayPal invoices, orders and payment lookups. | Free, needs business account |
| [Square MCP](https://github.com/square/square-mcp-server) | MCP server | Square catalogue, orders, customers and payments. | Free, needs Square account |

## Sales & CRM

Research, prep and pipeline.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [Knowledge Work Plugins: sales](https://github.com/anthropics/knowledge-work-plugins) | Skill collection | Prospect research, call prep, pipeline review and outreach drafts. | Free |
| [Twenty CRM MCP](https://github.com/mhenry3164/twenty-crm-mcp-server) | MCP server | Manages people, companies and tasks in the open-source Twenty CRM. | Free with self-hosted Twenty |
| [Salesforce DX MCP](https://github.com/salesforcecli/mcp) | MCP server | Queries and updates Salesforce data. | Free Developer Edition works |
| [HubSpot MCP](https://developers.hubspot.com/mcp) | MCP server | Searches and updates HubSpot contacts, companies and deals. | Needs HubSpot account; free-CRM support unconfirmed |

## Data

Ask questions of your numbers in plain English.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [DuckDB / MotherDuck MCP](https://github.com/motherduckdb/mcp-server-motherduck) | MCP server | Fast SQL over local CSV, Parquet and Excel files. | Free locally |
| [MCP Toolbox for Databases](https://github.com/googleapis/genai-toolbox) | MCP server | Safe access to Postgres, MySQL, BigQuery and more. | Free |
| [Google Analytics MCP](https://github.com/googleanalytics/google-analytics-mcp) | MCP server | Plain-English questions about your GA4 traffic and conversions. | Free, needs Google Cloud project |
| [Supabase MCP](https://github.com/supabase-community/supabase-mcp) | MCP server | Manages your Supabase database and queries. | Free tier |
| [Knowledge Work Plugins: data](https://github.com/anthropics/knowledge-work-plugins) | Skill collection | SQL, dataset exploration, charts and dashboards. | Free |

## Productivity

Email, calendar, notes, files and memory.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [Filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | MCP server | Reads, writes and organises files in folders you allow. | Free |
| [Memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) | MCP server | A simple long-term memory of people, projects and facts. | Free |
| [Google Workspace MCP](https://github.com/taylorwilsdon/google_workspace_mcp) | MCP server | Gmail, Calendar, Drive, Docs and Sheets from one server. | Free, needs a Google OAuth app |
| [Google Workspace CLI](https://github.com/googleworkspace/cli) | Skill collection | Command-line tool plus 40+ skills for Drive, Gmail, Calendar and Sheets. | Free |
| [Notion MCP](https://github.com/makenotion/notion-mcp-server) | MCP server | Searches, reads and edits Notion pages and databases. | Free, needs Notion account |
| [Obsidian MCP](https://github.com/MarkusPfundstein/mcp-obsidian) | MCP server | Searches and edits notes in your Obsidian vault. | Free |
| [Todoist AI](https://github.com/Doist/todoist-ai) | MCP server | Adds, finds and completes tasks in Todoist. | Free tier |

## Automation & infra

Hosting, deploys and workflows you own.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [Cloudflare MCP servers](https://github.com/cloudflare/mcp-server-cloudflare) | MCP server | Docs, Workers, logs, DNS analytics and browser rendering. | Free, some tools need paid Workers |
| [Cloudflare Skills](https://github.com/cloudflare/skills) | Skill collection | Build and deploy on Cloudflare Workers. | Free |
| [n8n-MCP](https://github.com/czlonkowski/n8n-mcp) | MCP server | Teaches your AI n8n's nodes so it can design and fix workflows. | Free, self-hosted |
| [n8n Skills](https://github.com/czlonkowski/n8n-skills) | Skill collection | Helps your AI build correct n8n automations. | Free |
| [Activepieces](https://github.com/activepieces/activepieces) | MCP server | Open-source automation with 280+ integrations exposed as MCP tools. | Free self-hosted |
| [Docker MCP Gateway](https://github.com/docker/mcp-gateway) | MCP server | Runs many MCP servers safely in containers. | Free |

## Smart home

Local-first control, no cloud needed.

| Tool | Type | What it does | Cost |
|---|---|---|---|
| [Home Assistant MCP Server](https://www.home-assistant.io/integrations/mcp_server/) | MCP server | Built into Home Assistant. Lets any AI control the devices you expose. | Free |
| [ha-mcp](https://github.com/homeassistant-ai/ha-mcp) | MCP server | 80+ tools to control devices and write automations and dashboards. | Free, self-hosted |
| [Home Assistant skill](https://github.com/homeassistant-ai/skills) | Skill | Teaches your AI to write clean, reliable automations. | Free |

## Find more

- [Official MCP Registry](https://registry.modelcontextprotocol.io): The canonical list of published MCP servers.
- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers): The biggest community list, by category.
- [anthropics/skills](https://github.com/anthropics/skills): Official example skills and the spec.
- [skills.sh](https://skills.sh): Skills directory. Install with npx skills add owner/repo.
- [awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills): Cross-agent skills list.
- [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills): Curated skills list.

## No longer free (September 2026)

Posting to X through its API is now pay per post. Medium no longer issues new API tokens. Brave Search ended its free API tier. Tools built on those cost money, so they are flagged or left out.
