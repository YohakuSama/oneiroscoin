# ONEIROSCOIN
## ONRC · Project Whitepaper 1.0

**Born from a dream. Destined for nothing. Honk your dreams.**

16 November 2026  |  Solana Mainnet  |  English Edition

**Abstract**

OneirosCoin (ONRC) is a culture-led meme token on Solana, built around the ideas of dreams, nothingness, and a mythical goose. Inspired by the *Oneiroi*, the dream spirits of Greek mythology, ONRC gives a distinct visual identity to an openly traded digital token. The project combines a fixed token supply with Meteora's Dynamic Bonding Curve (DBC), a USDC-denominated market, and predetermined graduation and liquidity-allocation parameters. It is operated by a single founder. The founder's token allocation is zero, and the project's operating revenue comes from creator trading fees allocated through the protocol.

ONRC separates its cultural identity from its market infrastructure. The goose is the recognizable symbol and creative center. Solana provides token settlement. Meteora supplies early-stage price discovery and the transition to a post-graduation liquidity pool. Participants can verify the token's core properties through public mainnet accounts.

## 01 The Idea: Give a Dream a Symbol

Online communities often begin with a shared image, phrase, or story. OneirosCoin begins with an intentionally simple premise: a dream without a promise can still have a recognizable, lasting digital symbol.

The name references the *Oneiroi*, figures associated with dreams in Greek mythology. The Chinese-language community connects that idea with the goose, giving rise to the nickname “Goose Coin.” Engraved coin artwork, dream imagery, and the goose form a consistent creative identity across languages and platforms.

The token's principal role is cultural expression and open market participation. People use the shared symbol, official content, and community channels to take part in the story. Its relevance depends on creative participation, cultural reach, and actual demand. The project has a deliberately clear scope from day one.

### Three design principles

**Recognizable.** OneirosCoin, ONRC, and the goose point to one public identity. Every official channel identifies the same Solana mint address.

**Accessible.** Participants use an ordinary Solana wallet and a DBC-compatible trading interface. Entry and exit quotes come from a public on-chain curve, rather than privately negotiated allocations.

**Verifiable.** Supply, token authorities, base trading fees, graduation threshold, and liquidity-allocation settings can be checked against public accounts. The website communicates; the deployed programs execute.

## 02 The Asset: ONRC at a Glance

| Property | OneirosCoin configuration |
|---|---|
| Name / ticker | OneirosCoin / ONRC |
| Network / standard | Solana mainnet / SPL Token |
| Fixed supply | **1,000,000,000 ONRC** |
| Token decimals | 6 |
| Quote asset | Native USDC on Solana |
| Launch venue | Meteora Dynamic Bonding Curve |
| DBC base trading fee | **0.30% (30 basis points)** |
| Graduation condition | **750 USDC quote reserve** |
| Post-graduation venue | Meteora DAMM v2 |
| Creator LP allocation after graduation | **100% permanently locked** |
| Founder token allocation | **0 ONRC** |

The token is live on Solana mainnet. A recorded post-deployment inspection confirmed the one-billion-token supply, six-decimal precision, revoked mint and freeze authorities, and immutable token metadata. These are properties of the deployed asset, not settings that the project website can revise.

### Public market distribution

ONRC uses the DBC launch path. Token inventory is administered through the bonding-curve trading and migration-reserve mechanics. Participants acquire ONRC by trading on-chain. The project has no founder reserve and no separate team allocation pool. The founder operates alone, commits not to hold ONRC personally, and uses only the protocol's creator-fee allocation as the founder's project income.

This structure connects the founder's economic interest to actual trading activity rather than the disposal of a privately allocated token inventory. Market holdings change with transactions. Token accounts and balances remain visible through Solana explorers.

## 03 The Market: From Bonding Curve to Liquidity Pool

OneirosCoin began trading through a Meteora DBC virtual pool. The curve establishes an on-chain quotation rule from launch. Each trade changes the relationship between USDC quote reserves and the supply of ONRC available along the curve.

