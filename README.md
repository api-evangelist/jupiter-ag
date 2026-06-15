# Jupiter (jupiter-ag)

Jupiter is the liquidity infrastructure powering the majority of DeFi on Solana. It aggregates spot DEXes, runs leveraged perpetuals, supports limit orders, dollar cost averaging, lending and flash loans, prediction markets, and a token launchpad. Developers integrate via production-grade REST APIs at api.jup.ag (and the rate- limited lite-api.jup.ag) covering Swap, Tokens, Price, Lend, Trigger (limit orders), Recurring (DCA), Perps, and Prediction, all behind a single API key. Open-source SDKs and the Jupiter Terminal embed widget extend the platform to wallets, exchanges, and apps.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/jupiter-ag/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/jupiter-ag/refs/heads/main/apis.yml)

## Tags

- Solana
- DeFi
- DEX Aggregator
- Swap
- Perpetuals
- Limit Orders
- DCA
- Lending

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

### Jupiter Swap API

Returns the best swap route across Solana DEX liquidity and produces a versioned transaction ready to sign and send. Supports quote-then-swap, swap-instructions for custom transaction building, slippage models, dynamic compute units, and priority fee guidance.

- **Human URL:** [https://dev.jup.ag/docs/swap-api](https://dev.jup.ag/docs/swap-api)
- **Base URL:** `https://api.jup.ag/swap`

#### Tags

- Swap
- Aggregation
- Quote
- Solana

#### Properties

- [Documentation](https://dev.jup.ag/docs/swap-api)
- [Repository](https://github.com/jup-ag/jupiter-quote-api-node)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Tokens API

Search Solana tokens by mint, symbol, or name; fetch metadata, verification status, tags, and trading metrics. Backs Jupiter's verified token list.

- **Human URL:** [https://dev.jup.ag/docs/tokens-api](https://dev.jup.ag/docs/tokens-api)
- **Base URL:** `https://api.jup.ag/tokens`

#### Tags

- Tokens
- Metadata
- Search
- Solana

#### Properties

- [Documentation](https://dev.jup.ag/docs/tokens-api)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Price API

USD pricing for up to 50 Solana tokens per request, sourced from on-chain aggregated liquidity. Used for portfolio valuation, charting, and quote previews.

- **Human URL:** [https://dev.jup.ag/docs/price-api](https://dev.jup.ag/docs/price-api)
- **Base URL:** `https://api.jup.ag/price`

#### Tags

- Price
- Market Data
- Solana

#### Properties

- [Documentation](https://dev.jup.ag/docs/price-api)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Trigger API (Limit Orders)

Create, query, and cancel on-chain trigger orders — single limit orders as well as one-cancels-the-other (OCO) and one-triggers-the-other (OTOCO) order structures.

- **Human URL:** [https://dev.jup.ag/docs/trigger-api](https://dev.jup.ag/docs/trigger-api)
- **Base URL:** `https://api.jup.ag/trigger`

#### Tags

- Limit Orders
- Trigger
- Trading

#### Properties

- [Documentation](https://dev.jup.ag/docs/trigger-api)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Recurring API (DCA)

Schedule recurring (dollar-cost-averaging) swaps that execute on a time interval. Manage active DCA positions and fetch execution history.

- **Human URL:** [https://dev.jup.ag/docs/recurring-api](https://dev.jup.ag/docs/recurring-api)
- **Base URL:** `https://api.jup.ag/recurring`

#### Tags

- DCA
- Recurring
- Automation

#### Properties

- [Documentation](https://dev.jup.ag/docs/recurring-api)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Perps API

REST interface to Jupiter Perpetuals — fetch markets, positions, funding, pricing, and build open / close / modify position transactions.

- **Human URL:** [https://dev.jup.ag/docs/perp-api](https://dev.jup.ag/docs/perp-api)
- **Base URL:** `https://perps-api.jup.ag`

#### Tags

- Perpetuals
- Leverage
- Trading

#### Properties

- [Documentation](https://dev.jup.ag/docs/perp-api)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Lend API

Lending product API for supplying, borrowing, repaying, withdrawing, and executing flash loans against Jupiter Lend markets.

- **Human URL:** [https://dev.jup.ag/docs/lend-api](https://dev.jup.ag/docs/lend-api)
- **Base URL:** `https://api.jup.ag/lend`

#### Tags

- Lending
- Borrowing
- Flash Loans

#### Properties

- [Documentation](https://dev.jup.ag/docs/lend-api)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Prediction API

Binary prediction-market API for browsing markets, fetching prices and positions, and constructing trade transactions.

- **Human URL:** [https://dev.jup.ag/docs/prediction-api](https://dev.jup.ag/docs/prediction-api)
- **Base URL:** `https://api.jup.ag/prediction`

#### Tags

- Prediction Markets
- Trading

#### Properties

- [Documentation](https://dev.jup.ag/docs/prediction-api)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Lite API

Public, no-key, rate-limited mirror of the Jupiter API surface intended for experimentation, demos, and low-volume integrations.

- **Human URL:** [https://dev.jup.ag](https://dev.jup.ag)
- **Base URL:** `https://lite-api.jup.ag`

#### Tags

- Public
- Rate Limited
- Lite

#### Properties

- [Documentation](https://dev.jup.ag)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jupiter Terminal

Open-source embeddable swap widget that drops a fully-featured Jupiter swap experience into any web app with a few lines of code.

- **Human URL:** [https://terminal.jup.ag](https://terminal.jup.ag)
- **Base URL:** `https://github.com/jup-ag/plugin`

#### Tags

- Widget
- Embed
- Swap

#### Properties

- [Documentation](https://terminal.jup.ag)
- [Repository](https://github.com/jup-ag/plugin)
- [Postman Collection](collections/jupiter-ag.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jupiter-ag.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://jup.ag)
- [Developers](https://dev.jup.ag)
- [Documentation](https://dev.jup.ag/docs)
- [Git Hub](https://github.com/jup-ag)
- [Twitter](https://x.com/JupiterExchange)
- [Discord](https://discord.gg/jup)
- [Blog](https://www.jup.ag/blog)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
