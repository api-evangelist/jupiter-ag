# Jupiter

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

**Areas:** Solana · DeFi · DEX Aggregator · Swap · Perpetuals · Limit Orders · DCA · Lending

## Jupiter on APIs.io

Everything profiled for Jupiter is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/jupiter-ag/](https://apis.io/providers/jupiter-ag/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Jupiter Swap API](https://apis.io/apis/jupiter-ag/swap-api/) — Returns the best swap route across Solana DEX liquidity and produces a versioned transaction ready to sign and send. Supports quote-then-swap,…
- [Jupiter Tokens API](https://apis.io/apis/jupiter-ag/tokens-api/) — Search Solana tokens by mint, symbol, or name; fetch metadata, verification status, tags, and trading metrics. Backs Jupiter's verified token list.
- [Jupiter Price API](https://apis.io/apis/jupiter-ag/price-api/) — USD pricing for up to 50 Solana tokens per request, sourced from on-chain aggregated liquidity. Used for portfolio valuation, charting, and quote previews.
- [Jupiter Trigger API (Limit Orders)](https://apis.io/apis/jupiter-ag/trigger-api/) — Create, query, and cancel on-chain trigger orders — single limit orders as well as one-cancels-the-other (OCO) and one-triggers-the-other (OTOCO) order…
- [Jupiter Recurring API (DCA)](https://apis.io/apis/jupiter-ag/recurring-api/) — Schedule recurring (dollar-cost-averaging) swaps that execute on a time interval. Manage active DCA positions and fetch execution history.
- [Jupiter Perps API](https://apis.io/apis/jupiter-ag/perps-api/) — REST interface to Jupiter Perpetuals — fetch markets, positions, funding, pricing, and build open / close / modify position transactions.
- [Jupiter Lend API](https://apis.io/apis/jupiter-ag/lend-api/) — Lending product API for supplying, borrowing, repaying, withdrawing, and executing flash loans against Jupiter Lend markets.
- [Jupiter Prediction API](https://apis.io/apis/jupiter-ag/prediction-api/) — Binary prediction-market API for browsing markets, fetching prices and positions, and constructing trade transactions.
- [Jupiter Lite API](https://apis.io/apis/jupiter-ag/lite-api/) — Public, no-key, rate-limited mirror of the Jupiter API surface intended for experimentation, demos, and low-volume integrations.
- [Jupiter Terminal](https://apis.io/apis/jupiter-ag/terminal/) — Open-source embeddable swap widget that drops a fully-featured Jupiter swap experience into any web app with a few lines of code.
- [Jupiter Swap API](https://apis.io/apis/jupiter-ag/jupiter-ag-swap-api/) — Quote and build Solana DEX-aggregator swap transactions.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Jupiter Ag Agentic Access](https://apis.io/agentic-access/jupiter-ag/jupiter-ag-agentic-access/)

#### Collections (2)

Postman and Open Collection request collections.

- [Jupiter Swap API](https://apis.io/collections/jupiter-ag/open-jupiter-ag/)
- [Jupiter Swap API](https://apis.io/collections/jupiter-ag/open-jupiter-ag-swap-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Jupiter Ag Authentication](https://apis.io/security/jupiter-ag/jupiter-ag-authentication/)
- [Jupiter Ag Domain Security](https://apis.io/security/jupiter-ag/jupiter-ag-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Jupiter Ag Plans Pricing](https://apis.io/plans/jupiter-ag/jupiter-ag-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Jupiter Ag Rate Limits](https://apis.io/rate-limits/jupiter-ag/jupiter-ag-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Jupiter Ag Finops](https://apis.io/finops/jupiter-ag/jupiter-ag-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://jup.ag)
- [Documentation](https://dev.jup.ag/docs)
- [Blog](https://www.jup.ag/blog)

## API Evangelist rating

**Kin Score 25.3** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 49.0 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 26.2 |
| Access clarity | 5.3 |

**Agent readiness 17.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 11.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/jupiter-ag/](https://apis.io/providers/jupiter-ag/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Jupiter: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/jupiter-ag/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