**Buying ONRC.** A buyer submits USDC. After applicable trading fees, the curve supplies an amount of ONRC based on its current state. Increased demand moves the marginal price along the configured curve.

**Selling ONRC.** A seller delivers ONRC and receives USDC according to the then-current curve. Both directions are sensitive to order size and available liquidity.

**Reading a quote.** A trader should verify the official mint, review the estimated output, choose a suitable slippage limit, and confirm the transaction in their wallet. USDC provides a familiar unit of account, while the market price of ONRC changes as trading takes place.

### The launch lifecycle

**A · Bonding-curve trading** → **B · 750 USDC quote-reserve condition** → **C · Protocol migration** → **D · DAMM v2 market**

The 750 USDC target measures the pool's quote reserve. It does not describe ONRC's market capitalization or cumulative turnover. Purchases increase quote reserve; sales can reduce it. Graduation follows net reserve conditions and protocol execution.

## 04 Liquidity Design: A Market Beyond the Launch

Once the curve completes and the relevant conditions are met, Meteora's migration process uses accumulated quote assets together with the allocated remaining ONRC to seed liquidity on DAMM v2. ONRC chose this route to give its launch phase a defined transition into an ongoing trading market.

The deployed configuration assigns **100% of the creator's migrated liquidity-provider allocation to permanent locking**. Creator-withdrawable LP allocation is **0%**. This arrangement concerns the principal represented by the migrated liquidity position. Protocol rules allow fees generated by relevant locked positions to be claimed by their beneficiaries.

The economic connection is straightforward: the founder earns the applicable fee stream while the post-graduation liquidity principal follows the permanent-lock setting. The lock is instantiated as part of completed migration. The deployment snapshot taken on 15 November 2026 recorded a DBC pool that had not yet migrated; subsequent status is obtained from the live chain.

## 05 The Incentive Model: Revenue from Real Trading

ONRC's DBC base fee is **30 basis points (0.30%)**, with the DBC dynamic-fee mechanism disabled. For a trade with a fee base of 1,000 USDC, the nominal base trading fee is 3 USDC. The protocol distributes that fee under the DBC fee rules. ONRC's creator share is set to **100% of the portion allocable to creators and partners**.

| Component | Mechanism | Why it matters |
|---|---|---|
| Token supply | One billion units, mint authority revoked | A defined supply limit |
| Early price discovery | DBC trading curve | Open market price formation |
| Base trading fee | 0.30% | An identifiable cost parameter |
| Founder income | Protocol-allocated creator fees | Revenue tracks trading activity |
| Graduation | 750 USDC net quote reserve | A measurable transition trigger |
| Post-migration liquidity | 100% of creator LP permanently locked | Principal follows the disclosed lock setting |

The DBC protocol also receives its protocol-level fee share. The founder receives the creator allocation specified by the configuration, rather than the entire gross trading fee. Real fee receipts depend on executed trades, the charged asset, and protocol accounting. The founder is responsible for site maintenance, communications, brand materials, and community operations, funded through the project fee stream.

## 06 The Community: A Goose That Travels

OneirosCoin is currently maintained by one founder. Its cultural work has three threads: dream-inspired creative work, the goose as an internet-native character, and accessible information about what the on-chain system is doing.

**Consistent identity.** The name, ticker, and engraved goose emblem are kept consistent so that the community can recognize official materials even when similar tickers appear elsewhere.

**Shared expression.** The X and Telegram channels host illustrations, short-form content, conversations, and community activities. Contributors are encouraged to interpret the dream and goose motifs in their own work.

**Open information.** The official website links to the mint, pool, configuration account, whitepaper, and social channels. Material changes to public information are communicated openly.

A single-founder model keeps early coordination simple and establishes clear operational responsibility. The founder maintains project communications, published content, and the creator-fee account.

## 07 Roadmap: Milestones That Can Be Observed

