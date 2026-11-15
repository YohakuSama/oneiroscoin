# OneirosCoin (ONRC)

Official English-language website for OneirosCoin, a Solana meme token.

- Website (once GitHub Pages is enabled): https://yohakusama.github.io/oneiroscoin/
- Token mint: `D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55`
- Meteora DBC pool: `2zbY23A7UWMmdY14zgeneJw5jcdRwqYQu6K6XbsgDpgU`
- X: https://x.com/oneiroscoin
- Telegram: https://t.me/OneirosCoin
- Contact: waylanus@gmail.com

## Whitepaper / 白皮书

Version 1.0, published 16 November 2026. Two equivalent language editions are published in the official website:

- **English (read online / print to PDF):** https://yohakusama.github.io/oneiroscoin/whitepaper/en/
- **简体中文（在线阅读 / 打印保存 PDF）：** https://yohakusama.github.io/oneiroscoin/whitepaper/zh/
- **English Markdown source:** [docs/whitepaper-en.md](docs/whitepaper-en.md)
- **中文 Markdown 原文：** [docs/whitepaper-zh.md](docs/whitepaper-zh.md)

The whitepapers distinguish verified mainnet observations from future migration conditions and unknown distribution details. At the referenced 15 November 2026 audit snapshot, the DBC pool had **not yet graduated or migrated**. Its configuration specifies 750 USDC graduation and 100% creator permanent-locked LP allocation **after successful migration**, not a present-day guarantee that DAMM v2 liquidity is locked.

Whitepapers are informational project disclosures, not third-party security audits or promises of investment returns.

## Publish with GitHub Pages

1. Open **Settings > Pages** for this repository.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Set the branch to **main**, directory to **/(root)**, and click **Save**.
4. Visit https://yohakusama.github.io/oneiroscoin/ once the Pages deployment completes.

The website is a single self-contained `index.html`. Images are served from the already-published Irys gateway metadata asset. No build step or wallet keys are required.

The 100% permanent liquidity lock is configured for a future DAMM v2 migration after the bonding curve graduates. The actual lock has not yet occurred.
