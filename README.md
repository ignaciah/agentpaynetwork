
┌──────────────────────────────┐
│          Frontend            │
│  - Policy config UI          │
│  - Run agent button          │
│  - Activity dashboard        │
└──────────────┬──────────────┘
               │ REST API
┌──────────────▼──────────────┐
│           Backend            │
│  - AI Agent logic            │
│  - Merchant mock API         │
│  - ethers.js contract calls  │
└──────────────┬──────────────┘
               │
┌──────────────▼──────────────┐
│     AgentWalletManager       │
│  - Holds MNEE                │
│  - Enforces policy           │
│  - Pays merchants            │
│  - Splits revenue            │
└──────────────┬──────────────┘
               │
┌──────────────▼──────────────┐
│            MNEE              │
│ USD-backed stablecoin (ERC20)│
│ 0x8ccedbAe4916b79da7F3F612…  │
└──────────────────────────────┘
# agentpaynetwork
The MNEE Agent Market is a functional prototype that demonstrates the power of programmable money, specifically using the MNEE USD-backed stablecoin on Ethereum, to unlock new possibilities in AI automation, digital commerce, and financial coordination.  This project showcases how an AI agent can securely manage, spend, and transfer MNEE. 
MNEE Agent Market
Programmable Money for AI Agents, Digital Commerce & Automated Finance
MNEE Agent Market is a working prototype demonstrating how programmable money—powered by the MNEE USD‑backed stablecoin on Ethereum—enables new forms of digital commerce, AI automation, and financial coordination.

This project shows how an AI agent can safely hold, spend, and route MNEE under strict on‑chain rules defined by a human owner.
Merchants get paid automatically. Collaborators receive revenue shares.
All actions are enforced by smart contracts and visible on-chain.

🌐 Why This Matters
AI agents are becoming powerful decision-makers, but they can’t safely manage money.
Businesses still rely on manual approvals, invoices, and spreadsheets.

Programmable money changes that.

With MNEE + smart contracts:

Agents can pay for services autonomously

Merchants can offer pay‑per‑use digital commerce

Teams can coordinate automatic revenue splits

Owners stay protected by on‑chain spending policies

This unlocks a new class of autonomous digital commerce.

🚀 What We Built
1. AgentWalletManager.sol
A programmable wallet contract that:

Holds MNEE for an owner

Enforces a spending policy

Allows a designated AI agent to spend within limits

Pays merchants in MNEE

Automatically routes collaborator shares

Supports bonus payouts for successful outcomes

The contract integrates directly with the MNEE token at:

Code
0x8ccedbAe4916b79da7F3F612EfB2EB93A2bFD6cF
2. AI Agent (Backend Service)
A lightweight AI agent that:

Reads the owner’s on-chain policy

Scans for “opportunities” (mock APIs)

Decides when to purchase a digital service

Calls the smart contract to pay merchants in MNEE

Triggers bonus payouts when results are good

This demonstrates autonomous commerce powered by programmable money.

3. Frontend Dashboard
A clean UI that lets users:

Configure agent policies

Fund the wallet with MNEE

Run the AI agent

Watch real-time payment flows

View on-chain activity logs

Perfect for a hackathon demo.
