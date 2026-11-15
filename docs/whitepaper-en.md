# OneirosCoin (ONRC)
## Project Whitepaper · English Edition · Version 1.0

**Publication date:** 16 November 2026  
**Network:** Solana mainnet-beta  
**Official website:** https://yohakusama.github.io/oneiroscoin/  
**Token mint:** `D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55`  
**Contact:** waylanus@gmail.com

> **Scope and evidence.** This document describes the OneirosCoin token, the on-chain configuration observed in the project's 15 November 2026 audit snapshot, and material limitations. It is a project disclosure, not a claim of technological innovation, an independent security audit, a prospectus, or investment advice. Facts may change after the verification time; verify live accounts before transacting.

## 1. Executive summary

OneirosCoin (ticker **ONRC**) is a Solana meme token with a mythical goose identity inspired by the *Oneiroi*, dream spirits in Greek mythology. Its premise is cultural and community-oriented. ONRC does not introduce a new blockchain, consensus protocol, decentralized exchange, oracle, or payment network. It uses existing Solana token infrastructure and Meteora's Dynamic Bonding Curve (DBC).

The verified token supply is **1,000,000,000 ONRC**, with **six decimals**. Its mint and freeze authorities have been revoked. The initial ONRC/USDC DBC pool is configured with a **0.30% base trading fee**, **disabled DBC dynamic trading fees**, and a **750 USDC quote-reserve graduation threshold**. If migration conditions are met and migration is executed, the configured destination is **Meteora DAMM v2**, with **100% of the creator LP allocation designated as permanently locked**. This is a configuration for the future migration, not proof that migrated liquidity has already been locked.

As of the public-state snapshot recorded at **2026-11-15 21:32 UTC**, the DBC pool had **0 USDC** in quoted reserve, showed **0%** graduation progress, and **had not migrated**. This is a dated observation, not a live market quotation.

## 2. Purpose and scope

### 2.1 Cultural identity

The name references the Greek mythological dream spirits. The goose, coin portrait, and tagline “Born from a dream. Destined for nothing. Honk your dreams.” are original project branding. The goose is not presented as a literal figure from the ancient sources.

### 2.2 What ONRC does today

ONRC is a transferable SPL token deployed on Solana. Its initial market was configured as a DBC pool quoted in USDC. Users can inspect the mint, pool, configuration, and transaction history using Solana explorers and public RPC interfaces. Trading availability, execution prices, and third-party integrations depend on current chain state and infrastructure.

### 2.3 What ONRC does not provide

There is **no documented token-backed claim to equity, dividends, revenue, treasury assets, redemption at a fixed value, governance votes, staking yield, or guaranteed services**. The project's public materials do not establish any of those rights. This whitepaper does not introduce such rights by implication.

## 3. Verifiable token specification

| Field | Value / observation |
|---|---|
| Name / ticker | OneirosCoin / ONRC |
| Network | Solana mainnet-beta |
| Token standard | SPL Token (legacy Token Program) |
| Mint | `D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55` |
| Decimal places | 6 |
| Total observed supply | 1,000,000,000 ONRC |
| Raw supply | 1,000,000,000,000,000 base units |
| Mint authority | Revoked (null) |
| Freeze authority | Revoked (null) |
| Token metadata | OneirosCoin / ONRC; immutable on-chain metadata |
| Quote token | USDC on Solana: `EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v` |
| DBC config account | `DARJaFYLWWepZnmN4ezrTziU2ymRbZae1NhZYuetNc1E` |
| DBC pool account | `2zbY23A7UWMmdY14zgeneJw5jcdRwqYQu6K6XbsgDpgU` |
| Published metadata URI | `https://gateway.irys.xyz/3S2vDEHeS4HQFsU3ePvzmpvB4Z3yxuWJznT8fLyAfpzK` |

**Meaning of a fixed supply.** Revoking mint authority prevents ordinary further issuance under this mint. It does **not** establish who controls existing tokens, ensure equitable distribution, guarantee exchange availability, or eliminate price risk. The audited metadata account was marked immutable; this limits edits to that metadata, not off-chain website or social-account changes.

## 4. Launch mechanism and pool lifecycle

### 4.1 Dynamic Bonding Curve

The project uses Meteora DBC, an existing permissionless Solana launch program. Before migration, swaps take place against a virtual pool according to a configurable on-chain price curve. Prices and slippage depend on the current curve, reserves, and trade size. The token does not promise a stable price or a minimum exit price.

### 4.2 Quote asset and graduation

The quote asset is Solana USDC. The DBC configuration specifies **750 USDC** as the migration quote-reserve threshold. This number is a condition for a pool lifecycle transition. It is **not** a project treasury balance, a guaranteed fundraising target, an investor protection fund, or a minimum liquidity commitment by the team. Meteora documents a mainnet keeper route for eligible USDC DBC pools at this threshold; actual migration still depends on applicable program conditions and services [5].

### 4.3 After graduation

