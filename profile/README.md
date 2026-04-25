# Prova

Verifiable storage anchored to Ethereum.

[prova.network](https://prova.network) — [docs](https://docs.prova.network)

You give Prova a file. Prova chunks it, replicates it across independent
provers, and pins it down with an on-chain deal. Every day, every prover
proves the file is still there with a cryptographic proof of data possession.
You retrieve over HTTPS, IPFS, or libp2p. You pay in USDC on Base.

Three things people store on Prova today:
- Static websites, anchored to ENS contenthash
- Datasets and research archives
- AI corpora and model weights

## What's here

- **[prova](./prova)** — main repository (CLI, SDK, prover, contracts, website)
- **[docs](./docs)** — public documentation source

## License

Apache-2.0 OR MIT.
