# inbrace-model-upgrade

The plugin was named `claude-config` before 0.4.0 and `inbrace-config` before 0.9.0. Entries before 0.7.0 are condensed; the full notes of each release are on the repository's GitHub Releases page.

## 0.9.2

### Patch Changes

- The plugin's display name is now "Model Upgrade Audit"; its `name` and commands are unchanged. ([#169](https://github.com/inbrace-tech/claude-plugins/pull/169) by [@ropdias](https://github.com/ropdias))

## 0.9.1

### Patch Changes

- The eval suite's guide moves out of the plugin folder to the repository's `docs/eval-suite.md`; the suite itself stays in `evals/`. ([#165](https://github.com/inbrace-tech/claude-plugins/pull/165) by [@ropdias](https://github.com/ropdias))

## 0.9.0

### Minor Changes

- The plugin is renamed `inbrace-model-upgrade`; the marketplace maps the old name, so update the marketplace and run `/plugin install inbrace-model-upgrade@inbrace` once. ([#161](https://github.com/inbrace-tech/claude-plugins/pull/161) by [@ropdias](https://github.com/ropdias))

### Patch Changes

- The eval suite's README names the sandbox prerequisites and links the platform list instead of showing a package-manager command. ([#159](https://github.com/inbrace-tech/claude-plugins/pull/159) by [@ropdias](https://github.com/ropdias))

## 0.8.2

### Patch Changes

- Directory listing cleanup: trim the regression suite's graders, condense the older changelog entries, drop `documentationUrl` and point every older link at inbrace-tech/claude-plugins. ([#155](https://github.com/inbrace-tech/claude-plugins/pull/155) by [@ropdias](https://github.com/ropdias))

## 0.8.1

### Patch Changes

- Point the plugin's homepage, repository, documentation and issue links at inbrace-tech/claude-plugins, the repository's new name. ([#150](https://github.com/inbrace-tech/claude-plugins/pull/150) by [@ropdias](https://github.com/ropdias))

- Transition audits: re-verify every quoted passage against today's docs, and update sampling, computer-use, 1M-context, subagent-effort, strict-tool and advisor traps that changed. ([#152](https://github.com/inbrace-tech/claude-plugins/pull/152) by [@ropdias](https://github.com/ropdias))

## 0.8.0

### Minor Changes

- Add the Claude Haiku 4.5 → Haiku 5.5 transition audit, started with `/inbrace-config:audit-haiku-5-5`, with its known traps, change digest and regression cases. ([#136](https://github.com/inbrace-tech/claude-plugins/pull/136) by [@ropdias](https://github.com/ropdias))

### Patch Changes

- Sonnet 5 → 5.5 audit: price Claude Sonnet 5.5 cache reads at USD 0.10 per million tokens, half Sonnet 5's, and flag a price entry copied from Sonnet 5. ([#138](https://github.com/inbrace-tech/claude-plugins/pull/138) by [@ropdias](https://github.com/ropdias))

## 0.7.0

### Minor Changes

- The audit works only from the change digest shipped with each transition: the drift stage and the docs-only mode are gone, and the contribution invite only gives a link. ([#114](https://github.com/inbrace-tech/claude-plugins/pull/114) by [@ropdias](https://github.com/ropdias))

### Patch Changes

- The Sonnet regression fixture's sample clients leave their credential to the SDK. ([#103](https://github.com/inbrace-tech/claude-plugins/pull/103) by [@ropdias](https://github.com/ropdias))

- Two known traps follow the docs as they read today: Opus P04's passage is re-recorded, and Sonnet P25 now says Opus 5.5 reads Sonnet 5.5 thinking blocks on the Claude API and Google Cloud. ([#112](https://github.com/inbrace-tech/claude-plugins/pull/112) by [@ropdias](https://github.com/ropdias))

- Every passage the knowledge files quote was re-checked against Anthropic's docs on 2026-10-06 and still holds, so each `verified` date now reads 2026-10-06. ([#123](https://github.com/inbrace-tech/claude-plugins/pull/123) by [@ropdias](https://github.com/ropdias))

- Each transition ships a change digest beside its known traps: what changed between the two models, each item with its page and a short quoted passage. ([#111](https://github.com/inbrace-tech/claude-plugins/pull/111) by [@ropdias](https://github.com/ropdias))

- The README and descriptions say the audit works from the docs as recorded and dated in the plugin. ([#115](https://github.com/inbrace-tech/claude-plugins/pull/115) by [@ropdias](https://github.com/ropdias))

## 0.6.3

- A listing icon, a README for the plugin folder, and re-tests for lines that restate an agent's or skill's effort.

## 0.6.2

- New and refined known traps for both audits, and a verifier that checks a file's existence before calling it missing.

## 0.6.1

- A regression suite for the Sonnet 5.5 and Opus 5.5 audits, more known traps, and a verifier that corrects every `file:line` it cites.

## 0.6.0

- One transition-agnostic audit behind the Opus and Sonnet commands, with a dollar cost estimate and each run kept in `.model-audits/`.

## 0.5.0

- The Sonnet 5 → 5.5 audit, `/inbrace-config:audit-sonnet-5-5`, and arguments that let both audits stop at the report.

## 0.4.7

- Advice the guide only offers is shown as optional.

## 0.4.6

- The cost footer explains what its token figures leave out.

## 0.4.5

- Estimates follow the measured run, and P01 keeps a `[1m]` model suffix.

## 0.4.4

- One agent per area, a `finding-verifier` for every finding, and a chat summary of what would change.

## 0.4.3

- Audit subagents run as the plugin's own read-only agent.

## 0.4.2

- The plan shows tables by area and by option.

## 0.4.1

- Cost figures include verifying and closing.

## 0.4.0

- The plugin is renamed `inbrace-config`, and the audit is `/inbrace-config:audit-opus-5-5`.

## 0.3.1

- Reports follow your language, and an interrupted run resumes where it stopped.

## 0.3.0

- The audit shows its plan and cost before reading, and asks what to apply.

## 0.2.0

- The audit is scoped to the Opus 5 → 5.5 transition and applies only approved changes.

## 0.1.0

- First audit of `CLAUDE.md`, rules, agents, skills and settings for the Opus 5 transition.
