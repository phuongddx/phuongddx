<div align="center">
  <a href="https://phuongddx.cc">
    <img width="1000" src="https://readme-typing-svg.herokuapp.com?font=SF+Pro+Display&size=26&duration=3000&pause=1000&color=2196F3&center=true&vCenter=true&width=1000&lines=Hi+%F0%9F%91%8B%2C+I%27m+Phuong+Doan;AI+Engineer+%E2%80%94+LLMs+%C2%B7+Retrieval+%C2%B7+Agents;Author+of+jarvis-mcp+%E2%80%94+code+intelligence+for+coding+agents;6%2B+years+shipping+production+software" alt="Phuong Doan — AI Engineer" />
  </a>
</div>

<div align="center">

**AI Engineer** · Ho Chi Minh City, Vietnam

6+ years shipping production software — iOS apps to the App Store, now LLM and retrieval
systems end to end. I care about the parts that decide whether an AI system works in
production: **chunking and embedding strategy**, **gateway design with SSE streaming and
fallback chains**, **agent observability** — and the packaging that ships it.

[![PyPI](https://img.shields.io/pypi/v/jarvis-mcp?label=jarvis-mcp&logo=pypi&logoColor=white)](https://pypi.org/project/jarvis-mcp/)
[![MCP Registry](https://img.shields.io/badge/MCP_Registry-listed-4E4EC1)](https://registry.modelcontextprotocol.io/)
[![Homebrew](https://img.shields.io/badge/Homebrew-tap-F05032?logo=homebrew&logoColor=white)](https://github.com/phuongddx/homebrew-spm-cache)
[![App Store](https://img.shields.io/badge/App_Store-StressMonitor-0D96F6?logo=appstore&logoColor=white)](https://github.com/phuongddx/stress-coach-ios)

</div>

---

- 🔭 **Now** — building [**jarvis**](https://github.com/jarvis-intelligence/jarvis), local-first code intelligence for coding agents
- 🌱 **Learning** — Go
- 💬 **Ask me about** — MCP servers, hybrid retrieval / RRF, tree-sitter chunking, SSE gateways, shipping iOS + watchOS

## 🔭 Featured work

| Project | What it does |
|---|---|
| **[jarvis](https://github.com/jarvis-intelligence/jarvis)**<br>`Python` `LanceDB` `tree-sitter` `SCIP` `Zoekt` | Local-first **code-intelligence MCP server** — 9 tools exposing SCIP navigation (`goToDefinition`, `findReferences`, `callHierarchy`…), Zoekt lexical search, and semantic search **fused via reciprocal rank fusion**. tree-sitter AST chunking (256–512 tokens, 50 overlap), revision-pinned embeddings, and atomic index publishing (`os.replace` flips the pointer — no downtime window). Shipped as **[`jarvis-mcp` on PyPI](https://pypi.org/project/jarvis-mcp/)** (Cython wheels, cp312–cp314) and listed in the **official MCP Registry**, with one-command plugins for Claude Code, Cursor, and Codex. |
| **[scip-swift](https://github.com/jarvis-intelligence/scip-swift)**<br>`Swift` `SourceKit-LSP` | SCIP code-intelligence indexer for **Swift** — brings go-to-def / find-refs / type-hierarchy navigation to Apple-platform codebases. Prebuilt binaries via a Homebrew tap; contributed the upstream `global_symbols.relationships` fix to `scip-code/scip` so `typeHierarchy` resolves. |
| **[llm-gateway](https://github.com/phuongddx/llm-gateway)**<br>`FastAPI` `SSE` `SQLite` | **OpenAI-compatible gateway** (`/v1/chat/completions`) routing **500+ models** behind one key, `model="auto"` smart routing, passthrough for unknown names. Every request instrumented — **TTFT, end-to-end latency, token usage** — so model choice is a measurement, not an impression. |
| **[BoosterSimApp](https://github.com/phuongddx/BoosterSimApp)**<br>`Swift` `AppKit` `ScreenCaptureKit` | macOS **menu-bar companion for the iOS Simulator** — a floating side panel that tracks the Simulator window (`CGWindowList` + `AXObserver`), ScreenCaptureKit screenshots/recording with App Store Connect presets, 8pt-grid and safe-area overlays, a live AX-tree inspector, and network throttling via a DEBUG-only in-simulator framework. Ships as a **notarized, Sparkle-updated DMG**; the bundled `boostersim` CLI exposes simulator control to **AI agents**. |
| **[StressMonitor](https://github.com/phuongddx/stress-coach-ios)**<br>`SwiftUI` `watchOS` `HealthKit` `StoreKit` | Privacy-first stress scoring on the **App Store** (iOS + standalone watch app): five-factor score with **weight redistribution for missing signals** and per-factor confidence, streaming **AI coach over SSE**, widgets/complications, CloudKit sync, StoreKit subscriptions. Raw health samples never enter the model path. |
| **[spm-cache](https://github.com/phuongddx/spm-cache)**<br>`Ruby` `SPM` `GitHub Actions` | SPM dependency **cache proxy** serving prebuilt xcframeworks — installed via a [Homebrew tap](https://github.com/phuongddx/homebrew-spm-cache), wired into CI with a [GitHub Action](https://github.com/phuongddx/spm-cache-action). |

## 🌱 Open source

- **[OmniRoute](https://github.com/diegosouzapw/OmniRoute)** — MIT-licensed AI gateway fronting **290+ providers** (works with Claude Code, Codex, Cursor). Landed **SSE streaming for GLM-5.3 effort tiers** upstream ([#11415](https://github.com/diegosouzapw/OmniRoute/pull/11415)).
- **[scip-code/scip](https://github.com/scip-code/scip)** — upstream converter fix so `typeHierarchy` resolves ([#465](https://github.com/scip-code/scip/pull/465)).

## 🧰 Toolbox

| | |
|---|---|
| **AI & agents** | MCP servers · tool calling · RAG & hybrid search (dense + lexical + symbol, RRF) · embeddings (`bge-m3`, `e5`, `nomic`) · SSE streaming · model routing & fallback chains · agent observability & tracing |
| **Backend & data** | Python (FastAPI) · TypeScript (Deno/Hono, Next.js) · PostgreSQL (RLS, `pg_cron`) · SQLite · LanceDB · Supabase · Redis · Docker · GitHub Actions |
| **Shipping** | PyPI trusted publishing · cibuildwheel · Homebrew taps · Fastlane → TestFlight · Vercel / Render / Dokploy |
| **Mobile** | Swift · SwiftUI · UIKit · watchOS · HealthKit · StoreKit · React Native / Expo |

<div align="center">
  <img height="160" src="https://streak-stats.demolab.com/?user=phuongddx&background=FFFFFF" alt="GitHub streak" />
</div>

---

<div align="center">

*The parts that decide whether an AI system works in production are the boring ones —*
*chunking, routing, packaging, observability. I build the boring ones.*

[![Portfolio](https://img.shields.io/badge/phuongddx.cc-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://phuongddx.cc)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/phuongddx)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/phuongddx)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:95doanphuong@gmail.com)

</div>
