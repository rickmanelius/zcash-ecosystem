# Zcash Ecosystem Reference

A map of the active Zcash ecosystem: the orgs, protocol layers, wallets, payment rails, tooling, exchanges, mining, and treasury players, with a one-line description of what each does.

**Use this file as context** when doing any Zcash research, evaluating a project or partnership in the space, writing about ZEC, or onboarding someone to how the ecosystem fits together. It is a structured directory, not analysis. Verify anything time-sensitive (scope, leverage limits, listing status) against the live source before relying on it.

**Source:** "Zcash Ecosystem May 2026," a running list maintained by Josh Swihart (@jswihart). Original X article: https://x.com/i/article/2060479023185334272 (linked from https://x.com/jswihart/status/2060482005713015277). The original lists hyperlinks per entry; those URLs are not reproduced here.

**Captured:** 2026-06-07. Snapshot of a fast-moving space. Treat dates, scopes, and "under development" notes as accurate to May 2026.

---

## At a glance

- **Who builds the core:** ZODL (full-stack company, Zashi/ZODL wallet, Zallet), Zcash Foundation (zebrad, FROST, governance), Shielded Labs (Crosslink, NSM), with research from Valar Group and QEDIT.
- **Where the protocol is headed:** NU7 is the next network upgrade; final scope settled by a June 2026 coinholder vote. The node stack is consolidating into the **Z3 Stack** (zebrad + Zaino + Zallet); zcashd is being deprecated.
- **Flagship wallet:** ZODL (formerly Zashi), shielded-by-default.
- **Big institutional backers:** Cypherpunk Technologies (CYPH, Winklevoss-backed, 290k+ ZEC) and DCG (owns Grayscale, Foundry, Fortitude).
- **Key distinction to keep straight:** "Shielded" ZEC carries Zcash's native privacy; "transparent" ZEC does not. Most exchanges and all wrapped-ZEC tokens on other chains are transparent only.

---

## Orgs

- **ZODL:** Independent full-stack Zcash company doing core protocol research and development, managing zcashd, and building the Zashi/ZODL wallet and Zallet.
- **Zcash Foundation (ZF):** 501(c)(3) stewarding protocol infrastructure (zebrad, FROST), governance, and the Shielded Aid Initiative. Runs the Zcon conference and manages the z.cash website and the Zcash X account.
- **Shielded Labs:** Swiss, donation-funded org working on Crosslink, dynamic fees, and the Network Sustainability Mechanism (NSM).
- **Valar Group:** Dev/research team that built ZODL's shielded coinholder-polling protocol and authored the NU7 block-time-reduction research.
- **Zcash Community Grants (ZCG):** Community-elected committee funding ecosystem work. Recently approved BTCPayServer improvements, Hito hardware wallet support, Tor's internet-freedom crowdfunding campaign, and DWeb Camp outreach.
- **Financial Privacy Foundation (FPF):** Cayman foundation providing back-office support for decentralized teams.
- **ZecHub:** Volunteer-driven education hub and community wiki.
- **Zk Av Club:** Community audiovisual collective doing privacy-first AV training, event recording stations, and archiving. ZCG-funded.
- **Regional communities:** Brazil, Nigeria, India, Ghana, Türkiye, and Arabia: independently grant-funded local chapters. Others form and sunset with grant cycles.
- **QEDIT:** Privacy-preserving asset-transfer systems. Lead implementer of Zcash Shielded Assets.

## Core Protocol & Infrastructure

- **zebrad:** Rust full node by the Zcash Foundation, becoming the sole consensus node after NU7.
- **zcashd:** The original C++ node, managed by ZODL and now being deprecated (still receiving security patches).
- **Zaino:** Rust indexer by the Zingo team that replaces lightwalletd.
- **lightwalletd:** Legacy light-client backend server that mobile and light wallets query. Being superseded by Zaino.
- **Zallet:** New wallet/RPC daemon developed by the ZODL team, succeeding the zcashd wallet.
- **Z3 Stack:** The unification of zebrad, Zaino, and Zallet.

