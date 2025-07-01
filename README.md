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
MONGO_URI=your_mongodb_connection_string
BASE_RPC_URL=https://base-sepolia...
ETHEREUM_RPC_URL=https://mainnet.infura.io/v3/...
POLYGON_RPC_URL=https://polygon-rpc.com
OPENAI_API_KEY=sk-...
TWILIO_ACCOUNT_SID=...
TWILIO_AUTH_TOKEN=...
ENCRYPTION_KEY=32charlongpassword1234567890
```

## 🚀 Deployment
1. Push this repo to GitHub
2. Connect to Render.com
3. It auto-detects `render.yaml` and deploys both frontend and backend