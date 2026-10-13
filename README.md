## Hey, I'm Ruslan 👋

**Lead Software Engineer & AI Champion** at [EPAM Systems](https://www.epam.com) · **AI Solution Architect** · Lviv 🇺🇦

[![EPAM AI Champion](https://img.shields.io/badge/EPAM-AI%20Champion-00A3E0?style=flat&logo=epam&logoColor=white)](https://leap.epam.com)
[![SAS Graduate](https://img.shields.io/badge/Solution%20Architecture%20School-Graduated%2087%25-059669?style=flat)](https://www.epam.com)
[![EASE Core Architect](https://img.shields.io/badge/EASE%20Agent%20Skills-%231%20Maintainer%20(919%20commits)-7C3AED?style=flat)](https://git.epam.com)
[![App Store Developer](https://img.shields.io/badge/App%20Store-Shipped%20Indie%20Apps-000000?style=flat&logo=apple&logoColor=white)](https://apps.apple.com/us/developer/ruslan-popesku/id1627013326)

10+ years engineering high-scale digital systems — from architecting platforms at **600M+ user scale (Disney+ Hotstar)** to driving **Enterprise AI Adoption** and building **autonomous multi-agent coding factories**.

Currently coordinating the **[Idea-to-Grow Mobile HyperFactory](https://leap.epam.com)** (Team 1566-EPM-AQCC in EPAM AI/RUN Mission 2026), leading the **EASE Agent Skills** platform (#1 core maintainer with 919 commits, 82 production skills), and consulting Tier-1 enterprise clients (**Philip Morris International**) on multi-agent architectures, Model Context Protocol (MCP), and tokenomics. Passionate about shipping indie products with privacy-first on-device AI, maintaining core open-source developer infrastructure, and making autonomous coding agents genuinely deterministic for engineering teams.

---

### 🧠 AI Open Source Contributions (Featured)

Active core contributor to memory architectures, semantic retrieval, and developer infrastructure for autonomous AI coding agents:

#### 🔍 [grepai](https://github.com/yoanbernabeu/grepai)
> **What it is:** 100% local semantic code search and AST call graph engine designed specifically for AI coding agents. Enables agents to navigate, index, and reason about codebases without uploading proprietary source code to cloud APIs.

- **Index Reliability & Recovery:** Built atomic index serialization and automatic recovery mechanisms that restore state when interrupted or corrupted ([PR #269](https://github.com/yoanbernabeu/grepai/pull/269)).
- **Worktree Discovery Controls:** Added configuration options to control linked git worktree discovery, preventing redundant index bloat in multi-branch workflows ([PR #270](https://github.com/yoanbernabeu/grepai/pull/270)).
- **Agent Skill & Search Hardening:** Authored recall-safe hybrid search combos and hardened tool-choice descriptions for agent prompt templates and skills ([PR #272](https://github.com/yoanbernabeu/grepai/pull/272)).

#### 🏛️ [MemPalace](https://github.com/MemPalace/mempalace)
> **What it is:** Open-source long-term memory and context retention system for AI coding agents. Ingests architectural decisions, session history, and project learnings into structured "drawers" using vector retrieval and MCP.

- **Incremental Re-Mining (`sync`):** Built the `sync` command with `content_hash` tracking in drawer metadata, enabling atomic re-mining only for modified files and avoiding expensive full-index sweeps ([PR #1343](https://github.com/MemPalace/mempalace/pull/1343), [PR #1344](https://github.com/MemPalace/mempalace/pull/1344)).
- **Vector Store Corruption Repair:** Engineered safe repair routines surviving ChromaDB HNSW vector index corruption during repair cycles.
- **Claude.ai Export Normalizer:** Added structured conversation normalizer to ingest exported Claude chat logs directly into memory drawers.
- **Hook Decoupling & Context Guard:** Decoupled the `precompact` hook toggle from `save_interval` via config & env flags, fixing context-exhaustion blocks during long agent sessions ([PR #1345](https://github.com/MemPalace/mempalace/pull/1345), [PR #1346](https://github.com/MemPalace/mempalace/pull/1346)).
- **MCP Tooling:** Authored the `mempalace_sync_status` MCP tool and memory freshness hooks ([PR #1347](https://github.com/MemPalace/mempalace/pull/1347)).

---

### 🛠️ Open Source Tooling & Frameworks

Creator and maintainer of open-source tools for iOS engineers & AI agents:

- 🔧 **[ios-agent-skills](https://github.com/rusel95/ios-agent-skills)** — 11 production-tested Agent Skills for Claude Code (`claude plugin add rusel95/ios-agent-skills`), Codex, and 40+ AI tools (`npx skills add rusel95/ios-agent-skills`). Covers SwiftUI MVVM, UIKit MVVM, VIPER, TCA, Swift Concurrency, GCD, Testing, Security Audit, Accessibility, and Localization. Benchmarked across 260+ scenarios with 850+ discriminating assertions. The exact engineering foundation used to ship my own apps!
- 🚀 **[ios-aso-copilot](https://github.com/rusel95/ios-aso-copilot)** — Free, open-source agent-native ASO engine. Features live Apple Search Hints (`MZSearchHints.woa`), multi-market rank tracking across 25+ storefronts, 21-day hypothesis ledgers, anti-regression guards, and Apple Search Ads break-even unit economics. Battle-tested across 77+ live hypotheses on Compresso and Hush.
- 🧪 **[Offline-AI-ML-Playground](https://github.com/rusel95/Offline-AI-ML-Playground)** — On-device SwiftUI testbed for running and evaluating open-source ML/LLM models locally on Apple platforms via MLX Swift with zero network dependency.

---

### 📱 Shipped Indie Products

Building and operating consumer iOS products on the App Store with privacy-by-design (zero cloud telemetry, 100% on-device compute):

- **[Compresso: Shrink Video Photo](https://apps.apple.com/us/app/compresso-shrink-video-photo/id6790447224)** — Privacy-first, 100% on-device photo & video compression (HEIC/HEVC) for iPhone with month-by-month swipe cleanup, zero cloud telemetry, and 34+ localized languages. Built using [ios-agent-skills](https://github.com/rusel95/ios-agent-skills) and grown with [ios-aso-copilot](https://github.com/rusel95/ios-aso-copilot).
- **[Hush: White Noise & Sleep Aid](https://apps.apple.com/us/app/hush-white-noise-sleep-aid/id6449785515)** — Focused ambient sound mixer with 30+ layered audio loops, background playback, lock-screen controls, smart fade-out timer, and 49 localized languages.
- 🍎 *Explore all releases on my [Apple Developer Profile](https://apps.apple.com/us/developer/ruslan-popesku/id1627013326).*

---

### 🧪 Swift & Testing Open Source Contributions

- 🧪 **[agent-swift-XCTest](https://github.com/reportportal/agent-swift-XCTest)** *(Core Contributor & Maintainer)* — Official Swift XCTest agent for [ReportPortal.io](https://reportportal.io). Modernized architecture with `async/await` over ReportPortal v2 API, multi-process parallel worker launch merging (`RP_LAUNCH_UUID` / Info.plist), launch-gate synchronization, and real-device cloud farm (SauceLabs) orchestration. Cut test execution time by 75% (6.0h to 1.5h).
- 🎬 **[MediaToolSwift](https://github.com/starkdmi/MediaToolSwift)** *(Contributor)* — Merged upstream [PR #13](https://github.com/starkdmi/MediaToolSwift/pull/13) fixing native iOS `AVAssetWriterInput` rejection of DCI-P3 wide-gamut video transcoding. Implemented single-encode AVFoundation compositor conversion to P3-D65 SDR (BT.709) and BT.2020 HDR (10-bit HLG/PQ) with orientation handling and comprehensive 83-test verification suite.

---

### 💼 Engineering Leadership & Experience

- **EPAM Systems** *(2021 — present)* · **Lead Software Engineer & AI Champion · Solution Architect**
  - **Idea-to-Grow Mobile HyperFactory:** Contact Point & Lead Coordinator for Team `1566-EPM-AQCC` in the flagship **EPAM AI/RUN Mission 2026** programme. Packaged end-to-end agentic workflows from idea validation to App Store release (50 locales) and ASO/ASA growth loops; increased commit velocity 4x (~50 to 200+/mo) with 100% crash-free stability.
  - **KIRO AI Adoption Expert (Consultant):** Direct enterprise AI adoption, multi-agent workflows, Model Context Protocol (MCP) tool integration, and tokenomics consulting for Philip Morris International (`PMIS-DRS`).
  - **EPAM EASE Agent Skills:** Founder & #1 Maintainer (919 commits) of the enterprise agent skill standard (`git.epam.com/epm-ease/research/agent-skills`), benchmarked across 150M+ tokens with +30% verified correctness improvement.
  - **Disney+ Hotstar:** Technical Team Lead on a 600M+ user streaming platform with 200+ engineers; led feature delivery with 75% unit-test and 100% UI automation coverage.
  - **Thomson Reuters:** Senior iOS Engineer on a flagship news product serving 2M+ active users.
  - **Planoly:** Senior iOS Engineer on social media planning product with 50K+ subscribers.
  - **Technical Evangelism & Talks:** 4 flagship masterclasses on EPAM VideoPortal (Spec-Driven Dev, Agent Skills, AWS DevOps Agent, AWS Security Agent); broadcast to 35+ global communities on We Are Community (177 badges).
- **Nullgravity** *(2019 — 2021)* · iOS Engineer
  - Shipped AR retail experience; reduced legacy clean build time by 60% (~20 min saved per developer daily).
- **Yalantis** *(2018 — 2019)* · iOS Engineer
  - Delivered commercial retail & social apps with complex third-party hardware/BLE and service integrations.

---

### 💻 Tech Stack & Craft

`Swift` · `SwiftUI` · `UIKit` · `Combine` · `Swift Concurrency` · `AVFoundation` · `TCA` · `VIPER` · `XCTest` · `Swift Testing` · `ReportPortal` · `MLX Swift` · `Python` · `ChromaDB` · `MCP (Model Context Protocol)` · `Context Engineering`

---

### 📫 Connect

[![App Store](https://img.shields.io/badge/App_Store-Developer_Page-black?style=flat&logo=apple&logoColor=white)](https://apps.apple.com/us/developer/ruslan-popesku/id1627013326)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rusel95)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/rusel95)
[![Website](https://img.shields.io/badge/Portfolio-rusel95.github.io-blue?style=flat)](https://rusel95.github.io)
[![Email](https://img.shields.io/badge/Email-ruslanpopesku95@gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:ruslanpopesku95@gmail.com)
