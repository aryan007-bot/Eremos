<p align="center">
  <img src="docs/banner2.png" alt="Eremos Banner" width="100%"/>
</p>

<h1 align="center">🗿 Eremos</h1>
<p align="center">
  <em>Autonomous swarm agents for early on-chain signal detection — built for the Solana ecosystem</em>
</p>

<p align="center">
  <a href="https://github.com/EremosCore/Eremos/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/EremosCore/Eremos" alt="License"/>
  </a>
  <a href="https://github.com/EremosCore/Eremos/stargazers">
    <img src="https://img.shields.io/github/stars/EremosCore/Eremos?style=social" alt="Stars"/>
  </a>
  <a href="https://github.com/EremosCore/Eremos/network">
    <img src="https://img.shields.io/github/forks/EremosCore/Eremos?style=social" alt="Forks"/>
  </a>
  <a href="https://github.com/EremosCore/Eremos/releases">
    <img src="https://img.shields.io/github/v/release/EremosCore/Eremos" alt="Release"/>
  </a>
  <a href="https://github.com/EremosCore/Eremos/issues">
    <img src="https://img.shields.io/github/issues/EremosCore/Eremos" alt="Issues"/>
  </a>
</p>

---

## 🌌 Overview

Eremos is a **lightweight, modular framework** for deploying autonomous agents that monitor **Solana blockchain activity** — from wallet funding flows to contract deploy patterns.

These agents:
- 🔍 Detect **early signals** before they're obvious
- 🧩 Are **modular** & easily extendable
- 🌐 Integrate seamlessly into dev & analyst workflows

Built as a **public good** — fully open-source, community-friendly, and designed to enhance transparency.

---

<p align="center">
  <img src="docs/therontphd2.png" alt="Agent Theron" width="150"/><br/>
  <em>Theron — Agent (000)</em>
</p>

> **Meet Theron — Agent-000**  
> Passive. Pattern-sensitive. Modular and extendable by design.

---

## 📑 Table of Contents
- [✨ Features](#-features)
- [📡 Example Signal](#-example-signal)
- [📊 Signal Confidence](#-signal-confidence)
- [🛠 Tech Stack](#-tech-stack)
- [🚀 Quickstart](#-quickstart)
- [📂 Key Folders](#-key-folders)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)
- [🔗 Links](#-links)

---

## ✨ Features
✅ **Modular Agents** — Scoped logic for detecting wallet activity, contract spawns, and anomalies  
✅ **Signal Emission** — Structured, low-noise outputs for logging, alerting, or downstream processing  
✅ **Swarm Design** — Agents run independently but share utilities  
✅ **Launch Wallet Detection** — Trace freshly funded wallets, monitor contract interactions, and flag high-confidence deploys in real-time  
✅ **Ghost Watcher** — Detects dormant wallets that suddenly reactivate  

---

## 📡 Example Signal

```ts
[agent-observer] → fresh funding detected from kraken (wallet: 6Yxk...P2M8) at 04:41:12Z
[agent-observer] → contract probing detected within 4s (pump.fun interaction traced)
[agent-observer] → token created at 04:41:17Z (tx: 5gW...pump)
[agent-observer] → 5 bundle-linked wallets interacted within 8s of deploy
[agent-observer] → launch confidence spike (0.91) - emitting signal (elapsed: 13s)

{
  agent: "Observer",
  type: "launch_detected",
  glyph: "Δ",
  hash: "sig_c7f9a3d2bc",
  timestamp: "2025-06-12T04:41:25Z",
  source: "agent-observer",
  confidence: 0.91
}
