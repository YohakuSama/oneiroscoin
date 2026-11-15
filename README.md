# OneirosCoin (ONRC)

Official English-language website for OneirosCoin, a Solana meme token.

- Website (once GitHub Pages is enabled): https://yohakusama.github.io/oneiroscoin/
- Token mint: `D52WmiMiEvfj4qXbpZP7PvtcUx3QWnaJJfERJfNSkB55`
- Meteora DBC pool: `2zbY23A7UWMmdY14zgeneJw5jcdRwqYQu6K6XbsgDpgU`
- X: https://x.com/oneiroscoin
- Telegram: https://t.me/OneirosCoin
- Contact: waylanus@gmail.com

## Whitepaper / 白皮书

**OneirosCoin Project Whitepaper 1.0 (16 November 2026).**

- [English whitepaper](https://yohakusama.github.io/oneiroscoin/whitepaper/en/) — vision, token design, DBC market, liquidity, founder-fee economics, community and roadmap.
- [中文版白皮书](https://yohakusama.github.io/oneiroscoin/whitepaper/zh/) — 项目愿景、发行与分配、市场机制、创始人经济模型、社群与路线图。
- [English source](docs/whitepaper-en.md)
- [中文原稿](docs/whitepaper-zh.md)

The whitepaper describes the founder's stated allocation policy: one founder, no reserved founder tokens, and project income from allocated creator trading fees. Network and token configuration are traceable to the listed Solana accounts. The whitepaper distinguishes the configured post-graduation LP lock from the actual migration event.

## Publish with GitHub Pages

1. Open **Settings > Pages** for this repository.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Set the branch to **main**, directory to **/(root)**, and click **Save**.
4. Visit https://yohakusama.github.io/oneiroscoin/ once the Pages deployment completes.

The website is a single self-contained `index.html`. Images are served from the already-published Irys gateway metadata asset. No build step or wallet keys are required.

The 100% permanent liquidity lock is configured for a future DAMM v2 migration after the bonding curve graduates. The actual lock has not yet occurred.
