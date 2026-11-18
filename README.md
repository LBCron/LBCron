# Ronan Chen-Lopes (`@LBCron`)

**Senior Systems, Protocol, Full-Stack & AI Infrastructure Engineer**  
`Rust` · `TypeScript` · `Python` · `Scala` · `Solidity (Foundry)` · `Solana` · `React / React Native` · `Next.js`

[![Hire Me on Upwork](https://img.shields.io/badge/Hire_Me_on_Upwork-Ronan_Chen--Lopes-14a800?style=for-the-badge&logo=upwork&logoColor=white)](https://www.upwork.com/freelancers/~0131dae36abcf59374)
[![Contact Email](https://img.shields.io/badge/Email-ronan.chenlopes%40gmail.com-0A66C2?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ronan.chenlopes@gmail.com)

📍 Grenoble / Lyon Region, France (CET / UTC+1) · 💼 **Direct Upwork Profile:** **[upwork.com/freelancers/~0131dae36abcf59374](https://www.upwork.com/freelancers/~0131dae36abcf59374)**

---

### Executive Engineering Summary

I partner with engineering teams, founders, and protocol maintainers to resolve high-stakes production defects, ship deterministic distributed systems, audit smart contracts before mainnet deployment, and build bounded AI agent & data infrastructure. Every engagement follows a strict engineering standard: **deterministic failing test reproduction first, minimal root-cause architecture, and regression-tested Pull Requests.**

---

### 1. L1 Consensus, Distributed Protocols & Web3 Security (`Rust` · `Scala` · `Solana` · `Solidity`)

- **[`tari-project/tari-ootle`](https://github.com/tari-project/tari-ootle)** *(Rust — Layer-2 Consensus & Execution Engine)*
  - **Merged Upstream PRs:**
    - **[`#3543`](https://github.com/tari-project/tari-ootle/pull/3543)** *(Merged)* — Engine execution security: reject zero-amount fee payments and enforce intrinsic argument arity.
    - **[`#3548`](https://github.com/tari-project/tari-ootle/pull/3548)** *(Merged)* — Epoch oracle determinism: defer `ConfiguredCurrentEpoch` persistence, validate global/max-epoch validator bounds, and prevent duplicate `HybridEpochOracle` transitions.
    - **[`#3535`](https://github.com/tari-project/tari-ootle/pull/3535)** *(Merged)* — Consensus safety: report local aborts on `AllAccept` disagreement and validate foreign proposal atoms.
- **[`ergoplatform/ergo`](https://github.com/ergoplatform/ergo) & [`ergoplatform/ergoscript-by-example`](https://github.com/ergoplatform/ergoscript-by-example)** *(Scala & ErgoScript — Layer-1 Node & UTXO Contracts)*
  - **Node & Protocol Engineering:** Maintainer-reviewed protocol PRs **[`ergo#2924`](https://github.com/ergoplatform/ergo/pull/2924)** (lazy incomplete fork-switch deferral in `FullBlockProcessor`), **[`ergo#2928`](https://github.com/ergoplatform/ergo/pull/2928)** (skipping redundant script execution in `CleanupWorker` for context-free transactions), and **[`ergo#2929`](https://github.com/ergoplatform/ergo/pull/2929)** (full UTXO set scan implementation), plus co-authored `v6.0.11` protocol work (**[`ergo#2847`](https://github.com/ergoplatform/ergo/pull/2847)**).
  - **Smart Contract Reference:** **[`ergoscript-by-example#24`](https://github.com/ergoplatform/ergoscript-by-example/pull/24)** — Decentralized EIP-0024 Artist Royalty NFT Sale Contract & interactive playground walkthrough.
- **[`LBCron/solroute-mandate`](https://github.com/LBCron/solroute-mandate) & [`LBCron/reactive-omni-aegis`](https://github.com/LBCron/reactive-omni-aegis)** *(Solana & EVM Programmable Treasury / Security)*
  - **`solroute-mandate`:** Non-custodial Solana (`SOL` / `USDC` / `USDG` / `Token-2022`) programmable multi-hop routing vault, enforceable spending-mandate policy kernel, client-side `VersionedTransaction (v0)` partial signer, HMAC-SHA256 webhook router, and JSON-RPC 2.0 MCP server.
  - **`reactive-omni-aegis`:** Solidity `0.8.24` Foundry-tested cross-chain DeFi liquidation & threat-mitigation suite with deterministic exploit/invariant test coverage.

---

### 2. AI Agents, Cloud Data Pipelines & Python Backends (`Python` · `FastAPI` · `MCP` · `Cloud`)

- **[`openminion/openminion`](https://github.com/openminion/openminion)** *(Python — Multi-Agent Runtime & Tool Execution SDK)*
  - **Merged Upstream Releases (`v0.1.20`):** **[`#704`](https://github.com/openminion/openminion/pull/704)** *(Merged — resolve `@tool`-decorated callables in subagent allowlists)* and **[`#706`](https://github.com/openminion/openminion/pull/706)** *(Merged — enforce turn-scoped memory write guards)*.
  - **Active Production Hardening PRs:** **[`#798`](https://github.com/openminion/openminion/pull/798)** *(reject missing or malformed Kubernetes `exec` exit status in container tools)* and **[`#799`](https://github.com/openminion/openminion/pull/799)** *(reject malformed pending RPC nonces during transaction prepare/broadcast)*.
- **[`mozilla-ai/otari`](https://github.com/mozilla-ai/otari) & [`LBCron/otari-finops-guard`](https://github.com/LBCron/otari-finops-guard)** *(Python — LLM Gateway & Token FinOps)*
  - Authored **[`mozilla-ai/otari#3006`](https://github.com/mozilla-ai/otari/pull/3006)** *(Merged in `v0.41.0`)* fixing service-key `external_id` budget attribution, alongside per-task virtual-key spend caps and 75%-watermark model routing.
- **Cloud Extraction & Systems Daemons:**
  - **Live Apify Cloud Actor:** Deployed serverless extraction & automation workflow on Apify Cloud (**[console.apify.com/actors/d7Ep4qlEVdozlinyq](https://console.apify.com/actors/d7Ep4qlEVdozlinyq)**).
  - **[`LBCron/whisperflow`](https://github.com/LBCron/whisperflow):** Low-latency Linux CUDA / PipeWire (`48kHz → 16kHz`) audio resampling & local `float16` speech-to-code IPC daemon.

---

### 3. TypeScript, React / React Native & Compiler / EDA Tooling

- **[`tscircuit`](https://github.com/tscircuit) Ecosystem** *(TypeScript — Electronic Design Automation, 3D/SVG Renderers & Constraint Routers)*
  - **[`tscircuit/core`](https://github.com/tscircuit/core):** Capacitance parser & unit validation (**[`#5708`](https://github.com/tscircuit/core/pull/5708)**), supplier LED pin-1 polarity resolution (**[`#5598`](https://github.com/tscircuit/core/pull/5598)**), and multi-phase fanout bus-lane routing (**[`#5284`](https://github.com/tscircuit/core/pull/5284)**).
  - **[`tscircuit/cli`](https://github.com/tscircuit/cli):** Pure Node.js `.tsx` circuit execution without Bun (**[`#5868`](https://github.com/tscircuit/cli/pull/5868)**) and `tsci check all` JSON/SARIF preflight diagnostics (**[`#5741`](https://github.com/tscircuit/cli/pull/5741)**).
  - **[`tscircuit/circuit-json-to-gltf`](https://github.com/tscircuit/circuit-json-to-gltf):** Embedded GLB/glTF `baseColorTexture` and UV coordinate preservation (**[`#303`](https://github.com/tscircuit/circuit-json-to-gltf/pull/303)**).
  - **[`tscircuit/circuit-to-svg`](https://github.com/tscircuit/circuit-to-svg):** Assembly pin-1 orientation accuracy (**[`#956`](https://github.com/tscircuit/circuit-to-svg/pull/956)**) and non-finite SVG coordinate guards (**[`#939`](https://github.com/tscircuit/circuit-to-svg/pull/939)**).
  - **[`tscircuit/tscircuit-autorouter`](https://github.com/tscircuit/tscircuit-autorouter):** Strict `minTraceToPadEdgeClearance` enforcement (**[`#3959`](https://github.com/tscircuit/tscircuit-autorouter/pull/3959)**) and bounded topology-merging / differential-pair validation (**[`#3605`](https://github.com/tscircuit/tscircuit-autorouter/pull/3605)**).
- **Published Open-Source Libraries & Cross-Stack Patches:**
  - **[`LBCron/react-touch-primitives`](https://github.com/LBCron/react-touch-primitives):** Zero-dependency React 18/19 & mobile touch physics hooks (`usePullToRefresh`, `useSwipeGesture`) and WCAG 2.2 / WAI-ARIA `BottomNavigation`.
  - **[`LBCron/apex-quant-dsl`](https://github.com/LBCron/apex-quant-dsl):** Zero-dependency TypeScript recursive-descent AST compiler and vectorized time-series indicator engine (`SMA`, `EMA`, `RSI`, `MACD`, `BBands`, `ATR`, `Sharpe`, `Z-Score`).
  - **Additional Upstream Systems Work:** **[`commaai/opendbc#3928`](https://github.com/commaai/opendbc/pull/3928)** *(16-bit one's-complement rolling checksum carry preservation in CAN/DBC)* · **[`paraspell/xcm-tools`](https://github.com/paraspell/xcm-tools)** *(Polkadot XCM existential-deposit fee verification)* · **[`onyx-dot-app/onyx`](https://github.com/onyx-dot-app/onyx)** *(PostgreSQL / Alembic migrations & OAuth connector state)*.

---

### Core Technical Stack & Consulting Scope

| Domain | Technologies & Deliverables |
| :--- | :--- |
| **Systems & Protocols** | `Rust (tokio, axum, PyO3)` · `Scala` · `C++` · `Linux / Docker` · `GitHub Actions Multi-Arch CI` |
| **Smart Contracts & Web3** | `Solidity (Foundry / forge test)` · `Solana (Anchor, SPL, Token-2022, VersionedTx v0)` · `Polkadot XCM` · `ErgoScript` |
| **AI Agents & Data Infra** | `Python 3.11+` · `FastAPI` · `Pydantic v2` · `Model Context Protocol (MCP)` · `Playwright` · `Apify Actors` · `LLM FinOps` |
| **Full-Stack & Mobile** | `TypeScript` · `Next.js 14/15` · `React 19` · `React Native / Expo` · `PostgreSQL / Supabase RLS` · `Stripe Webhooks` |

[![Work With Me on Upwork](https://img.shields.io/badge/Work_With_Me_on_Upwork-%3C24h_Turnaround_Available-14a800?style=for-the-badge&logo=upwork&logoColor=white)](https://www.upwork.com/freelancers/~0131dae36abcf59374)
