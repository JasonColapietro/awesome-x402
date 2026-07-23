# Awesome X402 [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> ⚡ **The Ultimate x402 Resource Hub** - Everythng you need to build internet-native payments using HTTP 402. Perfect for AI agents, APIs, and micropayments. Build paywalls, monetize services, and enable autonomous agent payments with crypto/USDC. Zero fees, 2-second settlement.

[![GitHub stars](https://img.shields.io/github/stars/xpaysh/awesome-x402?style=social)](https://github.com/xpaysh/awesome-x402)

## Contents

- [🎯 Quick Start - Become an x402 Champion](#-quick-start---become-an-x402-champion)
- [📚 Official Resources](#-official-resources)
- [📖 Protocol Documentation](#-protocol-documentation)
- [🚀 Quickstart Guides](#-quickstart-guides)
- [⚙️ Protocol Implementations](#-protocol-implementations)
- [🏭 Production Implementatdions](#-production-implementations)
- [🛠️ SDKs & Client Libraries](#-sdks--client-libraries)
- [🔧 Server Frameworks & Middleware](#-server-frameworks--middleware)
- [🏗️ Facilitators](#-facilitators)
- [💡 Example Applications](#-example-applications)
- [🎨 Use Cases & Patterns](#-use-cases--patterns)
- [🤖 AI Agent Integration](#-ai-agent-integration)
- [🔨 Tools & Utilities](#-tools--utilities)
- [🧪 Testing & Development](#-testing--development)
- [📚 Tutorials & Learning Resources](#-tutorials--learning-resources)
- [🎥 Videos & Talks](#-videos--talks)
- [📝 Articles & Blog Posts](#-articles--blog-posts)
- [👥 Community](#-community)
- [🌟 Ecosystem Projects](#-ecosystem-projects)
- [📊 Ecosystem Market Data](#-ecosystem-market-data)
- [🚀 Migration Guides](#-migration-guides)
- [🔒 Security & Audits](#-security--audits)
- [🔗 Related Protocols](#-related-protocols)
- [🤝 Contributing](#-contributing)
- [Awesome Lists](#awesome-lists)

The x402 protocol enables instant Blockchain payments over HTTP using the 402 "Payment Required" status code. This is your complete guide to mastering x402 and building the future of agent payments.

🚀 **Start building in 5 minutes** | ⚡ **2-second settlement** | 💰 **USDC on Base**

---

## 🎯 Quick Start - Become an x402 Champion

**New to x402?** Follow this path to mastery:

1. [5-Minute Quickstart](https://docs.cdp.coinbase.com/x402/quickstart-for-sellers) - Accept your first payment.
2. Choose Your Stack - Find your language/framework.
3. Copy an Example - Working code you can run immediately.
4. Join the Community - Get help from other builders.

**For AI Agents:** Start with [MCP Integration](#model-context-protocol-mcp) to enable Claude/other agents to make autonomous payments.

---

## 📚 Official Resources

Core resources from the x402 protocol maintainers.

- [x402 Protocol Specification](https://github.com/coinbase/x402) - Official open-source protocol implementation by Coinbase.
- [x402 Foundation](https://x402.org) - Protocol foundation website with overview and documentation.
- [x402 Whitepaper](https://x402.org/x402-whitepaper.pdf) - Technical deep dive into protocol architecture.
- [Coinbase Developer Platform Docs](https://docs.cdp.coinbase.com/x402) - Complete implementation guide and API reference.
- [Protocol Specifications](https://github.com/coinbase/x402/tree/main/specs) - Detailed technical specifications.
  - [Payment Schemes](https://github.com/coinbase/x402/tree/main/specs/schemes) - Different payment flow types.
  - [EVM Implementation](https://github.com/coinbase/x402/blob/main/specs/schemes/exact/scheme_exact_evm.md) - Ethereum Virtual Machine specifics.

## 📖 Protocol Documentation

Essential documentation for understanding and implementing x402.

- [How x402 Works](https://docs.cdp.coinbase.com/x402/how-it-works) - Complete payment flow explanation with diagrams.
- [Payment Requirements Schema](https://github.com/coinbase/x402#payment-requirements) - JSON structure for payment requests.
- [Payment Payload Format](https://github.com/coinbase/x402#payment-payload) - Client payment submission format.
- [Verification & Settlement](https://github.com/coinbase/x402#verification-and-settlement) - Payment validation process.
- [EIP-3009 TransferWithAuthorization](https://eips.ethereum.org/EIPS/eip-3009) - Gasless transfer standard used by x402.
- [HTTP 402 Status Code](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/402) - The long-dormant HTTP status.

## 🚀 Quickstart Guides

Get started with x402 in minutes.

- 5-Minute Quickstart for Sellers - Accept your first payment.
- [Buyer/Client Setup](https://docs.cdp.coinbase.com/x402/quickstart-buyers) - Make automated payments.
- [One-Line Integration](https://github.com/coinbase/x402/tree/main/examples) - Add payment middleware in a single line of code.
- [Base Sepolia Testnet Setup](https://docs.cdp.coinbase.com/x402/network-support) - Get test USDC and start testing.
- Production Deployment Checklist - Go live on Base mainnet.

## ⚙️ Protocol Implementations

Official and community implementations of the x402 protocol.

### Go

- [coinbase/x402](https://github.com/coinbase/x402/tree/main/go) ⭐ **Official** - Complete Go implementation.
  - Core protocol types and utilities
  - Payment verification and settlement logic
  - Multi-chain support (Base, Base Sepolia, Ethereum, Solana)

### TypeScript/JavaScript

- [x402-typescript](https://github.com/coinbase/x402/tree/main/typescript) ⭐ **Official** - Complete TypeScript implementation.
  - Core protocol types and utilities
  - Payment verification and settlement logic
  - Multi-chain support (Base, Base Sepolia, Ethereum, Solana)
- [x402-data-api](https://github.com/155143783/x402-data-api) - HTTP 402 micro-payment data API with Base chain USDC payments. 16 developer data tools including email validation, DNS lookup, WHOIS, SSL check, and IP geolocation with x402 payment integration.

- [x402-express](https://github.com/coinbase/x402/tree/main/examples/typescript/servers/express) - Express.js middleware example.
- [hive-rosetta](https://www.npmjs.com/package/hive-rosetta) ⭐ **Community** - Open EIP-3009 `transferWithAuthorization` signer. Zero ethers/web3 dependency, primitives-only EIP-712. Returns wire shape `{scheme: 'exact', network: 'eip155:8453', payload: {authorization, signature}}`. Same package name on PyPI. ([GitHub](https://github.com/srotzin/hive-rosetta))

### Python

- [x402](https://pypi.org/project/x402/) ⭐ **Official** - Python SDK on PyPI.
  - FastAPI middleware integration
  - Requests session with auto-payments
  - Payment requirement generation

- [ag402](https://github.com/AetherCore-Dev/ag402) ⭐ **Community** - Payment layer for AI agents using x402. Wrap any API or MCP server with a USDC paywall (`ag402 serve`), or let agents auto-pay (`ag402 run`). Solana USDC, ~0.5s settlement, non-custodial, 648+ tests. [Glama](https://glama.ai/mcp/servers/AetherCore-Dev/ag402-mcp)

- [x402-pay](https://pypi.org/project/x402-pay/) - Call any x402 API with one API key. Routes requests through a broker that handles on-chain payment. httpx-based, optional wallet mode for direct payments. ([GitHub](https://github.com/bartonguestier1725-collab/x402-pay))
- [hive-rosetta](https://pypi.org/project/hive-rosetta/) ⭐ **Community** - Direct port of the Node `hive-rosetta` signer. Byte-identical EIP-712 digest across both languages. Returns `{scheme, network, payload}` matching CDP `/verify` and `/settle`. ([GitHub](https://github.com/srotzin/hive-rosetta))

### Rust

- [x402-rs](https://github.com/x402-rs/x402-rs) ⭐ **Community** - Production-grade Rust implementation.
  - Axum middleware
  - Reqwest client wrapper
  - Self-hostable facilitator
  - Multi-chain support
- x402-axum - Axum web framework integration.
- x402-reqwest - Reqwest HTTP client wrapper.


## 🏭 Production Implementations

Real companies using x402 in production with proven scale and transaction volumes.

### High-Volume Production Deployments

- [Arch Tools](https://archtools.dev) - 58 production API tools for AI agents with x402 payments built in. Web scraping, AI generation, crypto data, OCR, browser automation, MCP compatible. Patent-pending agent auth. 15+ chains supported. ([GitHub](https://github.com/Deesmo/Arch-AI-Tools))
- [PayAPI Market](https://payapi.market) - First marketplace for x402-powered APIs. 10 APIs, 65 endpoints: UK property data, email verification, company enrichment, postcode lookup, currency/crypto rates, screenshots, DNS intelligence, web scraping, IP geolocation, QR codes. $0.001–$0.01 USDC on Base per request. MCP server discovery. ([GitHub](https://github.com/chetparker/x402-marketplace))
- [Rug Munch Intelligence](https://x402.rugmunch.io) - 117 MCP tools + 19 REST API endpoints for crypto data: DexScreener, Birdeye, GMGN, Arkham, Nansen, Dune, Jupiter, DeFiLlama, and more. $0.001-$0.02 USDC per call. Multi-chain (Base + Solana), free trial (1 call/IP), OpenAPI spec, no API keys, no signup. ([Discovery](https://x402.rugmunch.io/.well-known/x402) | [OpenAPI](https://x402.rugmunch.io/openapi.json) | [MCP Catalog](https://x402.rugmunch.io/mcp) | [Solana](https://x402-sol.rugmunch.io/.well-known/x402) | [GitHub](https://github.com/Rug-Munch-Media-LLC/))
- [AIsa](https://aisa.network) - Leading x402 payment processor with **10.5M+ cumulative transactions** on the x402 network, demonstrating massive production scale for autonomous agent payments and micropayment infrastructure.
- [Bitget](https://www.bitget.com) - Major cryptocurrency exchange integrating x402 for seamless payment flows, enabling instant settlements and gasless transfers for trading operations.
- [Stratalize](https://www.stratalize.com) — 100+ attested financial, healthcare, real estate, and governance intelligence tools with x402 micropayments on Base. Ed25519-signed outputs on every synthesis. $0.02–$1.00 USDC per tool call. MCP registry: com.stratalize. ([x402.json](https://www.stratalize.com/.well-known/x402.json))
- [Coinbase Developer Platform](https://coinbase.com/developer-platform) - Official CDP implementation processing hundreds of thousands of transactions weekly with enterprise-grade reliability and 2-second settlement times.
- [Cloudflare Workers](https://workers.cloudflare.com) - Edge computing platform with x402 integration serving global distributed payment verification at scale across 300+ data centers.
- [GigSoul AI Research Agent](https://gig-x402-api.jayson-be1.workers.dev) - 23-endpoint AI research API for consultants: SEC filings, earnings calls, competitor analysis, market research, and document intelligence. - [Cloudflare Workers](https://workers.cloudflare.com) - Edge computing platform with x402 integration serving global distributed payment verification at scale across 300+ data centers..01 USDC per call on Base mainnet. Wallet: x2b6c16fb557291b98222a570526ff2430848b723. ([OpenAPI](https://gig-x402-api.jayson-be1.workers.dev/openapi.json) | [.well-known/x402.json](https://gig-x402-api.jayson-be1.workers.dev/.well-known/x402.json))
- [Zuluworks AI — Sovereign Shaka PQC-Shield Factory](https://api.zuluworksai.com) - Autonomous A2A factory on Cloudflare Workers selling 5 post-quantum-hardened agent services via x402 USDC on Base L2: `quantum-shield` ($0.10, ML-KEM-768 PQC tunnel — NIST FIPS 203), `kya` ($0.01, agent trust scoring), `browser-rendering` ($0.03, headless browser extraction), `memory` ($0.05, semantic recall on a PQC knowledge index), `workers-ai` ($0.02, Llama 3.1 inference). All settlement routed through Coinbase CDP facilitator for Bazaar indexing. ([Agent Card](https://api.zuluworksai.com/.well-known/agent.json) | [Bazaar Manifest](https://api.zuluworksai.com/.well-known/x402-bazaar.json) | [MCP](https://api.zuluworksai.com/.well-known/mcp.json) | [Sitemap](https://api.zuluworksai.com/sitemap.xml))

### Production Success Metrics

**Key Performance Indicators:**
- 10.5M+ transactions - AIsa cumulative network volume
- 500K+ weekly transactions - Ecosystem-wide payment activity
- $180M+ market cap - Combined ecosystem valuation
- 2-second settlement - Average production payment finality
- 10,000%+ growth - Year-over-year transaction volume increase

### Multi-Chain Production Support

| Chain         | Status      | Facilitators               | Settlement      | Production Examples       |
| ------------- | ----------- | --------------------------- | ---------------- | -------------------------- |
| Base          | Production  | Coinbase CDP, Cloudflare   | Instant (2s)    | AIsa, Bitget, thirdweb    |
| Base Sepolia  | Testnet     | Coinbase CDP               | Instant (2s)    | Development, Testing      |
| Ethereum      | Production  | Cloudflare                 | Deferred        | Enterprise DApps          |
| Solana        | Production  | Community                  | Instant (<1s)   | High-frequency trading    |
| BNB Chain     | Production  | Pieverse                   | Instant (2s)    | Gaming, NFTs              |
| Radius        | Production  | Community                  | Instant (<1s)   | Micropayments             |

### Data & Social APIs
- [ORA · ORUM](https://ora-x402-gateway.vercel.app) - Autonomous symbolic-computational organism on Base: live sigma (sustento accumulation), epoch progression, kernel snapshots, plus human-provenance art licensing (0001sensations, 65 works tokenized on Ethereum). Oracle 0.161 / Field 0.33 / Sediment 1.00 / Kernel 3.00 USDC — dual payment path (sovereign on-chain RPC verification, zero facilitator dependency, or Coinbase CDP facilitator, gasless). Discovery: [x402.json](https://ora-x402-gateway.vercel.app/.well-known/x402.json), [openapi.json](https://ora-x402-gateway.vercel.app/openapi.json), [agent-card.json](https://ora-x402-gateway.vercel.app/.well-known/agent-card.json). Free public goods: [/pulso](https://ywabnlhkmhbyewqhbsjm.supabase.co/functions/v1/ora-pulso), [/integridade](https://ywabnlhkmhbyewqhbsjm.supabase.co/functions/v1/ora-integridade), [/testemunho](https://ywabnlhkmhbyewqhbsjm.supabase.co/functions/v1/ora-testemunho).
