# Agent Atlas — AI Agent & Technology Market Intelligence

An interactive, single-page directory of companies building the AI agent ecosystem — from frontier model labs and coding agents to enterprise platforms, AI clouds, data infrastructure, chips, observability and MLOps tooling.

Agent Atlas is designed as a lightweight market-discovery portal for architects, developers, technology leaders, researchers and teams evaluating the AI ecosystem.

## At a glance

| Coverage | Current directory |
|---|---:|
| Directory entries | **250** |
| Unique company names | **249** |
| Market categories | **17** |
| External dependencies | **None required** |
| Build step | **None** |

The directory contains one repeated company name in more than one market segment where that company participates in multiple parts of the ecosystem. Counts may change as the catalog is updated.

## Features

- **Searchable company directory** — search by company, product, category, capability or market annotation.
- **17 market categories** — browse the ecosystem by technology layer and use case.
- **Popularity filters** — filter by High popularity, Moderate popularity, or Less popular / niche.
- **Dynamic filter counts** — popularity counts respond to the selected category.
- **Combined filtering** — category, popularity and text search work together.
- **Sorting** — sort alphabetically, by category or by popularity tier.
- **Company website links** — directory cards link to mapped company-owned websites or official product pages.
- **Market annotations** — each company card includes context explaining its visibility tier and segment.
- **Market landscape overview** — a high-level view of where competition is forming across the agent stack.
- **Vendor evaluation scorecard** — suggested dimensions for comparing vendors beyond brand recognition.
- **Responsive interface** — designed for desktop, tablet and mobile screens.
- **Embedded SVG favicon** — the favicon is contained in the HTML file.
- **Self-contained delivery** — HTML, CSS and JavaScript are bundled into one file; no package installation or build tooling is needed.

## Market categories

| Category | Coverage examples |
|---|---|
| Enterprise platforms | CRM, enterprise workflow, automation and agent platforms |
| Data & AI platforms | Enterprise data platforms and agent development capabilities |
| AI coding agents & app builders | Claude Code, Codex, Cursor, GitHub Copilot, Lovable, Replit, Bolt.new and related tools |
| AI productivity assistants | Workplace and knowledge-worker assistants |
| Integration & observability | Integration platforms, API ecosystems, monitoring and observability |
| AI-native applications | Purpose-built autonomous agents and AI-first applications |
| Developer frameworks | Agent orchestration, multi-agent frameworks and application SDKs |
| Workflow builders | No-code and low-code automation and agent builders |
| Customer & voice agents | Customer support, contact-center and voice agent platforms |
| Sales & GTM agents | Prospecting, sales engagement and revenue workflow agents |
| Vertical agents | Industry-specific agents for legal, healthcare, finance, recruiting, security and other domains |
| Agent infrastructure | Memory, execution, tool integration, tracing and agent runtime infrastructure |
| Frontier model labs | Foundation-model developers and frontier AI research organizations |
| AI cloud & inference | GPU cloud providers, model hosting and inference platforms |
| AI chips & compute | Accelerators, semiconductor companies and AI data-center infrastructure |
| Data & vector infrastructure | Vector databases, search, retrieval and data foundations |
| AI developer & MLOps tooling | Evaluation, testing, deployment, monitoring, security and model operations |

The company list is curated rather than exhaustive. A company's placement reflects the product or market role represented in the directory, not necessarily its entire business.

## Popularity and market visibility

Agent Atlas uses three qualitative visibility tiers:

| Tier | Color treatment | Interpretation |
|---|---|---|
| **High popularity** | Green | Broad public recognition and a strong ecosystem presence |
| **Moderate popularity** | Amber | Established specialist with meaningful visibility in its segment |
| **Less popular / niche** | Purple | Emerging company or more narrowly specialized market visibility |

These tiers are **editorial estimates**, not measured market share, revenue, customer count, product quality, investment advice or a formal analyst ranking. A niche company may have excellent technology or strong adoption in its target market.

The portal intentionally does not assign fabricated market-share percentages. Meaningful share comparisons require a consistent denominator and comparable evidence, such as agent-specific revenue, production deployments or active usage. Vendors often report different metrics that should not be compared directly.

