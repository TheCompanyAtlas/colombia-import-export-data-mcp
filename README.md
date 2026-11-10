# Colombia Import Export Data MCP

**Colombia Customs Data: Importers, Suppliers & HS Codes.** Colombia import export data for your AI assistant. Search Colombia customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Colombia trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/colombia
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Colombia: the server tells your AI to filter on `CO` unless you ask about another country

## Colombia data coverage

- **Years:** 2024–2026
- **Records:** Import declarations: Colombian importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `CO` (use `buyerCountry: "CO"` for imports into Colombia)
- **Common products:** maize (HS 1005), fertilizers (HS 3105), cars (HS 8703), refined fuel (HS 2710)

## Notable traders in the data

Companies that appear most often in recent Colombia records (by number of declaration lines, not value):

**Importers**

- Ecopetrol
- Automotores Toyota Colombia
- Mazda de Colombia
- Contegral
- Yara Colombia
- ADM Colombia

## Example prompts

- *"Who are the top importers of maize (HS 1005) into Colombia?"*
- *"What does Ecopetrol import, and from which countries?"*
- *"List Colombian importers of fertilizers (HS 3105) in 2025"*
- *"Which suppliers ship cars to Automotores Toyota Colombia?"*
- *"Show recent import shipments for Yara Colombia"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Colombia import data, Colombia export data, Colombia customs data, Colombia shipment data, importers in Colombia, Colombia buyers and suppliers, HS code search, datos de importación Colombia, importadores de Colombia, comercio exterior, partida arancelaria
