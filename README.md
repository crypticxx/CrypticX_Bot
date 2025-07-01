# WhatsApp Crypto Bot with AI + Admin Dashboard

This project includes:
- A WhatsApp bot (Node.js) using Twilio + OpenAI
- Multi-user crypto wallet support on Base, ETH, Polygon
- AES-encrypted private keys stored in MongoDB
- React + Tailwind Admin dashboard
- Deploy-ready on Render.com

## 🧠 Features
- Set and authenticate user PINs
- Named wallets (e.g. "dev wallet" ➝ 0xabc...)
- Send ETH with natural commands: `Send 0.01 ETH to dev`
- Multi-chain: Base, Ethereum, Polygon
- On-chain alerts for incoming/outgoing txs
- Admin Dashboard for viewing users, wallets, balances

## 📦 Folder Structure
```
/client         - Admin Dashboard (React + Tailwind)
/server         - WhatsApp bot (Node.js + Express)
render.yaml     - Render.com auto-deploy config
```

## 🛠 .env (for `/server`)
```
const mongoUri = process.env.MONGO_URI;
const baseRpc = process.env.BASE_RPC_URL;
const ethereumRpc = process.env.ETHEREUM_RPC_URL;
const polygonRpc = process.env.POLYGON_RPC_URL;
const openaiKey = process.env.OPENAI_API_KEY;
const accountSid = process.env.TWILIO_ACCOUNT_SID;
const authToken = process.env.TWILIO_AUTH_TOKEN;
const encryptionKey = process.env.ENCRYPTION_KEY;

## 🚀 Deployment
1. Push this repo to GitHub
2. Connect to Render.com
3. It auto-detects `render.yaml` and deploys both frontend and backend
