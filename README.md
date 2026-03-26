# 🐳 Whale Tracker Agent

A free automated crypto agent that monitors whale wallets across multiple chains and sends instant Telegram alerts when big money moves.

---

## What It Does

- Tracks **19 known whale wallets** across Ethereum, BNB Chain, Polygon, and Arbitrum
- Detects large token transfers between **$500K and $1M+**
- Classifies each move as **Bullish 🟢**, **Bearish 🔴**, or **Neutral ⚪**
- Sends formatted alerts straight to your **Telegram channel**
- Runs automatically every **15 minutes** — 24/7

---

## Alert Tiers

| Size | Label | Alert |
|---|---|---|
| $500K – $1M | Whale 🐳 | 📡 |
| $1M – $5M | Large Whale 🐋 | ⚠️ |
| $5M+ | Mega Whale 🦣 | 🚨 |

---

## Chains Covered

- ⟠ Ethereum
- ◈ BNB Chain
- ⬡ Polygon
- 🔵 Arbitrum

---

## Tech Stack

| Tool | Purpose | Cost |
|---|---|---|
| n8n Cloud | Workflow automation | Free |
| Moralis API | On-chain wallet data | Free |
| Telegram Bot | Alert delivery | Free |

**Total cost: $0/month**

---

## Setup

1. Import `whale-tracker-v4.2-final.json` into your n8n Cloud account
2. Get a free API key from [moralis.io](https://moralis.io)
3. Create a Telegram bot via [@BotFather](https://t.me/botfather)
4. Replace the 3 placeholder values in the workflow:
   - `YOUR_MORALIS_API_KEY` — in both Moralis nodes
   - `YOUR_TELEGRAM_CHAT_ID` — in the Telegram node
5. Activate the workflow

---

## Sample Alert

```
🚨 ⟠ Ethereum MEGA WHALE 🦣 🔴
───────────────────────
💰 2,300,000.00 USDT
💵 Est. Value: $2,300,000
👛 Wallet: 0x28C6...d60
🏷 Label: Binance Hot Wallet 1
📤 From: 0x28C6c062...
📥 To:   0xdac17f95...
───────────────────────
📊 📉 Sending — Potential distribution
💼 Balance: 0.00 ETH
───────────────────────
⏰ Thu, 05 Mar 2026 13:17:00 UTC
```

---

## Wallet Sources

All 19 wallet addresses are sourced from publicly known exchange wallets via Etherscan labels and Arkham Intelligence's public database.

---

Built with n8n · Moralis · Telegram
