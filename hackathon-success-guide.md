# 🛠️ **Hackathon Success Guide**

## 📅 Upcoming Hackathons

- [ETHGlobal Prague](https://ethglobal.com/events/prague) - May 30 - June 1, 2025
- [ETHGlobal Cannes](https://ethglobal.com/events/cannes) - July 4 - 6, 2025
- [ETHGlobal New York 2025](https://ethglobal.com/events/newyork2025) - August 15 - 17, 2025
- [ETHGlobal Buenos Aires](https://ethglobal.com/events/buenosaires) - November 21 - 23, 2025

## 🟢 Introduction

**LayerZero** is an **omnichain interoperability protocol** that enables seamless communication between different blockchains. It allows developers to build omnichain applications (OApps) that can interact across multiple chains as if they were on a single chain.

**Why build with LayerZero at a hackathon?**

- **Reach More Users:** Deploy your dApp once and interact with users and assets across all supported chains.
- **Unify Liquidity:** Avoid fragmented liquidity; build DEXes, lending platforms, etc., that leverage a shared cross-chain pool.
- **Simplify Development:** Build complex cross-chain logic using familiar tools (Hardhat, Foundry, etc.) and LayerZero's contract standards (OApp, OFT, ONFT). Get started quickly with the `create-lz-oapp` CLI.
- **Enhance Security:** Benefit from a configurable, decentralized security model using Decentralized Verifier Networks (DVNs).
- **Improve User Experience:** Abstract away cross-chain complexities, offering seamless interactions without users needing multiple wallets or bridging steps.
- **Innovate:** Explore novel use cases like cross-chain governance, gaming, data queries (`lzRead`), and complex multi-step workflows (Composability).

## 🚀 Getting Started: Quick Links

- 💬 **[Join LayerZero Discord](https://discord.gg/ktbvm8Nkcr)** - Get support, ask questions, and connect with the team and other builders.
- 📖 **[LayerZero Docs](https://docs.layerzero.network/v2/developers/evm/overview)** - Start with docs. Covering OApp, OFT, ONFT standards, configuration, tooling.
- 🛠️ **[CLI Quickstart Guide](https://docs.layerzero.network/v2/developers/evm/create-lz-oapp/start)** - Fastest way to start building with `create-lz-oapp`. Quickly scaffold a Hardhat/Foundry project.
- ⚙️ **Core Concepts**
  - [What is LayerZero?](https://docs.layerzero.network/v2/concepts/getting-started/what-is-layerzero)
  - [Protocol Overview](https://docs.layerzero.network/v2/concepts/protocol/protocol-overview)
  - [Glossary](https://docs.layerzero.network/v2/concepts/glossary)
- 💡 **[Example Projects](https://github.com/LayerZero-Labs/devtools/tree/main/examples)** - Example projects can be found in [devtools/examples](https://github.com/LayerZero-Labs/devtools/tree/main/examples) repo, including OApp, ONFT, lzRead, and multiple VM-specific or use case-specific examples.
- **🔍 LayerZero Scan** - Transaction explorer for [Mainnet](https://layerzeroscan.com/) and [Testnet](https://testnet.layerzeroscan.com/)
- **📹 Tutorials & Workshop Recordings:**
  - There's usually a live workshop before the hackathon starts. It's a good idea to attend this. If you miss it, here are some recordings of past workshops:
  - [Intro to LayerZero V2 & Omnichain Apps for Beginners](https://www.youtube.com/watch?v=W0J_Jz76apE)
  - [Mastering Cross Chain State Retrieval](https://www.youtube.com/watch?v=DEvfd44q5ys)

## 🎯 Hackathon Project Ideas

A few project idea starters, to give you some inspiration.

- **Omnichain Yield Aggregator:** Create a dApp that automatically finds the best yield opportunities for a specific asset (e.g., USDC) across multiple supported chains and allows users to deposit/withdraw from a single interface, using `lzRead` for cross-chain state checks.
- **Cross-Chain NFT Utility Unlocker:** Build an ONFT project where owning the NFT on _any_ supported chain grants access to specific features or content within a dApp deployed on a different chain.
- **Composable DeFi Strategy Builder:** Leverage LayerZero Composability to create a dApp where users can chain together actions across different protocols on multiple chains in a sequence managed by LayerZero messages. For example:
  - Swap on Uniswap (ETH) →
  - Bridge Asset via OFT →
  - Deposit into Aave (Polygon)
- **Decentralized Cross-Chain Oracle:** Use `lzRead` and potentially `lzMap`/`lzReduce` to build a system where contracts can request aggregated data (e.g., median token price) from multiple chains, providing a more resilient oracle feed.
- **Omnichain Governance Portal:** Design a system where a DAO's governance token (OFT) holders can vote on proposals from any chain where the token exists, with votes securely tallied on a designated home chain via LayerZero messaging.

## 💰 Prizes & Bounties

[Bounties for ETHGlobal Prague](https://ethglobal.com/events/prague/prizes#layerzero) (the nearest hackathon) are listed below.

#### **lzRead Track - $4000**

- 1st place - $2,500
- 2nd place - $1,500

Develop a comprehensive solution using [LayerZero Read](https://docs.layerzero.network/v2/developers/evm/lzread/overview) (`lzRead`) to request, retrieve, and process external on-chain state from destination blockchains.

Your solution should use `lzRead` to perform cross-chain data queries and update state on the source or another destination chain based on the retrieved data.

Projects should focus on secure and efficient cross-chain data queries, using features like `lzMap()` and `lzReduce()` for off-chain computation.

#### Composability Track - $4000

- 1st place - $2,500
- 2nd place - $1,500

Build an innovative application that showcases [LayerZero's horizontal composability](https://docs.layerzero.network/v2/developers/evm/composer/overview) features. Your project should break down a complex cross-chain workflow into discrete, sequential steps managed through LayerZero messages.

Demonstrate how you can trigger follow-up actions (composed messages) on a destination chain after an initial LayerZero message is delivered, potentially involving interactions with multiple contracts or protocols across different chains.

Focus on creating advanced, multi-step workflows that wouldn't be easily possible with traditional bridging or single atomic cross-chain transactions. Show how this approach improves user experience, reliability, or enables new use cases by decoupling operations and leveraging LayerZero's message-passing framework.

#### General Prize Track - $2000

- 1st place - $1,000
- 2nd place - $1,000

For outstanding projects utilizing any LayerZero feature (OApp, OFT, ONFT, lzRead, Composability) to build a compelling omnichain application.

This track rewards creative and well-executed projects that demonstrate the power and potential of LayerZero, even if they don't fit perfectly into the specific `lzRead` or Composability tracks. Show us your best omnichain ideas!

## 📋 Judging Criteria

- **Innovation & Creativity:** How novel is the idea? Does it leverage LayerZero's unique capabilities in interesting ways?
- **Technical Implementation:** Quality of the code, effective use of LayerZero protocols (OApp, OFT, ONFT, lzRead, Composability), smart contract security, and overall technical soundness.
- **Impact & Usefulness:** How valuable is the application? Does it solve a real-world problem or have significant potential?
- **Omnichain Aspect:** How core is LayerZero to the application? Does it solve a real cross-chain problem or enable a truly omnichain experience?
- **User Experience (UX):** How easy and intuitive is the application to use? Does it successfully abstract away cross-chain complexity?
- **Presentation & Demo:** Clarity of the project presentation and effectiveness of the live demo.

## 🔥 Inspiration & Past Winners

Examples of past hackathon projects built with LayerZero:

ETHGlobal Bangkok 2024 - Best Omnichain Solutions
- [ERC20 Unchained](https://ethglobal.com/showcase/erc20-unchained-ziaz1)
- [FlashFi](https://ethglobal.com/showcase/flashfi-g27p4)
- [BOO Market](https://ethglobal.com/showcase/boo-market-oekxo)

ETHGloabal Bangkok 2024 - Best LayerZero Read
- [METAINTENTS](https://ethglobal.com/showcase/metaintents-8kjr4)
- [Solvnet](https://ethglobal.com/showcase/solvnet-rr87n)

ETHGlobal San Francisco 2024 - Most Innovative Omnichain Solution
- [Quark](https://ethglobal.com/showcase/quark-py5p4)
- [LayerKit](https://ethglobal.com/showcase/layerkit-ksqw0)
- [PowerAgents](https://ethglobal.com/showcase/power-agents-djqmb)

ETHGlobal Singapore 2024 - Most Innovative Omnichain Solution
- [JITLiq Network](https://ethglobal.com/showcase/jitliq-network-m2cw1)
- [PageETH](https://ethglobal.com/showcase/pageeth-rcjiz)

ETHOnline 2024 - Most Innovative Omnichain Solution
- [OmniGas](https://ethglobal.com/showcase/omnigas-cqg1m)
- [Membrane Finance](https://ethglobal.com/showcase/membrane-finance-qvq7k)

ETHGlobal Brussels 2024 - Best Omnichain Implementation
- [SyncSafe](https://ethglobal.com/showcase/syncsafe-dcrfk)
- [liqu1tent](https://ethglobal.com/showcase/liqu1tent-5mctm)

## 🧑‍💻 Technical Support & Community

- **Primary Support Channel** - [LayerZero Discord](https://discord.gg/ktbvm8Nkcr) - Start with `#dev-general` channel.
- **LayerZero Team** - Find members of our team at LayerZero table in the hackathon venue. Talk to them about your project, ask questions, get help.