| Phase | Focus | Position |
|---|---|---|
| 01 · Mainnet launch | Create ONRC, DBC pool, metadata, and the goose identity | Completed |
| 02 · Public foundation | Official website, bilingual whitepaper, on-chain links, social channels | Published; maintained |
| 03 · Market clarity | Improve wallet and venue guidance; explain fee and graduation tracking | Work direction |
| 04 · Cultural expansion | Extend original artwork, mythology-led content, and creative participation | Work direction |
| 05 · Graduation | On reaching the reserve threshold, migrate to DAMM v2 and publish LP-lock records | Triggered by conditions |

The roadmap separates delivered work, operating priorities, and the protocol-driven graduation event. Cultural growth depends on actual participation. The timing of graduation follows market activity and net reserves.

## 08 Canonical Accounts and Verification

On-chain accounts define the technical identity of ONRC. A search result, logo, or ticker is only a discovery aid.

| Account | Solana mainnet address |
|---|---|
| ONRC mint | `D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55` |
| DBC pool | `2zbY23A7UWMmdY14zgeneJw5jcdRwqYQu6K6XbsgDpgU` |
| DBC configuration | `DARJaFYLWWepZnmN4ezrTziU2ymRbZae1NhZYuetNc1E` |
| USDC mint | `EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v` |
| Creator / fee claimer | `9p9dNQSVoq3hD6iGG9k9WF2ozcMsfMQGY6ZSN2xq2GbY` |

Inspect the token on [Solscan](https://solscan.io/token/D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55). The [Meteora DBC overview](https://github.com/MeteoraAg/docs/blob/main/core-products/dbc/what-is-dbc.mdx) describes the underlying trading lifecycle. The deployment transactions for the configuration and the pool are confirmed on Solana mainnet.

## 09 Technical Appendix: The Engine Behind Price Discovery

Meteora DBC organizes price movement using a segmented liquidity curve. Within a simplified constant-product segment, let virtual ONRC reserve be `x` and virtual USDC reserve be `y`; the underlying relation is `x × y = k`. Buying increases relative USDC reserves and decreases relative ONRC reserves, moving the marginal price. Actual trade execution is shaped by the active segment, available liquidity, fees, and on-chain integer precision.

Meteora's curve description uses `L × (√P_high − √P_low)` to express the quote amount needed to traverse a price segment. A transaction that crosses multiple segments accumulates each segment's contribution. ONRC was configured using the official SDK `buildCurve` path, which uses the selected supply and graduation target to derive curve and migration parameters. The mathematics belongs to the established Meteora protocol. ONRC's design decisions are its launch settings, founder economics, and cultural identity.

The three most useful pre-trade checks are the correct mint address, current estimated output and slippage, and live USDC quote reserves. The underlying implementation is documented in the [Meteora DBC formulas](https://github.com/MeteoraAg/docs/blob/main/core-products/dbc/formulas.mdx) and [SDK source](https://github.com/MeteoraAg/dynamic-bonding-curve-sdk/blob/main/packages/dynamic-bonding-curve/src/helpers/buildCurve.ts).

## 10 Market and Operational Risks

ONRC is a freely priced meme token. Price volatility, thin early liquidity, execution slippage, smart-contract behavior, Solana network conditions, and exposure to the USDC quote asset all affect participation. The project's communications and creative output also depend on sustained founder involvement. Market participants should assess live liquidity, transaction costs, and their own risk tolerance before trading.

## Sources and Project Information

**Protocol implementation:** Meteora DBC overview and formulas; official DBC TypeScript SDK; Solana SPL Token Program; Meteora DAMM v2.  
**Whitepaper structure reviewed:** Bitcoin (2008), Ethereum (2014), Uniswap v3 (2021), Solana (2017). These projects do not sponsor or endorse ONRC.  
**Recorded mainnet snapshot:** 15 November 2026, 21:32 UTC; the config and pool were live, and migration had not occurred at that time.  
**Website:** https://yohakusama.github.io/oneiroscoin/  
**X:** https://x.com/oneiroscoin  |  **Telegram:** https://t.me/OneirosCoin  |  **Contact:** waylanus@gmail.com

**Version 1.0 · 16 November 2026**