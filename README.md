# Sunwoo Moon

**Systems · Security · Developer Tooling**

I build local-first developer infrastructure, reproducible security tooling, and
low-level runtime experiments. My work focuses on explicit trust boundaries,
testable contracts, and evidence that distinguishes a working implementation
from an architectural claim.

## Selected work

### [Ditto](https://github.com/eunhhu/ditto)

A local-first semantic microkernel for AI agents, written in Rust. It provides a
durable event spine, bounded context and capability retrieval, content-addressed
artifacts, provider-neutral model contracts, and fail-closed effect leases.

- Rust workspace with formatting, Clippy, unit, integration, and doc-test gates
- Typed and replayable trust boundaries rather than implicit agent authority
- Repository-native contracts for long-running, agent-assisted development

### [flab](https://github.com/eunhhu/flab)

An authorized Frida instrumentation workbench for reproducible mobile and game
security research. A shared TypeScript core powers its TUI, CLI, MCP/ACP, and
structured agent interfaces.

- Device-safe process discovery, attach/spawn, tracing, and cleanup lifecycle
- Descriptor-driven instruments with bounded inputs and explicit side effects
- Unit, protocol, TUI, packaging, and native-runtime verification surfaces

### [RexPlayer](https://github.com/eunhhu/RexPlayer)

A container-native Android runtime and defensive security research project for
Windows/WSL2 and Linux. The public repository is intentionally evidence-led and
marks unimplemented product goals separately from reproduced runtime results.

- Reproduced Android 14 boot and ADB on Linux and Windows/WSL2 substrates
- Verified `/dev/uinput` to Android InputReader touchscreen path
- Defensive exposure matrix, integrity-checked evidence, and CI verification

## External validation

- [DreamHack profile](https://dreamhack.io/users/97873): **16,550 points, rank #28,
  76 challenges**, with a focus on reversing and systems security
- Frida Luma contributions merged upstream:
  [PR #3](https://github.com/frida/luma/pull/3) and
  [PR #4](https://github.com/frida/luma/pull/4)
- Paid client delivery across web, automation, and systems projects; detailed
  scope and redacted evidence are available in a role-specific résumé

## Engineering approach

- **Languages:** Rust, TypeScript/JavaScript, Python, C, Shell
- **Platforms:** Linux, Android, Windows/WSL2, containers, GitHub Actions
- **Focus:** platform engineering, developer experience, runtime security,
  reverse engineering, automation, and reliable operations
- **Workflow:** agent-assisted where useful, with human-owned architecture,
  explicit attribution, executable checks, and reproducible evidence

## Security boundary

Security work shown here is limited to systems I own or am authorized to test,
offline targets, and isolated research environments. The goal is defensive,
reproducible engineering—not unauthorized access or interference with other
users, services, or economies.
