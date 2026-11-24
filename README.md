# AU Agent Tools (MCP): PDF to Markdown, screenshots, Australian addresses, AU/NZ holidays, phone validation

5 pay-per-use tools for AI agents, served through the hosted Apify MCP server. No install: add one URL to your MCP client.

```
https://mcp.apify.com/?tools=geeky_goth_gamer/pdf-docx-to-markdown,geeky_goth_gamer/url-to-screenshot-pdf,geeky_goth_gamer/au-nz-address-parser-geocoder,geeky_goth_gamer/au-nz-public-holidays-business-days,geeky_goth_gamer/phone-number-validator-extractor
```

Claude Code:

```bash
claude mcp add --transport http au-agent-tools "https://mcp.apify.com/?tools=geeky_goth_gamer/pdf-docx-to-markdown,geeky_goth_gamer/url-to-screenshot-pdf,geeky_goth_gamer/au-nz-address-parser-geocoder,geeky_goth_gamer/au-nz-public-holidays-business-days,geeky_goth_gamer/phone-number-validator-extractor"
```

Cursor / VS Code / Claude Desktop (`mcp.json`):

```json
{"mcpServers": {"au-agent-tools": {"url": "https://mcp.apify.com/?tools=geeky_goth_gamer/pdf-docx-to-markdown,geeky_goth_gamer/url-to-screenshot-pdf,geeky_goth_gamer/au-nz-address-parser-geocoder,geeky_goth_gamer/au-nz-public-holidays-business-days,geeky_goth_gamer/phone-number-validator-extractor"}}}
```

Sign in with your Apify account when the client asks (OAuth), or send `Authorization: Bearer <APIFY_TOKEN>`. A free Apify account includes $5 of monthly credit. Agents without an account can buy a prepaid token at https://agi.apify.com.

## Tools

| Tool | What it does | MCP tool name |
|---|---|---|
| [PDF & DOCX to Markdown](https://apify.com/geeky_goth_gamer/pdf-docx-to-markdown) | Convert PDF and Word files at URLs into clean Markdown for LLMs and RAG. | `geeky_goth_gamer--pdf-docx-to-markdown` |
| [Website Screenshot & URL to PDF](https://apify.com/geeky_goth_gamer/url-to-screenshot-pdf) | Full-page website screenshots and web page to PDF with real Chrome, ads and cookie banners hidden. | `geeky_goth_gamer--url-to-screenshot-pdf` |
| [Australian Address Validator & Geocoder](https://apify.com/geeky_goth_gamer/au-nz-address-parser-geocoder) | Validate, standardise and geocode Australian addresses with official G-NAF data; parse NZ. | `geeky_goth_gamer--au-nz-address-parser-geocoder` |
| [AU & NZ Public Holidays & Business Days](https://apify.com/geeky_goth_gamer/au-nz-public-holidays-business-days) | AU/NZ public holidays by state, Tasmanian area and NZ region; add or count business days. | `geeky_goth_gamer--au-nz-public-holidays-business-days` |
| [Phone Number Validator & Formatter](https://apify.com/geeky_goth_gamer/phone-number-validator-extractor) | Validate, format (E.164) and extract phone numbers in bulk for 240+ countries. | `geeky_goth_gamer--phone-number-validator-extractor` |

Each tool's input schema is described for LLMs: required fields, formats and an example input. Results come back as JSON dataset items (use `get-dataset-items` with the run's `datasetId`).

## When to use which

- Have a PDF/DOCX link and need its text? **PDF & DOCX to Markdown** ($0.001/page).
- Need to see or archive a web page? **Website Screenshot & URL to PDF** ($0.0075/file).
- Messy Australian addresses, missing postcodes, need lat/long? **Australian Address Validator & Geocoder** (from $0.0005/address).
- Due date N business days out, or public holidays in an AU state / NZ region? **AU & NZ Public Holidays** (from $0.0003/date).
- Cleaning a phone list or pulling numbers out of text? **Phone Number Validator** ($0.0005/valid number).


Pricing is pay-per-event on Apify; you only pay for results. Source of the hosted server: https://github.com/apify/apify-mcp-server.

## License

MIT for this listing repository. The tools run on Apify under the Apify terms.
