# Auto Swap Bot for PRJX (Project X) on hyperEVM

<img width="1500" height="987" alt="image" src="https://github.com/user-attachments/assets/bc9a7116-be5c-420a-883b-c5c8db44e7e6" />

## 🚀 Features
- Daily automated transactions with randomized frequency and timing

- HYPE ↔ USDT0 swaps using on-chain in DEX PRJX (Project X)

- Dynamic delay and transaction range per day (configured via .env)

## 📦 Installation
Clone the repository and install dependencies:

```bash
git clone https://github.com/Kurisaitou/auto-swap-prjx-on-hyperEVM.git
```
```bash
cd auto-swap-prjx-on-hyperEVM
```
```bash
npm install
```

## ⚙️ Environment Setup
Create a .env file in the project root:
```bash
nano .env
```
Fill in your wallet details and configure your preferred settings:
```bash
RPC_URL=https://rpc.hyperliquid.xyz/evm
PRIVATE_KEY=your_privatekey

# 1 = legacy gas (gasPrice). 0 = try EIP-1559 then fallback
USE_LEGACY_GAS=1

# Keep some native HYPE for gas so you don't run out
GAS_RESERVE_HYPE=0.001

# ===== Daily plan (UTC) ===== (you can change)
DAILY_TX_MIN=6
DAILY_TX_MAX=12

# ===== Swap amounts ===== (you can change)
# HYPE -> USDT0: random amount range (HYPE)
HYPE_SWAP_MIN=0.1
HYPE_SWAP_MAX=0.9
# (USDT0 -> HYPE always swaps ALL balance)

# ===== Delay between transactions (seconds) ===== (you can change)
DELAY_MIN_SEC=60
DELAY_MAX_SEC=180

# ===== Router/Pool config =====
# Try these fee tiers in order until success
POOL_FEES=500,100,3000,10000
DEADLINE_SEC=600
```

## ▶️ Running the Bot
To start the bot:
```bash
node index.js
```

## 🎯 Goal
Maximize your point with the PRJX (Project X) boost your chances of earning more rewards from PRJX (Project X) — automatically.

## 🔖 Tags
#hyperevm #airdrop #swap #bot #crypto #web3 #automation #trading #prjx #dex #stake #hype #project-x
