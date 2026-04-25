<div align="center">
  <img src="https://prova.network/brand/prova-mark.svg" alt="Prova" width="120" height="120" />

  <h1>Prova</h1>

  <p><strong>Verifiable storage anchored to Ethereum.</strong></p>

  <p>
    <a href="https://prova.network">prova.network</a> ·
    <a href="https://docs.prova.network">docs</a> ·
    <a href="mailto:hello@prova.network">hello@prova.network</a>
  </p>
</div>

---

You give Prova a file. We chunk it, replicate it across independent provers, and
pin it down with an on-chain deal. Every 30 seconds, every prover proves the
file is still there with a cryptographic proof of data possession. You retrieve
over HTTPS, IPFS, or libp2p. You pay in USDC on Base.

No new chain. No bridges. No token launch. No custody. Just verifiable,
retrievable storage.

## What people store on Prova

- **Static websites**, anchored to ENS contenthash
- **Datasets and research archives**
- **AI corpora and model weights**, with auditable provenance

## Repos

| Repo | What |
| --- | --- |
| [**prova**](https://github.com/prova-network/prova) | Umbrella + cross-cutting docs |
| [**cli**](https://github.com/prova-network/cli) | `@prova-network/cli` — the `prova` command |
| [**sdk**](https://github.com/prova-network/sdk) | `@prova-network/sdk` + `core` — TypeScript SDK |
| [**contracts**](https://github.com/prova-network/contracts) | Solidity contracts (Base) |
| [**prover**](https://github.com/prova-network/prover) | `provad` — the Go prover daemon |
| [**website**](https://github.com/prova-network/website) | The [prova.network](https://prova.network) site |
| [**desktop**](https://github.com/prova-network/desktop) | Electron prover wrapper |
| [**brand**](https://github.com/prova-network/brand) | Logos, diagrams, brand kit |
| [**docs**](https://github.com/prova-network/docs) | [docs.prova.network](https://docs.prova.network) source |

## Try it

```bash
# Browser, no install
open https://prova.network/upload/

# CLI
curl -fsSL https://get.prova.network | sh
prova auth
prova put ./file.bin

# SDK
npm i @prova-network/sdk viem
```

## License

All code: Apache-2.0 OR MIT.
Brand assets: CC-BY-4.0.
