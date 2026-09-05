# 📜 The Architects Protocol
### Engineering Standards & Contribution Directives

Welcome to **baiersoft**. We are *architects of the unseen*—crafting digital monoliths at the intersection of mathematical beauty, fine-grained reactivity, and subterranean obsidian aesthetics.

To preserve the uncompromising quality and performance of our systems, all contributors and team members operate under **The Architects Protocol**.

---

## 🏛️ 1. Core Architectural Tenets

```
01 // SIMPLICITY FIRST
     Write the minimum code required to solve the vector.
     No speculative "flexibility," no premature abstractions for single-use routines.
     If a routine can be expressed cleanly in 30 lines, reject the 150-line framework.

02 // SURGICAL PRECISION
     Touch only what you must. Do not churn whitespace, reorder imports, or refactor
     adjacent code unrelated to your immediate mission. Every changed line must trace
     directly to an issue or directive.

03 // ZERO RUNTIME BLOAT
     Prefer native Web APIs (Web Audio API, WebGL 2.0, OffscreenCanvas, CSS Custom Properties)
     over heavy runtime dependencies. Every third-party package added must be rigorously justified.

04 // EMPIRICAL VERIFICATION
     Never declare a vector complete without automated verification. Unit tests must achieve
     high branch coverage, E2E tests must pass under chaos fault-injection, and frame budgets
     must remain locked.
```

---

## 🛰️ 2. Development & Git Workflow

### Branch Naming Conventions

All branches must adhere to our standardized vector prefixes:

| Vector Prefix | Purpose | Example |
| :--- | :--- | :--- |
| `orbit/*` | New functional features or experimental subsystems | `orbit/webgl-caustics` |
| `patch/*` | Critical fixes and anomaly resolutions | `patch/audio-suspend-jitter` |
| `perf/*` | Frame-budget, memory allocation, and speed optimizations | `perf/bounding-sphere-acceleration` |
| `telemetry/*` | Documentation, architecture specs, and logging telemetry | `telemetry/architecture-v2` |
| `refactor/*` | Surgical internal restructuring without external API change | `refactor/signal-primitives` |

### Commit Message Syntax (Conventional Commits)

Commit messages must be concise, descriptive, and follow the Conventional Commits specification:

```
<type>(<optional-scope>): <imperative description>

[optional detailed architectural body]

[optional issue reference: Resolves #42]
```

**Types:**
- `feat`: A new feature or subsystem capability.
- `fix`: An anomaly resolution or bug fix.
- `perf`: A code change that improves performance, framerate, or memory usage.
- `refactor`: A code change that neither fixes a bug nor adds a feature.
- `test`: Adding missing tests or correcting existing tests.
- `docs`: Documentation, architecture specs, or comments only.
- `chore`: Toolchain, dependency, or build configuration updates.

---

## ⚡ 3. Quality Assurance & Testing Mandate

Before submitting a Pull Request for architectural review:

1. **Unit & Integration Suite:**
   ```bash
   npm test
   # or: npx vitest run --coverage
   ```
   Ensure coverage thresholds are maintained with 0 failures.

2. **Chaos Resilience & E2E Verification:**
   ```bash
   npx playwright test
   ```
   Verify responsive viewport adaptation (from 280px foldables to 4K Ultrawide) and network degradation resilience.

3. **Production Build & Type Check:**
   ```bash
   npm run build
   ```
   Must compile cleanly under strict TypeScript with 0 compiler warnings.

---

## 🛡️ 4. Code Review & Transmission Standards

- **Pull Request Template:** Fill out all sections of [.github/PULL_REQUEST_TEMPLATE.md](https://github.com/baiersoft/.github/blob/main/.github/PULL_REQUEST_TEMPLATE.md). Include measured before/after telemetry.
- **Tone & Collaboration:** Technical discourse should be objective, analytical, and respectful. Critique the code and architectural vectors, never the person.
- **Merge Strategy:** Linear history with squash-and-merge or rebase to keep git logs pristine.


---

<div align="center">
  <sub>baiersoft // Architects of the unseen.</sub>
</div>
