# Agent Skills

A collection of skills for AI coding agents.

Skills follow the [Agent Skills](https://agentskills.io/) format.

## Agent and Plugin Compatibility

This repository is structured around portable Agent Skills and can also be used as a Codex plugin.

- Agent Skills remain in `skills/<skill-name>/SKILL.md` with optional `references/`, `assets/`, `evals/`, and agent-specific metadata.
- Codex plugin metadata lives in `.codex-plugin/plugin.json` and points to the existing `./skills/` directory.
- Agent-specific files belong under each skill's `agents/` directory so future agents can add their own metadata without changing the skill content.
- Shared guidance should stay in `SKILL.md` and `references/`; keep Codex-only behavior in plugin or `agents/openai.yaml` metadata.

### Use as a Codex Plugin

Install or package this repository as a local Codex plugin from the repository root. The Codex manifest is intentionally thin and reuses the same `skills/` tree used by other Agent Skills-compatible tooling.

## Available Skills

### android-mvi (thx to @soracel for co-authoring)

Use this skill when creating, migrating, or reviewing Android MVI screens in Kotlin or Jetpack Compose. Apply it to name `UserIntent`, `UiState`, `SideEffect`, and `MVIViewModel` contracts; separate persistent render state from one-shot effects; enforce exhaustive sealed-interface handling; or document shared MVI primitives.

#### Install android-mvi

<details open>
<summary>bun</summary>

```bash
bunx skills add swissonid/agent-skills --skill android-mvi
```

</details>

<details>
<summary>pnpm</summary>

```bash
pnpm dlx skills add swissonid/agent-skills --skill android-mvi
```

</details>

<details>
<summary>npm</summary>

```bash
npx skills add swissonid/agent-skills --skill android-mvi
```

</details>

### android-clean-architecture (thx to @soracel for co-authoring)

Use this skill when creating, migrating, or reviewing Android Kotlin features with clean architecture boundaries, suspend use case or action classes, optional suspend repositories, Result-based failure handling, no thrown exceptions above repositories, and TDD-first implementation.

#### Install android-clean-architecture

<details open>
<summary>bun</summary>

```bash
bunx skills add swissonid/agent-skills --skill android-clean-architecture
```

</details>

<details>
<summary>pnpm</summary>

```bash
pnpm dlx skills add swissonid/agent-skills --skill android-clean-architecture
```

</details>

<details>
<summary>npm</summary>

```bash
npx skills add swissonid/agent-skills --skill android-clean-architecture
```

</details>

### android-clean-mvi (thx to @soracel for co-authoring)

Use this skill when creating, migrating, or reviewing a complete Android Kotlin or Jetpack Compose screen that combines MVI presentation contracts with clean architecture boundaries, including `UserIntent`, `UiState`, `SideEffect`, `MVIViewModel`, `Action` or `UseCase` dependencies, `Result`-based errors, and no ViewModel access to repositories or data sources.

#### Install android-clean-mvi

<details open>
<summary>bun</summary>

```bash
bunx skills add swissonid/agent-skills --skill android-clean-mvi
```

</details>

<details>
<summary>pnpm</summary>

```bash
pnpm dlx skills add swissonid/agent-skills --skill android-clean-mvi
```

</details>

<details>
<summary>npm</summary>

```bash
npx skills add swissonid/agent-skills --skill android-clean-mvi
```

</details>
