<div align="center">

<a href="https://lumenwipe.com">
  <img src="https://raw.githubusercontent.com/LumenWipe/.github/main/profile/assets/hero.png" alt="LumenWipe: close any Stellar account, recover every locked XLM" width="100%" />
</a>

**LumenWipe is infrastructure for closing Stellar accounts and recovering the XLM locked in their reserves.**

It offers a web app, a REST API, and an SDK, so anyone from a single user to a whole platform can run the same non-custodial wind-down. Every transaction is signed in your browser, and no server ever holds your keys or funds.

<br />

[![Live app](https://img.shields.io/badge/Live_app-lumenwipe.com-0BBBEF?style=for-the-badge&labelColor=0B1220)](https://lumenwipe.com)
[![Docs](https://img.shields.io/badge/Docs-docs.lumenwipe.com-0B1220?style=for-the-badge)](https://docs.lumenwipe.com)
[![Built on Stellar](https://img.shields.io/badge/Built_on-Stellar-F5A623?style=for-the-badge&labelColor=0B1220)](https://stellar.org)
[![License](https://img.shields.io/badge/License-Apache_2.0-0B1220?style=for-the-badge)](https://github.com/LumenWipe/lumenwipe/blob/main/LICENSE)

</div>

<br />

## What it does

A clean close is several transactions in a strict order. LumenWipe runs the whole sequence in one guided flow.

<div align="center">
  <img src="https://raw.githubusercontent.com/LumenWipe/.github/main/profile/assets/sequence.png" alt="The close, in order: signers, data, offers, positions, convert, trustlines, then merge out as recovered XLM." width="94%" />
</div>

<br />

| Capability | Status | Detail |
|---|---|---|
| Full account wind-down | Live | Clears every subentry in order, then merges. Most accounts close in a single signature. |
| Soroban and DeFi exits | Building | Exit positions on Blend, Aquarius, Soroswap, Phoenix, and FxDAO so the account can close. |
| Exchange-compatible merge | Live | Bridges the close to a CEX deposit address with the correct memo. |
| Sponsored fees | Planned | Frees accounts too locked to pay their own transaction fee. |
| Allowance inspector | Planned | Revoke risky token approvals, even without closing. |

You decide what happens to each balance: swap it to XLM or return it to its issuer. Nothing converts on autopilot.

## Non-custodial by design

- Keys stay in your browser. The backend is read-only and cannot move funds.
- Live on-chain state is re-read before anything is built or signed.
- The transaction builder is open source and auditable, with no network side effects.

## For builders

A REST API and TypeScript SDK (planned) let wallets, exchanges, and platforms run the same wind-down with their own keys. [Pollar](https://pollar.xyz/), our first integration partner, is building it into its account-closure path.

## Explore

Try it on [lumenwipe.com](https://lumenwipe.com), read the [docs and architecture](https://docs.lumenwipe.com), or dig into the [source](https://github.com/LumenWipe/lumenwipe).

<div align="center">

Open source and non-custodial, built for the Stellar ecosystem.

</div>
