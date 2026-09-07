# 🍪 CookieFlow: Next-Gen SVM Portal & Interactive Explorer for Cookie Chain

[![Cookie Chain](https://img.shields.io/badge/Network-Cookie%20Chain%20SVM-f59e0b.svg)](https://cookiechain.wtf)
[![Engine](https://img.shields.io/badge/Solana%20Core-4.1.2%20Agave-10b981.svg)](https://github.com/solana-labs/solana)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-Available-blue.svg)](https://vincentsai.github.io/cookieflow-svm/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **CookieFlow** is a modern, high-performance, developer-friendly Web3 portal and interactive workstation purpose-built for the **Cookie Chain** SVM ecosystem. Designed to showcase Cookie Chain's sub-second transaction finality, ultra-low gas execution, and developer ergonomics.

---

## 🌟 Overview & Highlights

Cookie Chain brings the speed, modularity, and power of the Solana Virtual Machine (SVM) into a rapid-iteration, community-driven decentralized environment. **CookieFlow** delivers an end-to-end user and builder interface that interacts natively with Cookie Chain's RPC (`https://rpc.cookiescan.io`).

### Key Capabilities

1. ⚡ **Live On-Chain Telemetry**:
   - Real-time polling of current SVM slot, block height, Solana Core version (`4.1.2 Agave`), and real-time JSON-RPC round-trip latency.
2. 👛 **Multi-Wallet Integration (Nightly-First)**:
   - Built-in support for **Nightly Wallet** (Cookie Chain's preferred multi-chain wallet) as well as Phantom and Solflare.
   - Dynamic balance fetching and account state detection.
3. ✍️ **SPL On-Chain Memo Inscription**:
   - Write immutable, censorship-resistant text records directly into the Cookie Chain ledger using the native SPL Memo Program (`MemoSq4gqABAXKb96qnH8TysNcWxMyWCqXgDLGmfcHr`).
4. 💸 **Instant SVM Native Transfer Engine**:
   - Zero-friction token transfers with pre-flight fee calculation, signature tracking, and deep-links to the CookieScan block explorer.
5. 🛠️ **Developer JSON-RPC Sandbox**:
   - Interactive RPC explorer enabling developers to test raw SVM calls (`getSlot`, `getBlockHeight`, `getVersion`, `getClusterNodes`, `getSupply`) with live latency and response formatting.
6. 🍪 **Cookie Ecosystem Directory**:
   - Integrated quick links to Cookiebox, Cookieswap, CookieScan DAS API (`api.cookiescan.io`), and community hubs.

---

## 🚀 Live Demo & Deployment

* **Live Application URL**: [https://vincentsai.github.io/cookieflow-svm/](https://vincentsai.github.io/cookieflow-svm/)
* **Official Cookie Chain RPC**: `https://rpc.cookiescan.io`
* **Block Explorer & API**: `https://api.cookiescan.io`
* **Cookie Chain Portal**: `https://www.cookiechain.wtf`

---

## ⚙️ Architecture & Network Specs

| Parameter | Configuration / Value |
| :--- | :--- |
| **Virtual Machine** | Solana Virtual Machine (SVM) |
| **Client Engine** | Agave `4.1.2` (Solana Feature-Set: 3345198602) |
| **RPC Endpoint** | `https://rpc.cookiescan.io` |
| **Explorer & DAS API** | `https://api.cookiescan.io` |
| **Primary System Program** | `11111111111111111111111111111111` |
| **SPL Memo Program** | `MemoSq4gqABAXKb96qnH8TysNcWxMyWCqXgDLGmfcHr` |
| **Average Finality** | Sub-second (~400ms) |
| **Average Deployment Cost**| ~$0.05 |

---

## 💻 Tech Stack

- **Frontend Core**: Modern semantic HTML5, Vanilla JavaScript (ES6+)
- **Styling**: Tailwind CSS (Dark cyberpunk mode tailored for Cookie Chain)
- **Web3 Engine**: `@solana/web3.js` (SVM compatibility layer)
- **Icons**: Lucide Icons
- **Deployment**: Static zero-dependency architecture, easily hosted on GitHub Pages, Vercel, or IPFS/Arweave.

---

## 🛠️ Local Development & Quickstart

Clone the repository and launch directly in any modern browser:

```bash
# Clone the repository
git clone https://github.com/VincentSai/cookieflow-svm.git

# Navigate into project directory
cd cookieflow-svm

# Serve locally using any HTTP server
python -m http.server 8080
# Or using Node.js:
# npx serve .
```

Open your browser at `http://localhost:8080`.

---

## 📱 User Walkthrough

1. **Connect Wallet**: Click `Connect Wallet` on the top right. Select **Nightly Wallet** (or Phantom).
2. **Inspect Telemetry**: Watch the live Slot and Block Height tick in real time via direct queries to `rpc.cookiescan.io`.
3. **Inscribe a Memo**: Go to the *On-Chain Inscription* tab, type a custom greeting, and click `Sign & Inscribe On-Chain`. Approve the transaction in your wallet.
4. **View Confirmation**: Once submitted, click the provided transaction link to inspect the block and signature on CookieScan.
5. **Developer Sandbox**: Switch to the *RPC Sandbox* tab to inspect cluster node metrics and runtime versioning.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE). Built for the Cookie Chain ecosystem and Superteam Earn Builders.
