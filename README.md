# Opyn (opyn)

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