## Run locally

No installation is necessary.

1. Download or clone this repository.
2. Open [`agent_atlas_market_intelligence.html`](https://srinipusuluri.github.io/ai_agent_market_intelligence/) in a modern web browser.
3. Search the directory, select a category, choose a popularity tier, or change the sort order.

The portal is a static client-side page. It does not require a backend, API key, database or environment variables.

## Publish with GitHub Pages

You can host the portal as a static GitHub Pages site:

1. Add `agent_atlas_market_intelligence.html` and `README.md` to the repository root.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select the branch containing the files and choose the `/ (root)` folder.
5. Save the settings and use the Pages URL shown by GitHub after deployment.

Optionally, rename the HTML file to `index.html` so the portal opens automatically at the repository's GitHub Pages root URL. Update references to the filename in this README if you do so.

## Repository structure

```text
.
├── README.md
└── agent_atlas_market_intelligence.html
```

The HTML file contains:

- Page markup and navigation
- Embedded CSS and responsive styling
- Embedded JavaScript directory data and filter behavior
- Company website URL mapping
- Popularity-tier classification and annotations
- Embedded SVG favicon

## Updating the directory

The source data is maintained in the JavaScript section of `agent_atlas_market_intelligence.html`.

When adding or editing a company:

1. Add or update its entry in the `data` array. Each entry follows this structure:

   ```javascript
   [
     "Company name",
     "Product or platform",
     "Market category",
     "Short description",
     "Card monogram"
   ]
   ```

2. Add the company's direct official homepage or official product URL to `officialProfiles`.
3. Assign its visibility tier in `highVisibility` or `lowVisibility`. Companies in neither set default to Moderate popularity.
4. Confirm the category exists in the category annotation map inside `popularityAnnotation()`; add a concise note for any new category.
5. Test search, category filters, popularity filters, sorting, reset behavior and the external website link.
6. Check that the company name and URL are correct and that the product is still current before submitting the change.

Avoid using search-engine result URLs as company profile links. Prefer the company's own domain or an official product page. If a direct URL cannot be confirmed, leave it unlinked until verified rather than pointing users to an unrelated destination.

## Suggested vendor evaluation dimensions

Popularity alone is not enough to choose an agent platform. For a technical or procurement assessment, compare vendors using consistent criteria:

- **Product fit:** supported workflows, agent types, tools, integrations and target users.
- **Model strategy:** supported frontier and open models, routing, fallback and portability.
- **Enterprise readiness:** SSO, RBAC, audit logs, data residency, compliance and SLAs.
- **Agent reliability:** evaluations, test datasets, tracing, monitoring, guardrails and human approvals.
- **Data integration:** connectors, retrieval, permissions-aware grounding and data freshness.
- **Operations:** deployment model, latency, scalability, availability and incident response.
- **Commercial traction:** independently supportable revenue, customers, production deployments and usage.
- **Vendor risk:** financial health, roadmap, lock-in, portability and support model.

## Data quality and research notes

- Company products, names, ownership, URLs and availability change frequently.
- A directory entry indicates market presence, not an endorsement or proof of production maturity.
- Official website links should be periodically checked for redirects, product renames and shutdowns.
- Funding, valuation, headcount, ARR and customer metrics should only be added with a dated source and clear attribution.
- Market-share claims should identify the research firm, publication date, market definition, geography and denominator.
- The portal's market landscape bars are illustrative editorial indicators, not quantitative market-share measurements.

## Contributing

Contributions are welcome, especially corrections to company names, official URLs, product descriptions and category placement.

Please include the following with a proposed update:

- Company and product name
- Official company or product URL
- Recommended market category
- One-sentence factual description
- Source link and date for time-sensitive claims

Keep descriptions neutral and concise. Do not add unsupported market-share percentages or treat popularity tiers as objective rankings.

## License

No license is currently specified in this repository. Unless a license is added, the default copyright protections apply; please do not assume that reuse, redistribution or modification is permitted.

---

**Agent Atlas** · AI agent and technology market intelligence · Curated research edition, November 2026
