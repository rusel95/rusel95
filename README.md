## Hey, I'm Ruslan 👋

Lead iOS Engineer at [EPAM](https://www.epam.com) · Lviv 🇺🇦

10 years building iOS apps — from UIKit & Objective-C to SwiftUI & Swift Concurrency. Focused on shipping indie products, contributing to open-source AI tooling & developer infrastructure, and making autonomous coding agents reliable for engineers.

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

---

### 📱 Shipped Indie Products

Building and operating consumer iOS products on the App Store:

- **[Compresso: Shrink Video Photo](https://apps.apple.com/us/app/compresso-shrink-video-photo/id6790447224)** — Privacy-first, 100% on-device photo & video compression (HEIC/HEVC) for iPhone with month-by-month swipe cleanup, zero cloud telemetry, and 34+ localized languages. Built using [ios-agent-skills](https://github.com/rusel95/ios-agent-skills) and grown with [ios-aso-copilot](https://github.com/rusel95/ios-aso-copilot).
- **[Hush: White Noise & Sleep Aid](https://apps.apple.com/us/app/hush-white-noise-sleep-aid/id6449785515)** — Focused ambient sound mixer with 30+ layered audio loops, background playback, lock-screen controls, smart fade-out timer, and 49 localized languages.
- 🍎 *Explore all releases on my [Apple Developer Profile](https://apps.apple.com/us/developer/ruslan-popesku/id1627013326).*

---

### 🧪 Swift & Testing Open Source Contributions

- 🧪 **[agent-swift-XCTest](https://github.com/reportportal/agent-swift-XCTest)** *(Core Contributor & Maintainer)* — Official Swift XCTest agent for [ReportPortal.io](https://reportportal.io). Modernized architecture with `async/await` over ReportPortal v2 API, multi-process parallel worker launch merging (`RP_LAUNCH_UUID` / Info.plist), launch-gate synchronization, and real-device cloud farm (SauceLabs) orchestration.
- 🎬 **[MediaToolSwift](https://github.com/starkdmi/MediaToolSwift)** *(Contributor)* — Merged upstream [PR #13](https://github.com/starkdmi/MediaToolSwift/pull/13) fixing native iOS `AVAssetWriterInput` rejection of DCI-P3 wide-gamut video transcoding. Implemented single-encode AVFoundation compositor conversion to P3-D65 SDR (BT.709) and BT.2020 HDR (10-bit HLG/PQ) with orientation handling and comprehensive 83-test verification suite.

---

### 💼 Engineering Leadership & Experience

- **EPAM Systems** *(2021 — present)* · Lead iOS Engineer
  - **Disney+ Hotstar:** Technical Team Lead on a 600M+ user streaming platform with 200+ engineers; led feature delivery with 75% unit-test and 100% UI automation coverage.
  - **Thomson Reuters:** Senior iOS Engineer on a flagship news product serving 2M+ active users.
  - **Planoly:** Senior iOS Engineer on social media planning product with 50K+ subscribers.
  - **AI Department Champion:** Leading mobile agent-skill initiatives at EPAM; speaking on spec-driven development and deterministic coding agent evaluation.
- **Nullgravity** *(2019 — 2021)* · iOS Engineer
  - Shipped AR retail experience; reduced legacy clean build time by 60% (~20 min saved per developer daily).
- **Yalantis** *(2018 — 2019)* · iOS Engineer
  - Delivered commercial retail & social apps with complex third-party hardware/BLE and service integrations.

---

### 💻 Tech Stack & Craft

`Swift` · `SwiftUI` · `UIKit` · `Combine` · `Swift Concurrency` · `AVFoundation` · `TCA` · `VIPER` · `XCTest` · `Swift Testing` · `ReportPortal` · `Python` · `ChromaDB` · `Context Engineering`

---

### 📫 Connect

[![App Store](https://img.shields.io/badge/App_Store-Developer_Page-black?style=flat&logo=apple&logoColor=white)](https://apps.apple.com/us/developer/ruslan-popesku/id1627013326)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rusel95)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/rusel95)
[![Email](https://img.shields.io/badge/Email-ruslanpopesku95@gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:ruslanpopesku95@gmail.com)
