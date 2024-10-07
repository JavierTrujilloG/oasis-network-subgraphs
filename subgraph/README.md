# Subgraph 101

## Deploying ERC-20 subgraph to Goldsky

We'll be indexing [Rosy token contract](https://explorer.oasis.io/mainnet/sapphire/token/0x6665a6Cae3F52959f0f653E3D04270D54e6f13d8) on Oasis Sapphire.

The subgraph is already build, all you need to do is to deploy it onto Goldsky with the following command:
`goldsky subgraph deploy rosy-sapphire-balances/1.0.0`

Alternatively, you can easily use this subgraph code to index any other ERC-20 contract by changing in the `subgraph.yaml`:
- Contract Address
- Start Block

Run `graph codegen` and `graph build` before deploying the subgraph.

All of the code for this example was borrowed from [Chainstack](https://docs.chainstack.com/docs/subgraphs-tutorial-indexing-erc-20-token-balance).

## Other fun subgraph resources

- [The Graph's](https://thegraph.com/docs/en/quick-start/) documentation for subgraphs.
  - [Creating a Subgraph](https://thegraph.com/docs/en/developing/creating-a-subgraph/).
  - [AssemblyScript API](https://thegraph.com/docs/en/developing/graph-ts/README/).
- [Messari subgraphs](https://github.com/messari/subgraphs): A collection of hand crafted subgraphs that cover a lot of different protocols. Lots of tooling is involved to build these, ping me if you need help.
- [Nouns](https://github.com/nounsDAO/nouns-monorepo/tree/master/packages/nouns-subgraph): A solid example of a DAO subgraph.
