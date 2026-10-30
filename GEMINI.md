# 🤖 Anti-Projects Workspace — AI Agent Workspace Instructions

> **ATTENTION ALL AI AGENTS (Antigravity, Cursor, Claude Code, Windsurf, Copilot, Gemini CLI)**  
> This workspace enforces an automated **AI-Native Knowledge Base System** located in [`knowledge/`](knowledge/).

---

## 1. Mandatory Pre-Execution Protocol (Strict Invariant)

> [!IMPORTANT]
> **MANDATORY FIRST TOOL ACTION**:
> On **ANY** task in this monorepo, your **VERY FIRST tool call MUST be inspecting [`knowledge/index.yaml`](knowledge/index.yaml)**.
> 
> When working inside a specific subproject (e.g. `Meet_recorder_chrome_extension/`), you MUST immediately transition to inspecting that subproject's dedicated `knowledge/index.yaml` and load its persona Knowledge Units.

1. **Query Master Index First**: Inspect [`knowledge/index.yaml`](knowledge/index.yaml) to identify the subproject catalog and workspace standards.
2. **Route to Subproject Knowledge Base**:
   - For **Meet Recorder Pro**: Inspect [`Meet_recorder_chrome_extension/knowledge/index.yaml`](Meet_recorder_chrome_extension/knowledge/index.yaml) and its associated Knowledge Units.
   - For **Monorepo Architecture**: Inspect [`ARCH-WS-001`](knowledge/architecture/ARCH-WS-001.yaml).
3. **Enforce Directives**: Strictly follow all `rule`, `do`, and `dont` fields in loaded Knowledge Units before taking any action.

---

## 2. Core Project Invariants

- **Monorepo Workspace Isolation**: Independent tool suites and extensions live in decoupled subdirectories with separate Git configurations and dependency managers.
- **Federated Knowledge Architecture**: The root catalog tracks active tools, while each individual subproject maintains an autonomous, fully specified `knowledge/` hierarchy.
- **Zero-Cloud & High Privacy**: All utility projects prioritize local-first execution, user privacy, and zero unnecessary telemetry.

---

## 3. Post-Change Knowledge Synchronization (Mandatory)

Whenever changes are made:
1. **Synchronize Subproject Knowledge**: Always update the target subproject's `knowledge/` folder and `index.yaml`.
2. **Synchronize Workspace Catalog**: Update `knowledge/index.yaml` if new subprojects or workspace-wide architectural rules are added.
