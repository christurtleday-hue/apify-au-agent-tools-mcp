# AU Agent Tools (MCP): documents, screenshots, data, verification and AU/NZ utilities

[![Glama](https://glama.ai/mcp/connectors/io.github.christurtleday-hue/au-agent-tools/badges/score.svg)](https://glama.ai/mcp/connectors/io.github.christurtleday-hue/au-agent-tools)
[![mcptry](https://mcptry.com/badge/io.github.christurtleday-hue/au-agent-tools)](https://mcptry.com/servers/io.github.christurtleday-hue/au-agent-tools)

11 pay-per-use tools for AI agents, served through the hosted Apify MCP server. Global document, data and verification tools come first; Australian and New Zealand utilities follow. No install: add one URL to your MCP client.

```
https://mcp.apify.com/?tools=geeky_goth_gamer/pdf-docx-to-markdown,geeky_goth_gamer/url-to-screenshot-pdf,geeky_goth_gamer/phone-number-validator-extractor,geeky_goth_gamer/cited-evidence-pack,geeky_goth_gamer/ai-context-distiller,geeky_goth_gamer/live-link-citation-verifier,geeky_goth_gamer/spreadsheet-json-query-engine,geeky_goth_gamer/page-doc-semantic-diff,geeky_goth_gamer/validated-table-invoice-extractor,geeky_goth_gamer/au-nz-address-parser-geocoder,geeky_goth_gamer/au-nz-public-holidays-business-days
```

## MCP setup

Claude Code:

```bash
claude mcp add --transport http au-agent-tools "https://mcp.apify.com/?tools=geeky_goth_gamer/pdf-docx-to-markdown,geeky_goth_gamer/url-to-screenshot-pdf,geeky_goth_gamer/phone-number-validator-extractor,geeky_goth_gamer/cited-evidence-pack,geeky_goth_gamer/ai-context-distiller,geeky_goth_gamer/live-link-citation-verifier,geeky_goth_gamer/spreadsheet-json-query-engine,geeky_goth_gamer/page-doc-semantic-diff,geeky_goth_gamer/validated-table-invoice-extractor,geeky_goth_gamer/au-nz-address-parser-geocoder,geeky_goth_gamer/au-nz-public-holidays-business-days"
```

Cursor / VS Code / Claude Desktop (`mcp.json`):

```json
{"mcpServers": {"au-agent-tools": {"url": "https://mcp.apify.com/?tools=geeky_goth_gamer/pdf-docx-to-markdown,geeky_goth_gamer/url-to-screenshot-pdf,geeky_goth_gamer/phone-number-validator-extractor,geeky_goth_gamer/cited-evidence-pack,geeky_goth_gamer/ai-context-distiller,geeky_goth_gamer/live-link-citation-verifier,geeky_goth_gamer/spreadsheet-json-query-engine,geeky_goth_gamer/page-doc-semantic-diff,geeky_goth_gamer/validated-table-invoice-extractor,geeky_goth_gamer/au-nz-address-parser-geocoder,geeky_goth_gamer/au-nz-public-holidays-business-days"}}}
```

Sign in with your Apify account when the client asks (OAuth), or send `Authorization: Bearer <APIFY_TOKEN>`. A free Apify account includes $5 of monthly credit. Agents without an account can buy a prepaid token at https://agi.apify.com.

## Tools

Global tools first, then AU/NZ.

| Tool | What it does | Price (USD) | MCP tool name |
|---|---|---|---|
| [PDF & DOCX to Markdown](https://apify.com/geeky_goth_gamer/pdf-docx-to-markdown) | Convert PDF and Word files at URLs into clean Markdown for LLMs and RAG. | $0.003/page | `geeky_goth_gamer--pdf-docx-to-markdown` |
| [Website Screenshot & URL to PDF](https://apify.com/geeky_goth_gamer/url-to-screenshot-pdf) | Full-page website screenshots and web page to PDF with real Chrome, ads and cookie banners hidden. | $0.01/file | `geeky_goth_gamer--url-to-screenshot-pdf` |
| [Phone Number Validator & Formatter](https://apify.com/geeky_goth_gamer/phone-number-validator-extractor) | Validate, format (E.164) and extract phone numbers in bulk for 240+ countries. | $0.0015/valid number; $0.0003/invalid | `geeky_goth_gamer--phone-number-validator-extractor` |
| [Cited Evidence Pack for AI Agents](https://apify.com/geeky_goth_gamer/cited-evidence-pack) | Question + URLs in, compact pack of verbatim cited quotes, gaps and a claim check out. | $0.025/pack | `geeky_goth_gamer--cited-evidence-pack` |
| [AI Context Distiller](https://apify.com/geeky_goth_gamer/ai-context-distiller) | Cut tokens from HTML, JSON, logs and public URLs into compact context for LLMs. | $0.0025/payload; $0.005/URL | `geeky_goth_gamer--ai-context-distiller` |
| [Live Link & Citation Verifier](https://apify.com/geeky_goth_gamer/live-link-citation-verifier) | Check live URLs, verify citations against pages, and look up PyPI or npm packages. | $0.0015/URL; $0.003/citation; $0.0005/package | `geeky_goth_gamer--live-link-citation-verifier` |
| [Spreadsheet & JSON Query Engine](https://apify.com/geeky_goth_gamer/spreadsheet-json-query-engine) | Profile, query and diff CSV, Excel, JSON or NDJSON from text or a public URL. | $0.003/inline; $0.005/URL | `geeky_goth_gamer--spreadsheet-json-query-engine` |
| [Page & Document Semantic Diff](https://apify.com/geeky_goth_gamer/page-doc-semantic-diff) | Semantic, structured or strict diffs of pages and documents, inline or from URLs. | $0.003/inline; $0.006/URL | `geeky_goth_gamer--page-doc-semantic-diff` |
| [Validated Table & Invoice Extractor](https://apify.com/geeky_goth_gamer/validated-table-invoice-extractor) | Extract typed tables and invoice fields from HTML, Markdown, CSV, text or PDFs. | $0.005/inline; $0.01/document | `geeky_goth_gamer--validated-table-invoice-extractor` |
| [Australian Address Validator & Geocoder](https://apify.com/geeky_goth_gamer/au-nz-address-parser-geocoder) | Validate, standardise and geocode Australian addresses with official G-NAF data; parse NZ. | from $0.001/address; $0.003 if geocoded | `geeky_goth_gamer--au-nz-address-parser-geocoder` |
| [AU & NZ Public Holidays & Business Days](https://apify.com/geeky_goth_gamer/au-nz-public-holidays-business-days) | AU/NZ public holidays by state, Tasmanian area and NZ region; add or count business days. | $0.004/calendar; $0.001/date calculation | `geeky_goth_gamer--au-nz-public-holidays-business-days` |

Each tool also charges `apify-actor-start` at $0.00005 per run start. Failed or rejected inputs are free as described on each Actor's Store page. Each tool's input schema is described for LLMs: required fields, formats and an example input. Results come back as JSON dataset items (use `get-dataset-items` with the run's `datasetId`).

## When to use which

- Have a PDF/DOCX link and need its text? **PDF & DOCX to Markdown** ($0.003/page).
- Need to see or archive a web page? **Website Screenshot & URL to PDF** ($0.01/file).
- Cleaning a phone list or pulling numbers out of text? **Phone Number Validator** ($0.0015/valid number, $0.0003/invalid).
- Answering a question or checking a claim from given web pages with citations? **Cited Evidence Pack** ($0.025/pack).
- Need to shrink HTML, JSON or logs before they hit an LLM? **AI Context Distiller** ($0.0025/payload, $0.005/URL).
- Need to know if a link is live or if a quote is still on the page? **Live Link & Citation Verifier** ($0.0015/URL, $0.003/citation, $0.0005/package).
- Want to profile, query or diff a spreadsheet or JSON file? **Spreadsheet & JSON Query Engine** ($0.003/inline, $0.005/URL).
- Comparing two pages or documents for what actually changed? **Page & Document Semantic Diff** ($0.003/inline, $0.006/URL).
- Extracting tables or invoice fields from a page or PDF? **Validated Table & Invoice Extractor** ($0.005/inline, $0.01/document).
- Messy Australian addresses, missing postcodes, need lat/long? **Australian Address Validator & Geocoder** (from $0.001/address, $0.003 if geocoded).
- Due date N business days out, or public holidays in an AU state / NZ region? **AU & NZ Public Holidays** ($0.004/calendar, $0.001/date).

Pricing is pay-per-event on Apify; you only pay for results. Source of the hosted server: https://github.com/apify/apify-mcp-server.

Listings: [Apify Store](https://apify.com/geeky_goth_gamer) · [Official MCP Registry](https://registry.modelcontextprotocol.io/v0/servers?search=io.github.christurtleday-hue/au-agent-tools) · [Glama](https://glama.ai/mcp/connectors/io.github.christurtleday-hue/au-agent-tools) · [mcptry](https://mcptry.com/servers/io.github.christurtleday-hue/au-agent-tools)

## License

MIT for this listing repository. The tools run on Apify under the Apify terms.
