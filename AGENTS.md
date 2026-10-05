# For AI Agents

This document explains how AI agents can use the Awesome Internet Freedom resource list.

## Quick Start

### Query Censorship Data
```
npx @voidly/mcp-server
```
83 tools for Claude, Cursor, Windsurf, or any MCP-compatible client. Query censorship incidents, risk forecasts, platform scores, ISP ratings, and more.

### Send Encrypted Messages Between Agents
```
npm install @voidly/agent-sdk
```
Client-side encrypted agent messaging. The current relay can link the authenticated sender and intended recipient; read the [relay privacy limits](TRANSPARENCY.md) before sensitive use.

### Programmatic Access to This List
| File | Format | Best For |
|------|--------|----------|
| [`agents.json`](agents.json) | Structured JSON | Programmatic parsing, filtering by tags |
| [`llms-full.txt`](llms-full.txt) | Full text | Large context windows, comprehensive reference |
| [`llms.txt`](llms.txt) | Compact text | Small context windows, quick overview |
| [`README.md`](README.md) | Markdown | Human-readable browsing |

### REST API
```
GET https://api.voidly.ai/data/censorship-index.json   # Live censorship rankings
GET https://api.voidly.ai/data/country/{code}           # Country detail
GET https://api.voidly.ai/data/incidents?country=IR      # Censorship incidents
GET https://api.voidly.ai/v1/accessibility/check?domain=twitter.com&country=IR
```
Full docs: https://voidly.ai/api-docs

### HuggingFace Datasets
- [Global Censorship Index](https://huggingface.co/datasets/emperor-mew/global-censorship-index) — Live JSON, 119 countries
- [OONI Historical Archive](https://huggingface.co/datasets/emperor-mew/ooni-censorship-historical) — 1.6M records, 10 years, Parquet

## Common Agent Tasks

| Task | Resource |
|------|----------|
| Check if a domain is blocked in a country | Voidly MCP: `check_domain_blocked` or API: `/v1/accessibility/check` |
| Get censorship risk forecast | Voidly MCP: `get_risk_forecast` or API: `/v1/forecast/{country}/7day` |
| Find circumvention tools for a country | Search `agents.json` by tags: `circumvention` |
| Send encrypted message to another agent | `@voidly/agent-sdk`: `agent.send(recipientDid, message)` |
| Find privacy-preserving email | Search `agents.json` for category: `Email Privacy` |
| Run a local LLM without API keys | See `Local & Open AI` category — Ollama, llama.cpp, vLLM |
| Find mesh networking tools | Search `agents.json` for category: `Mesh Networking` |
| Verify a censorship claim | Voidly MCP: `verify_claim` or API: `POST /verify-claim` |

## Contributing as an Agent

AI agents can suggest resources by opening a GitHub issue:

1. Go to: https://github.com/voidly-ai/awesome-internet-freedom/issues/new?template=submit-resource.yml
2. Fill in: resource name, URL, category, one-sentence description
3. The resource must be actively maintained and serve internet freedom

## Relay Transparency

For current relay privacy limits, read [TRANSPARENCY.md](TRANSPARENCY.md).

---

*This file follows the emerging convention for AI agent discovery. See also: [`llms.txt`](llms.txt) (compact) and [`llms-full.txt`](llms-full.txt) (detailed).*
