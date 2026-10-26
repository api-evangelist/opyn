# Opyn (opyn)

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

Opyn is a DeFi options protocol on Ethereum mainnet best known for Squeeth (squared ETH), a Power Perpetual that gives traders continuous exposure to ETH² without liquidation risk on long positions. The protocol encompasses the Gamma Protocol (v2 options with cash-settled European options), the Crab Strategy (automated ETH²/ETH delta-neutral vault), Bull Strategy, and Opyn Markets (concentrated-liquidity perps). Developers integrate via The Graph GraphQL subgraph for querying squeeth positions, vault data, funding rates, and on-chain event history, combined with direct Ethereum smart-contract interaction through the Controller, Oracle, WPowerPerp, and Strategy contracts. No centralised REST API key is required; data access is permissionless through the subgraph and blockchain.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/opyn/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/opyn/refs/heads/main/apis.yml)

## Tags

- DeFi
- Options
- Ethereum
- Squeeth
- Power Perpetual
- Derivatives
- Cryptocurrency
- Web3
- Smart Contracts
- Subgraph
- Crab Strategy
- Vault

## Timestamps

- **Created:** 2026-06-14
- **Modified:** 2026-06-14

## APIs

### Opyn Squeeth Subgraph API

GraphQL API powered by The Graph that indexes all on-chain Squeeth events on Ethereum mainnet. Enables developers to query oSQTH positions, short vaults, vault collateral and debt, funding (mark/index) history, Crab strategy deposits and withdrawals, and liquidation events without running an archive node. The subgraph ID on The Graph network is Ao1QSKEQzsnNyyGKR1Faurjmkr6oNVTbgdxy6diAw9r.

- **Human URL:** [https://thegraph.com/explorer/subgraphs/Ao1QSKEQzsnNyyGKR1Faurjmkr6oNVTbgdxy6diAw9r?view=Overview&chain=mainnet](https://thegraph.com/explorer/subgraphs/Ao1QSKEQzsnNyyGKR1Faurjmkr6oNVTbgdxy6diAw9r?view=Overview&chain=mainnet)
- **Base URL:** `https://gateway.thegraph.com/api`

#### Tags

- Squeeth
- Subgraph
- GraphQL
- Positions
- Vaults
- Funding Rate
- Crab Strategy
- Liquidations

#### Properties

- [Documentation](https://opyn.gitbook.io/squeeth)
- [Graph Q L](https://thegraph.com/explorer/subgraphs/Ao1QSKEQzsnNyyGKR1Faurjmkr6oNVTbgdxy6diAw9r?view=Playground&chain=mainnet)
- [GitHub Repository](https://github.com/opynfinance/squeeth-monorepo)
- [Code Examples](https://github.com/opynfinance/squeeth-monorepo)

### Opyn Gamma Subgraph API

GraphQL API via The Graph that indexes the Gamma Protocol (Opyn v2) on Ethereum mainnet. Covers oToken creation, option series, vault collateral, minting and burning events, settlement, and operator authorisations for European cash-settled options. Useful for querying options series data, vault collateral ratios, and historical settlement prices.

- **Human URL:** [https://github.com/opynfinance/Gamma-Subgraph](https://github.com/opynfinance/Gamma-Subgraph)
- **Base URL:** `https://api.thegraph.com/subgraphs/name/opynfinance/gamma-mainnet`

#### Tags

- Options
- Gamma Protocol
- Subgraph
- GraphQL
- oTokens
- Vaults
- Settlement

#### Properties

- [Documentation](https://github.com/opynfinance/v2-documentation)
- [Graph Q L](https://api.thegraph.com/subgraphs/name/opynfinance/gamma-mainnet)
- [GitHub Repository](https://github.com/opynfinance/Gamma-Subgraph)
- [GitHub Repository](https://github.com/opynfinance/v2-documentation)
- [Graph Q L Schema](graphql/opyn-schema.graphql)
- [Graph Q L](graphql/opyn-graphql.md)

### Squeeth Portal Auction API

Web interface and data feed for the Crab Strategy weekly auction mechanism. The Squeeth Portal at squeethportal.xyz provides auction status, hedging queue, and rebalancing parameters used by Crab v2 and Jumbo Crab vaults. Developers can read auction state directly from the CrabStrategyV2 contract (0x3B960E47784150F5a63777201ee2B15253D713e8) on Ethereum mainnet.

- **Human URL:** [https://www.squeethportal.xyz/auction](https://www.squeethportal.xyz/auction)
- **Base URL:** `https://www.squeethportal.xyz`

#### Tags

- Auction
- Crab Strategy
- Hedging
- Rebalancing
- Squeeth

#### Properties

- [Documentation](https://opyn.gitbook.io/squeeth/crab-strategy/introduction)
- [Interface](https://www.squeethportal.xyz/auction)
- [GitHub Repository](https://github.com/opynfinance/squeeth-monorepo)

## Common Properties

- [Website](https://www.opyn.co)
- [Website](https://squeeth.opyn.co)
- [Documentation](https://opyn.gitbook.io/squeeth)
- [GitHub Organization](https://github.com/opynfinance)
- [Twitter](https://x.com/opyn_)
- [Discord](https://discord.gg/2NFdXaE)
- [Medium](https://medium.com/opyn)
- [Bug Bounty](https://immunefi.com/bounty/opyn/)
- [Audits](https://opyn.gitbook.io/squeeth/resources/audits-and-insurance)
- [Smart Contracts](https://etherscan.io/address/0x64187ae08781B09368e6253F9E94951243A493D5)
- [Smart Contracts](https://etherscan.io/address/0xf1B99e3E573A1a9C5E6B2Ce818b617F0E664E86B)
- [Smart Contracts](https://etherscan.io/address/0x3B960E47784150F5a63777201ee2B15253D713e8)
- [Graph Explorer](https://thegraph.com/explorer/subgraphs/Ao1QSKEQzsnNyyGKR1Faurjmkr6oNVTbgdxy6diAw9r)
- [Plans](plans/opyn-plans-pricing.yml)
- [Rate Limits](rate-limits/opyn-rate-limits.yml)
- [Fin Ops](finops/opyn-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
