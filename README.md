# 🎲 BaseFlip

**Provably fair coin flip & dice casino on [Base](https://base.org), powered by Chainlink VRF.**

![Base](https://img.shields.io/badge/Chain-Base-0052FF?style=flat-square&logo=coinbase)
![Solidity](https://img.shields.io/badge/Solidity-0.8.20-363636?style=flat-square&logo=solidity)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## Overview

BaseFlip is an onchain casino on Base L2 with two games:

- **CoinFlip** — bet ETH on heads or tails, win 1.96x
- **Dice** — pick a threshold (2–98), roll over/under, payout scales with risk

Randomness is provided by **Chainlink VRF v2.5** — fully verifiable on-chain.

---

## Contracts

| Contract | Network | Address |
|----------|---------|---------|
| `BaseFlip` | Base Sepolia | `0x...` |
| `BaseDice`  | Base Sepolia | `0x...` |

---

## Getting started

```bash
git clone https://github.com/YOUR_USERNAME/base-flip
cd base-flip
npm install
cp .env.example .env
npm run compile
npm test
npm run deploy:testnet
```

---

## House edge

2% on all games. Max bet is capped at 1% of contract balance.

---

## Security

- Chainlink VRF for tamper-proof randomness
- `ReentrancyGuard` on all payable functions
- Max bet ceiling to protect liquidity

> ⚠️ Unaudited. Use on testnet only.

---

## License

MIT
