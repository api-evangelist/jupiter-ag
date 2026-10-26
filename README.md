# Jupiter (jupiter-ag)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