## Protocol Upgrades & Cryptographic Research

> NU7 scope is still TBD and will be settled by polling in June 2026.

- **NU7:** The ninth network upgrade. Final scope to be resolved by the June 2026 coinholder vote.
- **Orchard Quantum Recoverability (QR):** Wallet-level recovery solution for Orchard shielded funds against future quantum threats. Rollout targeted for mid-2026. Strong community support.
- **FROST:** Threshold/multisig signatures for shielded transactions (v3.0.0 released April 2026).
- **25-Second Block Time:** Active proposal to cut target block time from 75s to 25s for faster confirmations.
- **Network Sustainability Mechanism (NSM):** Proposed fee-burning and issuance-smoothing mechanism from Shielded Labs. Components polled differently and remain under deliberation.
- **Project Tachyon:** Longer-horizon scaling research (proof-carrying wallets, oblivious sync). Not slated for NU7.
- **Crosslink:** Proposed hybrid PoW/PoS finality layer developed by Shielded Labs.
- **Zcash Shielded Assets (ZSA):** User-issued private tokens, led by QEDIT. Coinholders voted heavily against inclusion; there is not yet clear consensus on whether ZSAs should be activated, and they are not slated for NU7.

## Wallets

- **ZODL (formerly Zashi):** The flagship self-custody, shielded-by-default wallet, built by the ZODL team. Supports Arti (Tor) and the CrossPay in-wallet cross-chain swap feature.
- **Zingo!:** Shielded-first mobile wallet with Orchard and Unified Address support.
- **Unstoppable:** Multi-currency self-custody wallet with shielded ZEC.
- **Edge:** Multi-asset mobile wallet with shielded ZEC support.
- **Brave Wallet:** Shielded Zcash built into the Brave browser.
- **Keystone:** Air-gapped open-source hardware wallet with shielded support.
- **Trezor:** Hardware wallet supporting transparent ZEC only.
- **Ledger:** Hardware wallet supporting transparent ZEC only.
- **Vultisig:** Seedless, multi-factor, multi-chain vault app.
- **Vizor:** macOS desktop wallet by the Keplr team. Shielded-by-default, multi-account, Keystone support, open source.
- **Zkool:** Multi-account Zcash wallet (successor to Ywallet, same developer). Supports nearly every account type and Unified Addresses.
- **Cake:** Multi-coin privacy wallet.

## Payments & Apps

- **CipherPay:** Non-custodial Zcash payment processor. Merchants detect payments via viewing keys and receive ZEC directly to a shielded wallet.
- **Free2z:** Peer-to-peer creator donations using Zcash.
- **ZGo:** Browser-based ZEC point-of-sale software for merchants (rebuilt on Zebra 4.0.0 for shielded payments).
- **Flexa:** Payments network enabling ZEC spending at retail. Integrated into ZODL.

## Network, Browser & Messaging Privacy

- **Nym Mixnet:** Protects transactions in transit by obscuring metadata.
- **WebZJS / MetaMask Zcash Snap:** ChainSafe's JavaScript SDK and MetaMask Snap bringing shielded Zcash (PCZT) to the browser.

## Tools, Data & Explorers

- **ZeWIF:** Wallet interchange format by Zingo Labs and Blockchain Commons for cross-wallet compatibility.
- **Zcashinfo.com:** Block explorer with real-time network and mining data, built by Foundry (launched April 2026).
- **Zcash Explorer:** Community block explorer by Nighthawk Apps (no trackers).
- **Blockchair:** Third-party Zcash explorer and blockchain data.
- **Bitquery:** Third-party Zcash explorer and blockchain data.
- **CipherScan:** Privacy-first, open-source Zcash block explorer with shielded pool stats and a free public API.

## Bridges, Swaps & Cross-Chain

