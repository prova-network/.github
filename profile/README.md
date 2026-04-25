# Prova

**Verifiable storage anchored to Ethereum.**

[prova.network](https://prova.network) — docs (coming) — twitter (coming)

You give Prova a file. Prova chunks it, replicates it across independent
provers, and pins it down with an on-chain deal. Every day, every prover
proves the file is still there with a cryptographic proof of data possession.
You retrieve over HTTPS, IPFS, or libp2p. You pay in USDC on Base.

## What people store on Prova

- **Static websites**, anchored to ENS contenthash
- **Datasets and research archives**
- **AI corpora and model weights**, with auditable provenance

## Source

This org is split into focused repos:

| Repo | What |
|------|------|
| **prova** | Umbrella + cross-cutting docs |
| **cli** | `@prova-network/cli` — the `prova` command |
| **sdk** | `@prova-network/sdk` + `core` — TypeScript SDK |
| **contracts** | Solidity contracts (Base) |
| **prover** | `provad` — the Go prover daemon |
| **website** | prova.network site |
| **desktop** | Electron prover wrapper |
| **brand** | Logos, diagrams |
| **docs** | docs.prova.network |

## License

Apache-2.0 OR MIT.
