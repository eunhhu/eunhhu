# Sunwoo Moon

I question inherited abstraction layers and build the runtime, language, and surface stack from the ground up.

Most modern software stacks pile database servers, ORMs, message queues, caches, routers, and separate UI code on top of a small state transition. At **[Yeowoo Labs](https://github.com/yeowoo-labs)**, I work on collapsing those layers into deterministic, local-first native systems with zero unnecessary middlemen—where storage, transport, execution, and interfaces share one mathematical contract.

---

### Core Direction

- **Abstraction Compression ([Pure · aup · Vega](https://github.com/yeowoo-labs))**
  Designing a C micro-runtime (`Pure`), its language and bytecode compiler (`aup`), and a unified surface SDK (`Vega` — TUI, CLI, Web, DirectFB from one spec). Events are total, atomic, deterministic functions over persistent B+tree state (`step : S × E → (S × Out*) ⊎ Fault`); views are pure snapshot reads; node-to-node links are connectionless, HPKE-sealed from packet one, and delivered exactly once.

- **Local-First Agent Infrastructure ([Ditto](https://github.com/eunhhu/ditto))**
  A Rust microkernel for long-running personal AI agents built around an append-only event spine, scoped memory, content-addressed artifacts, and explicit capability boundaries instead of opaque prompt loops.

- **Runtime Security & Low-Level Systems**
  Building reproducible dynamic analysis and native host substrates rather than treating binaries and OS runtimes as black boxes:
  - **[flab](https://github.com/eunhhu/flab)** & **[vlitz](https://github.com/eunhhu/vlitz)** — Frida-based runtime instrumentation workbench (TUI · CLI · MCP/ACP) and process inspection tooling.
  - **[RexPlayer](https://github.com/eunhhu/RexPlayer)** — Container-native Android 14 runtime host and raw input bridge for Linux & WSL2.
  - **[Spellwire](https://github.com/eunhhu/spellwire)** & **[remotepad](https://github.com/eunhhu/remotepad)** — Sub-millisecond native input automation and binary UDP touch controllers in Rust.

---

### Upstream & Track Record

- **Open Source:** Merged runtime reliability and session provider patches into **[frida/luma](https://github.com/frida/luma)** ([#3](https://github.com/frida/luma/pull/3), [#4](https://github.com/frida/luma/pull/4)).
- **Offensive & Defensive Security:** Ranked **#28 on [DreamHack](https://dreamhack.io/users/97873)** (16,550 pts · 76 challenges solved), specializing in binary reverse engineering, Android internals, and systems exploitation.
- **How I Work:** Measure instructions, bytes per commit, and tail latency on constrained hardware (Raspberry Pi 5, ARM64) before trusting abstractions; verify identical state across architectures (`aarch64`, `x86_64`, `arm64-apple`).
