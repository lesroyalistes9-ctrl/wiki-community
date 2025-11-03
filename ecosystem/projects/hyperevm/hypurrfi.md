---
icon: cat
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# HypurrFi

**HypurrFi** is the debt infrastructure powering Hyperliquid's financial ecosystem, providing lending markets, synthetic dollar tooling, and cashflow-enabled credit products.

[Website](https://hypurr.fi) | [X](https://x.com/HypurrFi) | [Telegram](https://t.me/+YvsBvSxlQrVhNDkx) | [Docs](https://docs.hypurr.fi) | [Demo](https://x.com/HypurrFi/status/1960693777510637802)

### What is HypurrFi?

While traditional lending protocols like Aave or Compound focus on isolated supply/borrow mechanics, HypurrFi is designed around **capital efficiency through leverage loops and synthetic dollar minting**.

**Core mission**: Provide the debt rails that make sophisticated onchain finance possible—from leveraged trading to real-world asset financing to everyday spending.

#### What Makes HypurrFi Different

**Traditional Lending**: Deposit → Borrow → Manual strategies

**HypurrFi**: Deposit → Borrow → **Loop for leveraged spot exposure** → Mint synthetic dollars → Deploy across ecosystem

The key differentiators:

* **Intuitive UX**: Quick deposit/borrow interface with clear dashboard showing real-time position health, yields, and net performance
* **Clean leverage loops**: Amplify your HYPE/stHYPE yield while maintaining 100% spot position exposure—no complex strategies needed
* **E-Mode**: Achieve higher borrowing power by grouping assets with correlated risks (stablecoins, liquid staking tokens)
* **USDXL synthetic dollar**: Mint dollars directly from your lending position without requiring suppliers, enabling capital efficiency unavailable in traditional protocols
* **UST Reserve backing**: Protocol profits continuously acquire tokenized US Treasuries as additional security for USDXL—creating a hybrid backing model unique to HypurrFi
* **Integrated ecosystem tools**: Credit card spending, cross-chain bridging, and trade aggregation built directly into the lending experience
* **Catflow philosophy**: Capital isn't meant to sit idle—HypurrFi creates incentives for productive capital deployment across the entire Hyperliquid ecosystem, generating yield not just for users but for DeFi protocols across the chain

### USDXL: Hybrid Synthetic Dollar

**USDXL** is HypurrFi's native synthetic dollar—a scalable stablecoin designed for capital efficiency across Hyperliquid. Unlike traditional stablecoins, USDXL is **minted on-demand from your collateral** without requiring a supply side, and is backed by both user overcollateralization and a growing reserve of **tokenized US Treasury bonds**.

#### How USDXL Works

USDXL follows a **mint-and-burn mechanism** integrated into HypurrFi's core lending markets:

* **Mint**: Supply collateral (HYPE, stHYPE, stables) → Borrow USDXL at $1.00 protocol value → USDXL created on-demand
* **Burn**: Repay borrowed USDXL + accrued interest → USDXL removed from circulation → Collateral unlocked
* **No suppliers**: Unlike traditional lending assets, USDXL doesn't require lenders—it's minted directly when borrowed
* **Interest flows**: All USDXL borrow interest → DAO treasury + UST reserve (no supplier split needed)

**Critical distinction**: While USDXL always trades at $1.00 _within HypurrFi protocol_, market price may fluctuate. This creates **natural arbitrage opportunities** that maintain peg stability.

#### UST Reserve Backstop

What makes USDXL "hybrid-backed":

* **Primary layer**: Overcollateralized user deposits (standard CDP model)
* **Reserve layer**: Protocol profits continuously acquire tokenized US Treasury bonds (UST)
* **Reserve functions**: Emergency backstop, yield stabilizer, long-term revenue generator

This creates a **flywheel effect**: Protocol revenue → More UST acquired → More yield generated → Stronger peg → More user confidence → Higher usage → More revenue.

#### USDXL V2: Current Stability System

[V2](https://x.com/HypurrFi/status/1978891057468187032) introduces three mechanisms to maintain peg while enabling scale:

**1. Dynamic Rate Controller**

Automatically adjusts borrow rates based on real-time market conditions:

* Tracks **48-hour trailing average** of USDT0 borrow rates as baseline
* Monitors **real-time USDXL price** from Pyth oracles
* **Target price**: $0.998 (where USDXL rates should match USDT0)

**Rate behavior**:

* Price drops below target → Borrow rate increases exponentially (discourages minting, reduces supply)
* Price near target → Rate tracks slightly above baseline
* Price above target → Rate drops below baseline
* **At $1.00 exactly, borrowing USDXL becomes cheaper than USDT0**

Rate changes are gradual (20% of gap per adjustment) to avoid sudden shocks.

**2. Reflexive Fee Distribution**

Creates **positive incentives** for peg support instead of just punishing borrowers:

* USDXL borrow fees → Flow directly to **USDXL/hyUSDT0 Balancer LP pool** depositors
* Price drops + rates increase → **LP rewards automatically increase**
* Natural arbitrage opportunities emerge to buy USDXL and restore peg

**Result**: When USDXL needs support most (below peg), those providing that support (LPs) get rewarded most.

**3. Global Stability Module (GSM)**

Captures value during upward deviations to support downward pressure:

* **Mint**: Swap 1 USDT0 → 1 USDXL when market price trades above $1.00
* **Redeem**: Swap 1.02 USDXL → 1 USDT0 (provides natural selling pressure below peg)
* All GSM funds deployed into **USDT0 lending market** earning interest
* Creates profitable arbitrage while building treasury reserves

**Traditional arbitrage still works**: Mint USDXL from lending markets at $1.00 → sell at premium, or buy cheap USDXL → repay debt and save money.

#### USDXL Use Cases

* **Leverage loops**: Deposit HYPE → Borrow USDXL → Buy more HYPE → Repeat for amplified yield while maintaining spot exposure
* **Better than USDT0 for loops**: USDXL has **no liquidity caps** (minted on-demand vs limited by suppliers), often **cheaper rates** (no supplier split + dynamic controller), and **scales infinitely** during high-demand periods when USDT0 utilization spikes
* **Profitable arbitrage**: Earn by helping maintain peg stability

### Credit Card: Spend Without Selling

HypurrFi's **Swype Card** (via Brahma) lets you spend crypto without selling—accepted at **100M+ merchants** globally.

**Two modes**:

* **Credit Mode**: Purchases create USDT0 borrows against your HypurrFi collateral—crypto stays deposited earning yield
* **Spend Mode**: Deposit USDT0, earn lending rates, spend the balance directly

**Why it matters**: Stay long HYPE while accessing spending power for everyday purchases.

### Bridge: Cross-Chain Deposits

The HypurrFi bridge enables **instant routing from multiple EVM chains** directly into HyperEVM, powered by **Enso** and **Stargate**. No more manual bridging—deposit from your preferred chain and start using HypurrFi immediately.

### Team & Development

Led by co-founders [@andyhyfi](https://x.com/andyhyfi) and [@androolloyd](https://x.com/androolloyd), HypurrFi takes a measured, user-focused approach to growth. The protocol prioritizes **long-term stability** over rapid TVL expansion, building trust through robust systems designed for institutional scale.

### Resources

* [The HypurrFi Vision](https://hypurrfi.beehiiv.com/p/the-hypurrfi-vision)
* [HypurrFi Points S1](https://x.com/HypurrFi/status/1966186516025323942) | [HypurrFi Points S2](https://x.com/HypurrFi/status/1966550509759648135)

***

_HypurrFi provides the debt infrastructure for Hyperliquid's financial ecosystem—enabling leveraged lending, synthetic dollars, and cashflow-enabled credit for sophisticated onchain finance. Making catflow purrr._
