# Sunwoo Moon

**Systems · Security · Developer Tooling**

I build local-first AI infrastructure, instrumentation tools, and Android runtime
experiments. I focus on explicit trust boundaries, testable contracts, and
reproducible evidence.

## Merged upstream: Frida Luma

- [**#3 · Harden Luma bug paths**](https://github.com/frida/luma/pull/3):
  improved build reliability, instrument-path validation, error reporting, and
  handling of malformed input or unavailable runtime resources.
- [**#4 · Fix mission session providers**](https://github.com/frida/luma/pull/4):
  fixed live assistant-text continuity and added an OpenAI-compatible mission
  provider with optional API keys and corrected URL handling.

Both contributions were merged into [frida/luma](https://github.com/frida/luma).

## Selected work

### [Ditto](https://github.com/eunhhu/ditto) · Local-first personal AI

- **Problem:** Keep long-running personal AI work manageable as memory,
  capabilities, and scheduled tasks grow.
- **Core:** A Rust runtime with an append-only event spine, scoped memory,
  bounded context retrieval, content-addressed artifacts, and explicit effect
  permissions.
- **Evidence & stage:** An executable foundation with
  [offline memory-correction and restart evidence](https://github.com/eunhhu/ditto/blob/main/docs/agent/tasks/015-evidence.md).
  The synthetic checks cover corrected-memory inclusion and irrelevant or
  cross-session memory exclusion; they do not establish general live-agent
  quality. Broader tool execution and efficiency goals remain in development.

### [flab](https://github.com/eunhhu/flab) · Reproducible instrumentation

- **Problem:** Keep authorized runtime research repeatable across manual and
  automated interfaces, with explicit session ownership and cleanup.
- **Core:** A shared TypeScript engine behind a guided TUI, CLI, and MCP/ACP
  interfaces, with bounded recording and descriptor-driven instruments.
- **Evidence & stage:** The
  [Android live-verification report](https://github.com/eunhhu/flab/blob/main/docs/android-live-verification.md)
  records device-specific results, restoration and cleanup, excluded targets,
  and remaining blockers. Coverage is limited to the documented authorized
  offline tests.

### [RexPlayer](https://github.com/eunhhu/RexPlayer) · Android runtime research

- **Problem:** Explore a small native host for container-based Android on
  Windows/WSL2 and Linux.
- **Core:** Android substrate experiments, a native input path, host capability
  inspection, and an early Rust host UI.
- **Evidence & stage:** The
  [runtime verification report](https://github.com/eunhhu/RexPlayer/blob/main/docs/VERIFICATION_2026-08-20.md)
  documents Android 14 boot, ADB, and raw touchscreen-input delivery on two lab
  substrates. This is a pre-alpha research project; integrated rendering,
  audio, production packaging, and performance remain unverified.

## More tooling

- [remotepad](https://github.com/eunhhu/remotepad): Rust remote-input server,
  binary UDP protocol, and web layout editor.
- [Spellwire](https://github.com/eunhhu/spellwire): TypeScript-to-native input
  automation with a Rust runtime, stateful hotkeys, and overlays.
- [Vlitz](https://github.com/eunhhu/vlitz): Frida-based dynamic debugging and
  process-analysis CLI in Rust.

## External validation

- [DreamHack profile](https://dreamhack.io/users/97873): **16,550 points, rank #28,
  76 challenges**, with a focus on reversing and systems security
- Paid client delivery across web, automation, and systems projects; detailed
  scope and redacted evidence are available in a role-specific resume

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
