# Opyn GraphQL API

The Opyn Gamma Protocol GraphQL API is powered by The Graph and indexes all on-chain activity for the Opyn v2 (Gamma Protocol) options system on Ethereum mainnet. It exposes oToken creation and lifecycle, vault collateral and debt management, option minting/burning, settlement, liquidations, and oracle expiry prices for European cash-settled options. No API key is required for the hosted service endpoint; The Graph gateway requests require an API key.

**Endpoint:** https://api.thegraph.com/subgraphs/name/opynfinance/gamma-mainnet

**Authentication:** No authentication required for the hosted service endpoint. The Graph decentralised network gateway at https://gateway.thegraph.com/api requires an API key as a path segment.

**Documentation:** https://github.com/opynfinance/Gamma-Subgraph

**References:**
- Documentation: https://github.com/opynfinance/v2-documentation
- GettingStarted: https://thegraph.com/docs/en/querying/querying-the-graph/
- Schema: https://github.com/opynfinance/Gamma-Subgraph/blob/master/schema.graphql
- Explorer: https://thegraph.com/hosted-service/subgraph/opynfinance/gamma-mainnet
