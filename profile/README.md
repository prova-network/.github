<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://prova.network/brand/prova-mark-dark.svg">
    <img src="https://prova.network/brand/prova-mark-light.svg" alt="Prova" width="120" height="120">
  </picture>

  <h1>Prova</h1>

  <p><strong>Verifiable storage anchored to Ethereum.</strong></p>

  <p>
    <a href="https://prova.network">prova.network</a> ·
    <a href="https://docs.prova.network">docs</a> ·
    <a href="https://spec.prova.network">spec</a> ·
    <a href="mailto:hello@prova.network">hello@prova.network</a>
  </p>
</div>

---

You give Prova a file. We chunk it, replicate it across independent provers, and pin it down with an on-chain deal on Base. Every challenge interval the prover proves the file is still there with a Merkle inclusion proof against the committed piece-CID. You retrieve over HTTPS or via ENS contenthash. You pay in **USDC**. The provers stake **PROVA**, and slashing burns the stake.

No new chain. No bridges. No custody. Boring stablecoin payments for clients, supply-side incentives for provers.

## What people store on Prova

- **Static websites**, anchored to ENS contenthash
- **Datasets and research archives**
- **AI corpora and model weights**, with auditable provenance

## How the economics work

```
Client uploads → 99% USDC streams to prover (per epoch, per proof)
                 1% USDC routes to FeeRouter → swaps to PROVA → burns

Prover earns:    USDC (real revenue)
                 + PROVA emission (50M total over 8 years, on-chain)
Prover stakes:   PROVA (slashable bond)
Prover risks:    PROVA slashing (loss of bond on misbehavior)
```

50% of all PROVA supply (50M of 100M) flows to provers as on-chain emission, paid weekly per byte proven, gated by anti-gaming protections (no self-dealing, redundancy cap, quality multiplier, 30-day vesting).

Full whitepaper at [prova.network/whitepaper](https://prova.network/whitepaper).
Token economics at [TOKENOMICS-2026.md](https://github.com/prova-network/prova/blob/main/TOKENOMICS-2026.md).
Protocol spec at [spec.prova.network](https://spec.prova.network).

## Repos

| Repo | What |
| --- | --- |
| [**prova**](https://github.com/prova-network/prova) | Umbrella + cross-cutting docs |
| [**contracts**](https://github.com/prova-network/contracts) | Solidity contracts (ProvaToken, ProvaVesting, ProverRewards, FeeRouter, StorageMarketplace, ProverStaking, …) |
| [**cli**](https://github.com/prova-network/cli) | `@prova-network/cli` — the `prova` command |
| [**sdk**](https://github.com/prova-network/sdk) | `@prova-network/sdk` + `core` — TypeScript SDK |
| [**prover**](https://github.com/prova-network/prover) | `provad` — the Go prover daemon |
| [**website**](https://github.com/prova-network/website) | The [prova.network](https://prova.network) site |
| [**docs**](https://github.com/prova-network/docs) | [docs.prova.network](https://docs.prova.network) source |
| [**desktop**](https://github.com/prova-network/desktop) | Electron prover wrapper |
| [**brand**](https://github.com/prova-network/brand) | Logos, diagrams, brand kit |

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

## Status

| | |
| --- | --- |
| Whitepaper | [v1.0 specification](https://prova.network/whitepaper) |
| Spec | [spec.prova.network](https://spec.prova.network) (per-section state + audit) |
| Contracts | 8 contracts, **81 unit tests passing**, full lifecycle smoke-tested on local anvil |
| Network | Base Sepolia testnet deploy in progress; mainnet H2 2026 |

## License

All code: Apache-2.0 OR MIT.
Brand assets: CC-BY-4.0.
