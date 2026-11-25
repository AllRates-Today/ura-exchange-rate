# Uganda Revenue Authority Exchange Rates API — ura-exchange-rate

[![npm version](https://img.shields.io/npm/v/ura-exchange-rate.svg)](https://www.npmjs.com/package/ura-exchange-rate)
[![license](https://img.shields.io/npm/l/ura-exchange-rate.svg)](https://github.com/AllRates-Today/ura-exchange-rate/blob/main/LICENSE)
[![zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://www.npmjs.com/package/ura-exchange-rate)
[![TypeScript](https://img.shields.io/badge/TypeScript-types%20included-3178C6.svg)](https://www.typescriptlang.org/)
[![USD/UGX today](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fura%3Fsource%3DUSD%26target%3DUGX&query=%24.rate&label=USD%2FUGX%20official%2C%20Uganda%20Revenue%20Authority&color=0A7E8C&cacheSeconds=3600)](https://allratestoday.com/tax-authority-rates-api/ura/)
[![rate date](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fura%3Fsource%3DUSD%26target%3DUGX&query=%24.rate_date&label=rate%20date&color=555&cacheSeconds=3600)](https://allratestoday.com/tax-authority-rates-api/ura/)

**Official Uganda Revenue Authority (Uganda) daily exchange rates for Node.js and TypeScript. The published tax authority rates behind tax filings, customs valuations, audits, and compliant invoicing — not market estimates, but the numbers Uganda Revenue Authority itself prints, every business day.**

## 🚀 Why this client?

- 🏛️ **Official rates** — Uganda Revenue Authority's own table, with the publisher's own `rate_date` on every response
- 📅 **History back to 2005** — point-in-time tables and daily series for any past date
- 🔀 **Official vs derived, always flagged** — computed inverse/cross pairs carry `derived: true`, never mixed with official prints
- ⚡ **Zero dependencies** — pure ESM + CJS over global `fetch`; Node 18+, Bun, Deno, and edge runtimes
- 🔷 **Type-safe** — full TypeScript definitions shipped with the package
- 🧾 **Compliance-grade metadata** — `rate_type`, publication date, and source disclaimer on every response

> **Official rate, not mid-market:** every value here is a number Uganda Revenue Authority itself published, fixed once printed and carrying the tax authority's own `rate_date` — what filings and audits require. Need the live mid-market rate for pricing or display instead? Use the [mid-market API](https://allratestoday.com/docs/) or [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk). The two can diverge by several percent.

## 🔑 Get your API key

Get a free API key at [allratestoday.com/register](https://allratestoday.com/register) — no credit card required. Latest rates are on every plan, including free.

## 📈 Latest official table

[![Latest Uganda Revenue Authority table](https://allratestoday.com/api/open/central-bank/ura/table.svg)](https://allratestoday.com/tax-authority-rates-api/ura/)

The image is rendered live from the keyless endpoint, so it follows the tax authority's publications on npm and on GitHub alike without a new release. The same table as text is folded below for search and copy-paste: on GitHub [a daily Action](.github/workflows/daily-table.yml) refreshes it whenever the tax authority publishes a new table; on npm it is as of the package's publish date.

<!-- daily-table:start -->
<details>
<summary>Table as text: published 2026-11-25 by Uganda Revenue Authority — 285 rates, first 60 shown. Updated 2026-11-25.</summary>

| Base | Quote | Type | Rate |
| --- | --- | --- | ---: |
| AED | UGX | export | 1118.4141 |
| AED | UGX | import | 1129.3051 |
| AED | UGX | income_tax | 1155.4158 |
| AED | UGX | vat | 1129.3051 |
| AUD | UGX | export | 2866.7187 |
| AUD | UGX | import | 2894.6307 |
| AUD | UGX | income_tax | 2813.2813 |
| AUD | UGX | vat | 2894.6307 |
| BHD | UGX | export | 10924.6394 |
| BHD | UGX | import | 11031.0224 |
| BHD | UGX | income_tax | 11286.9681 |
| BHD | UGX | vat | 11031.0224 |
| BIF | UGX | export | 1.3693 |
| BIF | UGX | import | 1.3827 |
| BIF | UGX | income_tax | 1.4088 |
| BIF | UGX | vat | 1.3827 |
| BND | UGX | export | 3207.4437 |
| BND | UGX | import | 3238.6774 |
| BND | UGX | income_tax | 3318.4631 |
| BND | UGX | vat | 3238.6774 |
| BRL | UGX | export | 792.7891 |
| BRL | UGX | import | 800.5092 |
| BRL | UGX | income_tax | 780.382 |
| BRL | UGX | vat | 800.5092 |
| BWP | UGX | export | 290.9931 |
| BWP | UGX | import | 293.8268 |
| BWP | UGX | income_tax | 307.4032 |
| BWP | UGX | vat | 293.8268 |
| CAD | UGX | export | 2901.0436 |
| CAD | UGX | import | 2929.2876 |
| CAD | UGX | income_tax | 2955.6709 |
| CAD | UGX | vat | 2929.2876 |
| CDF | UGX | export | 1.777 |
| CDF | UGX | import | 1.7943 |
| CDF | UGX | income_tax | 1.8249 |
| CDF | UGX | vat | 1.7943 |
| CHF | UGX | export | 4957.4451 |
| CHF | UGX | import | 5005.7149 |
| CHF | UGX | income_tax | 5044.7548 |
| CHF | UGX | vat | 5005.7149 |
| CLP | UGX | export | 4.2193 |
| CLP | UGX | import | 4.2604 |
| CLP | UGX | income_tax | 4.3412 |
| CLP | UGX | vat | 4.2604 |
| CNY | UGX | export | 614.0847 |
| CNY | UGX | import | 620.0642 |
| CNY | UGX | income_tax | 637.1027 |
| CNY | UGX | vat | 620.0642 |
| COP | UGX | export | 1.2406 |
| COP | UGX | import | 1.2527 |
| COP | UGX | income_tax | 1.3235 |
| COP | UGX | vat | 1.2527 |
| CRC | UGX | export | 8.9894 |
| CRC | UGX | import | 9.077 |
| CRC | UGX | income_tax | 9.3477 |
| CRC | UGX | vat | 9.077 |
| CZK | UGX | export | 189.7009 |
| CZK | UGX | import | 191.5482 |
| CZK | UGX | income_tax | 195.4186 |
| CZK | UGX | vat | 191.5482 |

</details>

[Full table on the Uganda Revenue Authority rates page](https://allratestoday.com/tax-authority-rates-api/ura/) · Source: [Official rates published by URA, served by AllRatesToday](https://allratestoday.com/tax-authority-rates-api/ura/). Rates are as printed by the tax authority; AllRatesToday is not affiliated with it.
<!-- daily-table:end -->

## 📦 Installation

```bash
npm install ura-exchange-rate
```

```bash
yarn add ura-exchange-rate
```

```bash
pnpm add ura-exchange-rate
```

Requires Node 18+ (global `fetch`); also runs on Bun, Deno and edge runtimes. Also published under the org scope as [`@allratestoday/ura-exchange-rate`](https://www.npmjs.com/package/@allratestoday/ura-exchange-rate) — same code, same versions.

## 🏁 Quick start

```js
import { getRate } from 'ura-exchange-rate';

const pair = await getRate('USD', 'UGX', { apiKey: 'art_live_...' });
console.log(pair.rate, pair.rate_date); // the official Uganda Revenue Authority rate, on the tax authority's own date
```

## 📚 API reference

- [Latest pair rate](#latest-pair-rate) — one pair from the latest official table
- [Full official table](#full-official-table) — everything the tax authority printed, in one call
- [Table for a date](#table-for-a-date) — the official table for an invoice or filing date
- [Daily time series](#daily-time-series) — one pair across a date range

---

### Latest pair rate

Free plan and up. Pairs the tax authority does not print directly are resolved from its table and flagged (see *Official vs derived rates* below).

```js
const pair = await getRate('USD', 'UGX', { apiKey: 'art_live_...' });
```

**Response:**

```javascript
{
  bank: 'ura',
  name: 'Uganda Revenue Authority',
  rate_date: '2026-11-25',   // Uganda Revenue Authority's own publication date
  source: 'USD',
  target: 'UGX',
  rate: 4107.6644,
  rate_type: 'export',
  derived: false,
  method: 'published',
  disclaimer: 'Official rates as published by the named central bank. On weekends/holidays the most recent published rate_date is returned.'
}
```

### Full official table

Free plan and up. The complete table for the latest publication date.

```js
import { getLatestRates } from 'ura-exchange-rate';

const table = await getLatestRates({ apiKey: 'art_live_...' });
console.log(table.rate_date, table.rates.length);
```

**Response:**

```javascript
{
  bank: 'ura',
  name: 'Uganda Revenue Authority',
  rate_date: '2026-11-25',
  rates: [
    { "base": "USD", "quote": "UGX", "type": "export", "value": 4107.6644 },
    { "base": "USD", "quote": "UGX", "type": "import", "value": 4147.6644 },
    { "base": "USD", "quote": "UGX", "type": "income_tax", "value": 4243.9 },
    { "base": "USD", "quote": "UGX", "type": "vat", "value": 4147.6644 },
    // … the rest of the official table (72 currencies vs UGX)
  ],
  disclaimer: '…'
}
```

### Table for a date

Paid plans. The official table for any date since 2005 — weekends and holidays return the most recent published date, flagged via `published_on_requested_date`, which is exactly the in-force rate a filing needs.

```js
import { getRatesForDate } from 'ura-exchange-rate';

const day = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...' });
// Optionally narrow to one pair:
const one = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...', source: 'USD', target: 'UGX' });
```

**Response:**

```javascript
{
  bank: 'ura',
  requested_date: '2026-06-30',
  rate_date: '2026-06-30',                // the date actually published
  published_on_requested_date: true,      // false when a weekend/holiday fell back
  rates: [ /* the full table for that date */ ],
  disclaimer: '…'
}
```

### Daily time series

Paid plans. One resolved rate per publication date — ready for charting, revaluation runs, or audit workpapers.

```js
import { getHistory } from 'ura-exchange-rate';

const series = await getHistory(
  { source: 'USD', target: 'UGX', from: '2026-01-01', to: '2026-11-25' },
  { apiKey: 'art_live_...' }
);
```

**Response:**

```javascript
{
  bank: 'ura',
  source: 'USD',
  target: 'UGX',
  from: '2026-01-01',
  to: '2026-11-25',
  count: 152,
  rates: [
    // one entry per publication date
    { date: '2026-11-25', rate: 4107.6644, rate_type: 'export', derived: false, method: 'published' },
    // …
  ],
  disclaimer: '…'
}
```

Pass `{ symbol: 'USD' }` instead of `source`/`target` to get the raw published rows for one currency (all rate types, no pair resolution).

---

## 🗺️ Currencies covered

Uganda Revenue Authority currently publishes rates covering **72 currencies** against the UGX (as of the latest table):

🇦🇪 `AED` · 🇦🇺 `AUD` · 🇧🇭 `BHD` · 🇧🇮 `BIF` · 🇧🇳 `BND` · 🇧🇷 `BRL` · 🇧🇼 `BWP` · 🇨🇦 `CAD` · 🇨🇩 `CDF` · 🇨🇭 `CHF` · 🇨🇱 `CLP` · 🇨🇳 `CNY` · 🇨🇴 `COP` · 🇨🇷 `CRC` · 🇨🇿 `CZK` · 🇩🇯 `DJF` · 🇩🇰 `DKK` · 🇩🇴 `DOP` · 🇪🇬 `EGP` · 🇪🇹 `ETB` · 🇪🇺 `EUR` · 🇬🇧 `GBP` · 🇬🇭 `GHS` · 🇭🇰 `HKD` · 🇭🇺 `HUF` · 🇮🇩 `IDR` · 🇮🇱 `ILS` · 🇮🇳 `INR` · 🇮🇷 `IRR` · 🇯🇴 `JOD` · 🇯🇵 `JPY` · 🇰🇪 `KES` · 🇰🇲 `KMF` · 🇰🇷 `KRW` · 🇰🇼 `KWD` · 🇱🇧 `LBP` · 🇱🇰 `LKR` · 🇱🇸 `LSL` · 🇱🇾 `LYD` · 🇲🇦 `MAD` · 🇲🇺 `MUR` · 🇲🇼 `MWK` · 🇲🇽 `MXN` · 🇲🇾 `MYR` · 🇳🇦 `NAD` · 🇳🇬 `NGN` · 🇳🇴 `NOK` · 🇳🇿 `NZD` · 🇴🇲 `OMR` · 🇵🇪 `PEN` · 🇵🇭 `PHP` · 🇵🇰 `PKR` · 🇵🇱 `PLN` · 🇶🇦 `QAR` · 🇷🇺 `RUB` · 🇷🇼 `RWF` · 🇸🇦 `SAR` · 🇸🇩 `SDG` · 🇸🇪 `SEK` · 🇸🇬 `SGD` · 🇸🇾 `SYP` · 🇸🇿 `SZL` · 🇹🇭 `THB` · 🇹🇷 `TRY` · 🇹🇼 `TWD` · 🇹🇿 `TZS` · 🇺🇸 `USD` · 🇺🇾 `UYU` · 🇻🇳 `VND` · `XAF` · 🇿🇦 `ZAR` · 🇿🇲 `ZMW`

## 🏛️ Source

The exchange rates the Uganda Revenue Authority prescribes by legal use: a monthly table for converting import values (customs duty), export values and VAT, and a daily table for income-tax purposes, all in Uganda shillings per unit of about 75 currencies. Taxpayers and customs declarants must use the URA rate for the relevant month or day when converting foreign-currency amounts for duty, VAT and income-tax computations.

- Publisher's own page: [Customs, VAT and income-tax exchange rates](https://ura.go.ug/en/exchange-rates/) · [ura.go.ug](https://ura.go.ug/)
- Publication: every business day; the exact schedule, freshness status and any current delay are on the [Uganda Revenue Authority rates page](https://allratestoday.com/tax-authority-rates-api/ura/)
- Values are stored unmodified, with the publisher's own `rate_date` on every row — see the [methodology](https://allratestoday.com/official-rates-methodology/)

## 🧭 Reading the numbers

- `value` is always **quote currency per 1 unit of base currency** (`base: "EUR", quote: "USD", value: 1.15` means 1 EUR = 1.15 USD).
- Uganda Revenue Authority quotes **UGX per 1 unit of foreign currency** (e.g. `base: "USD", quote: "UGX"` means UGX per one US dollar).
- Need the other way round? Ask `getRate(target, source)` and the API inverts or crosses for you, flagged `derived: true` — never divide a published rate yourself in a compliance workflow.
- `rate_type` tells you which of the tax authority's series a row belongs to (`export` here); some publishers print buy/sell or several fixings for the same pair.

## 🧩 ERP & accounting systems

Loading the official Uganda Revenue Authority rate into an accounting system is a supported workflow, not a hack. Step-by-step guides with the direction each system expects:

- [Dynamics 365 Business Central](https://allratestoday.com/docs/integrations/business-central/) — built-in Currency Exchange Rate Service, no code
- [Xero](https://allratestoday.com/docs/integrations/xero/) · [QuickBooks Online](https://allratestoday.com/docs/integrations/quickbooks/) · [SAP S/4HANA and ECC](https://allratestoday.com/docs/integrations/sap/) · [Odoo](https://allratestoday.com/docs/integrations/odoo/)

The same keyed endpoints return `?format=csv`, `?format=xml` and `?format=xlsx`, and accept the key as `?api_key=` on the URL for importers that cannot send headers:

```bash
curl "https://allratestoday.com/api/v1/central-bank/ura/latest?format=xml&api_key=art_live_..."
```

## 🤖 AI agents

- MCP server: `npx -y @allratestoday/central-bank-mcp` (stdio) or the hosted endpoint `https://allratestoday.com/api/mcp` — tools for official rates, history, cross-bank comparison and publication calendars
- Already using the general SDK or MCP server? Since 2026-10-01 [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk) 1.4+ has `officialRates('ura')` and [`@allratestoday/mcp-server`](https://www.npmjs.com/package/@allratestoday/mcp-server) 0.6+ has a `get_official_rates` tool — both return this source's latest table with no key, so you can add it without a second dependency
- Claude Code plugin (no key): `/plugin marketplace add AllRates-Today/claude-code-plugin` then `/plugin install allratestoday@allratestoday` — bundles both MCP servers plus an `/official-rate ura ...` command
- Evaluating? Agents can self-issue a trial key with no signup: `POST https://allratestoday.com/api/agent/keys` (send `Content-Type: application/json`) returns a 100-call key valid 7 days that covers the free-plan methods (latest table, pairs); dated tables and history need a [paid plan](https://allratestoday.com/pricing/). The MCP servers expose it as `request_trial_key`
- Machine-readable site guide: [llms.txt](https://allratestoday.com/llms.txt) · [for-ai-agents](https://allratestoday.com/for-ai-agents/)

## ⚖️ Official vs derived rates

If Uganda Revenue Authority does not print a pair directly, the API resolves it from the tax authority's own table and says so — official and computed values are never confused:

| `method` | `derived` | Meaning |
| --- | --- | --- |
| `published` | `false` | The tax authority printed this pair directly |
| `inverse` | `true` | Computed as 1 ÷ the published opposite direction |
| `cross` | `true` | Computed via UGX from two published rates |

## 🛡️ Error handling

Errors are thrown as `Error` with `status` (HTTP code) and `body` (the API's JSON error) attached:

```js
try {
  const pair = await getRate('USD', 'XXX', { apiKey: 'art_live_...' });
} catch (err) {
  console.log(err.message); // human-readable reason
  console.log(err.status);  // e.g. 404
}
```

| Status | Meaning |
| ------ | ------- |
| — | Missing `apiKey` (thrown before any request) |
| `400` | Malformed date or parameters |
| `401` | Invalid API key |
| `403` | Endpoint needs a [paid plan](https://allratestoday.com/pricing/) (historical dates & series) |
| `404` | Pair or date range not covered by Uganda Revenue Authority |
| `429` | Monthly quota exceeded |

## 🔷 TypeScript

Full definitions ship with the package — no `@types` install:

```ts
import type { LatestRates, PairRate, DatedRates, RateEntry, HistoryQuery, RequestOptions } from 'ura-exchange-rate';
```

## 📦 CommonJS

```javascript
const { getRate } = require('ura-exchange-rate');

getRate('USD', 'UGX', { apiKey: 'art_live_...' }).then((pair) => console.log(pair.rate));
```

## 💡 Quota tips

- Rates change once per business day — cache the official table locally and a small monthly quota goes a long way.
- Every request counts toward your AllRatesToday quota, shared across all AllRatesToday endpoints on your key.

## 📖 Methods reference

| Method | Plan | Description |
| ------ | ---- | ----------- |
| `getRate(source, target, { apiKey })` | Free | Latest rate for one pair, resolved from the official table |
| `getLatestRates({ apiKey })` | Free | The tax authority's full latest official table |
| `getRatesForDate(date, { apiKey, source?, target? })` | Paid | The official table (or one pair) for a YYYY-MM-DD date |
| `getHistory({ symbol \| source+target, from?, to? }, { apiKey })` | Paid | Daily series since 2005 |

## 📥 Bulk data (no key)

Need the whole archive rather than an API call? The same official tables are mirrored daily as open data:

- Hugging Face: [AllRatesToday/central-bank-exchange-rates](https://huggingface.co/datasets/AllRatesToday/central-bank-exchange-rates) — one CSV per institution (`rates/ura.csv`)
- Kaggle: [allratestoday/central-bank-exchange-rates](https://www.kaggle.com/datasets/allratestoday/central-bank-exchange-rates)
- Raw JSON on GitHub: `https://raw.githubusercontent.com/AllRates-Today/central-bank-exchange-rates/main/data/ura/latest.json`

## 🔗 Links

- **Website:** [allratestoday.com](https://allratestoday.com)
- [Uganda Revenue Authority rates page](https://allratestoday.com/tax-authority-rates-api/ura/) — live table, publication cadence, FAQ
- [All tax authority sources](https://allratestoday.com/tax-authority-rates-api/) · [Full list of 120+ central banks and 50+ tax authorities](https://allratestoday.com/central-bank-rates-api/institutions/) — one API, the same response shape for every source
- [Download central bank rates](https://allratestoday.com/download-central-bank-rates/) — every bank's latest table and history as Excel, CSV or JSON
- [Bank Exchange Rate API](https://allratestoday.com/bank-exchange-rate-api/) — live buy and sell rates from 1,200+ commercial banks in 120+ countries · [npm](https://www.npmjs.com/package/bank-exchange-rates) · [GitHub](https://github.com/AllRates-Today/bank-exchange-rates)
- [Package docs on the site](https://allratestoday.com/docs/sdk/ura-exchange-rate/) · [ERP integration guides](https://allratestoday.com/docs/integrations/)
- [API documentation](https://allratestoday.com/docs/#central-bank) · [Interactive reference](https://allratestoday.com/api-reference/) · [Methodology](https://allratestoday.com/official-rates-methodology/)
- [Register (Free)](https://allratestoday.com/register) · [Dashboard](https://allratestoday.com/profile) · [Pricing](https://allratestoday.com/pricing/)
- [Status](https://allratestoday.com/status)
- [Postman collection](https://allratestoday.com/postman/)
- [ChatGPT app](https://chatgpt.com/plugins/plugin_asdk_app_6ae1e76098f48191a285ac3f5ab7a83b) — ask ChatGPT for live and official central bank rates
- [OpenAPI reference on Bump.sh](https://bump.sh/allratestoday/doc/allratestoday-api) — also on [SwaggerHub](https://app.swaggerhub.com/apis-docs/allratestoday/allratestoday-exchange-rate-central-bank-rates-api/2.2.0)
- [GitHub](https://github.com/AllRates-Today/ura-exchange-rate)

## 📜 License

MIT