The intended destination is Meteora **DAMM v2**. The audited configuration specifies **100% creator permanent-locked LP**, **0% creator withdrawable LP**, **0% partner withdrawable LP**, and **0% partner permanent-locked LP**. These percentages apply to the migrated liquidity position allocation, **not to the entire token supply**. Liquidity locks cannot be verified as completed until the migration and destination positions exist on-chain.

Permanent LP locking restricts withdrawal of locked principal. It does **not** necessarily prevent claims on trading fees accrued to a locked position; Meteora's DAMM v2 documentation distinguishes liquidity withdrawal from fee claims [6]. Therefore, permanent liquidity locking should never be described as a waiver of all creator economics.

## 5. Trading fees and creator economics

| Setting | Observed configuration |
|---|---|
| Initial DBC base trading fee | 30 basis points (0.30%) |
| Initial DBC dynamic fee | Disabled |
| Creator allocation of non-protocol DBC fee | 100% of the creator/partner share |
| Configured DBC pool-creation fee | 0 |
| Graduation destination | DAMM v2 |
| Selected DAMM v2 base fee option | 0.30% |
| Permanent LP allocation after migration | 100% creator-locked; 0% withdrawable |

A **0.30% base fee** means a configured fee of 0.003 units per 1 unit of traded notional before other transaction-specific costs. It is not a promise about total wallet costs, which can also include network fees, routing fees, price impact, and slippage. Meteora's DBC splits trading fees into protocol and non-protocol components; **100% creator allocation does not mean 100% of the gross trading fee reaches the creator** [4].

The on-chain creator/fee-claimer/leftover-receiver address at the audit time was `9p9dNQSVoq3hD6iGG9k9WF2ozcMsfMQGY6ZSN2xq2GbY`. The public evidence does not establish a binding commitment to spend any claimed fees on liquidity, development, marketing, grants, buybacks, or burns. No such commitment is made here. Protocol-level fees and migration charges are governed by Meteora's applicable program rules [4].

## 6. Supply, distribution, and ownership disclosures

**Fixed supply is verified; distribution policy is not.** The observed mint supply was one billion tokens. The available audit does not establish a complete initial allocation ledger, beneficial ownership of all addresses, team allocations, investor allocations, vesting agreements, or exchange holdings. The project therefore does not claim “zero team allocation,” “100% fair launch,” “no insiders,” or “fully decentralized ownership.”

Token balances and transfers are public on Solana. A responsible future disclosure would include a dated allocation table with wallet addresses, controlled-entity relationships, and any transfers to team, community, or liquidity accounts. Until such a disclosure is independently checked, readers should treat distribution concentration as **unknown**.

The presence of an official creator/fee-receiver wallet does not by itself indicate that its balances belong to a public treasury or a legally segregated foundation. No treasury governance scheme has been documented.

## 7. Governance, operations, and planned activity

### 7.1 Current governance

There is no verified on-chain ONRC token-voting system, treasury DAO, or tokenholder-controlled protocol upgrade process. Website content and social communications are operated off-chain. The project has a published contact email, `waylanus@gmail.com`. The identity and jurisdiction of any formal legal operating entity have not been established by the supplied public records.

### 7.2 Ongoing disclosures, not guarantees

The project intends to maintain accessible English and Chinese documentation, public links to its Solana accounts, and dated corrections where errors are found. Potential future community or artistic initiatives require separate announcements and evidence before they may be treated as product commitments. **There is no guaranteed development schedule, token listing, marketing budget, exchange partnership, or future utility specified in this document.**

### 7.3 Documents versus chain state

This whitepaper is explanatory and does not override on-chain program behavior. For claims about mint supply, permissions, pool configuration, and migration, readers should prioritize verified chain state over screenshots, cached explorer displays, or website prose.

## 8. Security and operational considerations

The project uses the Solana SPL Token Program and third-party Meteora DBC/DAMM v2 programs. Using known programs does not eliminate risks from software defects, permission structures, protocol upgrades, RPC outages, fee behavior, external services, or wallet compromise. An earlier read-only project audit checked selected public account fields and transaction finality; **that review was not an independent code security audit or formal certification**.

The observed mint authority and freeze authority were null, and the metadata was immutable. These are useful constraints but cannot guarantee safe markets, accurate external interfaces, fair distribution, or protection against every form of malicious trading. Users must independently verify contract addresses, wallet prompts, approvals, and service domains.

## 9. Material risks

**Speculation and total loss.** ONRC has no guaranteed redemption value or cash flow. Its market price may be extremely volatile and can fall to zero.

**Liquidity and execution.** A small or inactive DBC pool may offer inadequate exit liquidity. Large trades can face severe slippage, adverse price movement, MEV, sandwich attacks, transaction failure, or trading interruption.

**Distribution and control.** Actual ownership concentration and insider holdings have not been fully disclosed. Fee-claim rights exist, and permanent LP locks do not waive all fee income.