- **NEAR Intents:** Powers private cross-chain swaps (e.g., ZEC to BTC/ETH) without a centralized exchange.
- **Maya Protocol:** Decentralized cross-chain exchange for trading across blockchains.
- **THORChain:** Cross-chain DEX with native ZEC swaps now live.
- **Zcash-Avalanche RedBridge:** Bridge between Zcash and Avalanche. Still under development.
- **THORSwap:** Multi-chain DEX aggregator listing ZEC.
- **SwapKit:** Developer toolkit with ZEC as a source/destination chain.
- **Houdini Swap:** Private cross-chain swapping service.
- **LeoDex:** Non-custodial cross-chain DEX interface for native L1 swaps.

## DeFi, Wrapped ZEC & Derivatives

> Note: wrapped ZEC on other chains are transparent tokens and do not support Zcash's native privacy.

- **Rhea Finance:** NEAR-based DeFi protocol (Ref + Burrow merger) building the Noir wallet and a Zcash DeFi gateway.
- **zenZEC:** Zenrock's 1:1 wrapped ZEC on Solana, secured by decentralized MPC custody and built for DeFi yield (transparent SPL token).
- **wZEC (Zolana):** Wrapped ZEC bridged onto Solana. Standard SPL token with no native privacy.
- **OKX:** Major exchange offering ZEC perpetual swaps (USDT and coin-margined). ZEC X-Perps added for EEA users at up to 10x leverage.
- **Hyperliquid:** On-chain DEX offering ZEC perpetual futures.
- **Backpack:** Exchange with a live ZEC-PERP market and zero-gas execution.

## Exchanges Supporting ZEC

> Most centralized exchanges support transparent ZEC only. Gemini supports shielded withdrawals.

- **Listing ZEC:** Robinhood (nationwide U.S., April 2026, transparent withdrawals only), Coinbase, Kraken, Binance, Gemini, Bitstamp, Bitfinex, KuCoin, Poloniex, CoinDCX, Luno.
- **Non-custodial / instant-swap:** ChangeNOW, Changelly, Flyp.me.
- **Institutional custodians:** Fireblocks, BitGo, Gemini.

## Mining

- **Foundry:** Launched a U.S. institutional-grade Zcash mining pool in April 2026.
- **Fortitude Mining:** Proprietary mining arm positioning as a "Zcash ecosystem leader."
- **ViaBTC:** Long-established multi-coin pool supporting ZEC.
- **F2Pool:** Major multi-coin pool supporting ZEC.
- **2Miners:** Popular pool favored by smaller/home miners.

## Institutional & Treasury

- **Cypherpunk Technologies (CYPH):** Winklevoss-backed Nasdaq-listed privacy-tech firm. Holds 290,000+ ZEC and actively backs the ecosystem, including a $5M investment into ZODL.
- **Digital Currency Group (DCG):** Conglomerate that owns Grayscale, Foundry, and Fortitude.
- **Grayscale Zcash Trust (ZCSH):** DCG's regulated ZEC investment vehicle (launched 2017), which Grayscale is seeking to convert into an ETF.

---

## Glossary of recurring terms

- **Shielded vs. transparent:** Shielded ZEC uses Zcash's zero-knowledge privacy (amounts and parties hidden); transparent ZEC behaves like a normal public-ledger coin. Wrapped ZEC on other chains is always transparent.
- **Orchard:** The current shielded pool / payment protocol (the target of the Quantum Recoverability work).
- **Unified Addresses:** A single address format that can receive across Zcash's pool types.
- **PCZT:** Partially Created Zcash Transaction; the format that lets browser/external signers build shielded transactions (used by WebZJS / the MetaMask Snap).
- **Coinholder vote / polling:** Zcash's governance signal where ZEC holders express preference (e.g., to settle NU7 scope in June 2026).
- **NU7:** The ninth network upgrade, the near-term protocol milestone.
- **Z3 Stack:** The post-NU7 node architecture: zebrad (node) + Zaino (indexer) + Zallet (wallet/RPC).