**Migration.** Graduation at 750 USDC and subsequent DAMM v2 migration are configured events, not guaranteed deadlines or completed states. A delay, failure, or change in third-party services can affect the outcome.

**Technical and custodial.** Solana, Meteora, wallets, token accounts, public RPC providers, Irys metadata hosting, websites, and domain accounts have independent availability and security risks. Loss of wallet keys can cause irreversible asset loss.

**Regulatory and tax.** Laws differ across jurisdictions and can change. Buyers and holders are responsible for assessing their own eligibility, legal obligations, and tax consequences.

**Information quality.** Explorer indexing, project pages, and screenshots can be inaccurate or stale. The exact audit snapshot cited here does not establish current price, holder count, trading depth, market capitalization, or future outcomes.

## 10. Verification record and evidence limits

| Item | Status at the referenced audit |
|---|---|
| DBC config and pool accounts | Present; decoded successfully |
| ONRC mint | Present; 1,000,000,000 supply, 6 decimals |
| Mint / freeze authorities | Both revoked |
| Metadata | Present, immutable, expected name, symbol, URI |
| DBC fee | 0.30% base; dynamic fee disabled |
| Graduation setting | 750 USDC quote reserve |
| Migration setting | DAMM v2; 100% creator permanent-locked LP |
| DBC reserve / progress | 0 USDC / 0% at 2026-11-15 21:32 UTC |
| DAMM v2 migration and final LP lock | **Not completed at that audit time** |
| Formal third-party security audit | **Not documented in the supplied evidence** |
| Token allocation by beneficial owner | **Not established by the supplied evidence** |

The snapshot was collected from a read-only Solana mainnet inspection on 15 November 2026, 21:32 UTC. Its checks passed, with one informational warning: DBC SDK token-supply fields were unavailable, so mint supply was checked independently. Both create-config and create-pool transaction records were finalized without execution errors in that inspection. **This does not establish the present pool reserve or migration state.**

## 11. Public addresses and communication

- **Official mint:** `D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55`
- **DBC pool:** `2zbY23A7UWMmdY14zgeneJw5jcdRwqYQu6K6XbsgDpgU`
- **DBC config:** `DARJaFYLWWepZnmN4ezrTziU2ymRbZae1NhZYuetNc1E`
- **Creator / fee-claimer:** `9p9dNQSVoq3hD6iGG9k9WF2ozcMsfMQGY6ZSN2xq2GbY`
- **Metadata:** https://gateway.irys.xyz/3S2vDEHeS4HQFsU3ePvzmpvB4Z3yxuWJznT8fLyAfpzK
- **Solscan token:** https://solscan.io/token/D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55
- **Project website:** https://yohakusama.github.io/oneiroscoin/
- **X:** https://x.com/oneiroscoin
- **Telegram:** https://t.me/OneirosCoin
- **Project email:** waylanus@gmail.com

## 12. References and editorial method

The presentation of the problem, design, mechanisms, risks, and independent verification is informed by established whitepaper conventions. The following publications are **structural and technical references**, not partners, endorsements, or claims of equivalence to ONRC.

1. Satoshi Nakamoto, *Bitcoin: A Peer-to-Peer Electronic Cash System* (2008). https://bitcoin.org/bitcoin.pdf
2. Ethereum, *A Next-Generation Smart Contract and Decentralized Application Platform* (2014). https://ethereum.org/whitepaper/
3. Solana, *A New Architecture for a High Performance Blockchain*. https://solana.com/solana-whitepaper.pdf
4. Meteora, *DBC Formulas* and *Launch Configurations*. https://github.com/MeteoraAg/docs/blob/main/core-products/dbc/formulas.mdx and https://github.com/MeteoraAg/docs/blob/main/core-products/dbc/launch-configurations.mdx
5. Meteora, *DBC Developer Guide and Migration Keeper Thresholds*. https://github.com/MeteoraAg/docs/blob/main/developer-guides/dbc/index.mdx
6. Meteora, *DAMM v2 Overview and LP Locks*. https://github.com/MeteoraAg/docs/blob/main/core-products/damm-v2/what-is-damm-v2.mdx and https://github.com/MeteoraAg/docs/blob/main/user-guides/how-to-use-damm-v2/damm-v2-pool-detail.mdx
7. Uniswap, *Uniswap v3 Core Whitepaper* (2021). https://app.uniswap.org/whitepaper-v3.pdf
8. OneirosCoin, *read-only on-chain verification snapshot* (15 November 2026, 21:32 UTC). Primary public accounts and transaction signatures are provided in Sections 3 and 11; the audit is a project-run inspection and not an independent protocol audit.

## Version and disclaimer

**Version 1.0 · 16 November 2026.** This text records presently evidenced project facts and explicit uncertainties. Any future revision should include a date, a change summary, and fresh chain-state verification. A translated edition must preserve the same substantive statements. This document is informational, not an offer to sell securities or a statement that tokens are suitable for any reader. Nothing here guarantees price appreciation, liquidity, graduation, rewards, or safety.