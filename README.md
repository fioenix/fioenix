<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.svg">
  <img src="assets/banner-light.svg" alt="Fioenix · FINOLABS — tools, language, research" width="1200">
</picture>

# Hi, I'm Fioenix

**Building with [FINOLABS](https://github.com/finolabs) · Ho Chi Minh City, Vietnam.**

I build open-source Agent Skills, CLIs and MCP servers that make AI agents useful for real work: delegating across providers, writing natural Vietnamese, structuring ideas, and running projects. They plug into Claude Code and Codex, and the FINOLABS plugins also install on Google Antigravity.

## Agent tools

### [Agybird](https://github.com/finolabs/agybird) &nbsp;[![release](https://img.shields.io/github/v/release/finolabs/agybird?label=&color=7FE2CE)](https://github.com/finolabs/agybird/releases/latest)

Delegate code, image generation and general tasks from Claude Code or Codex to the official Google Antigravity CLI (`agy`), using your own Gemini subscription. No extracted credentials, no private APIs. Unofficial; not affiliated with Google.

```bash
claude plugin marketplace add finolabs/plugins
claude plugin install agybird@finolabs
```

### [FINOLABS Vibecode](https://github.com/finolabs/finolabs-vibecode) &nbsp;[![release](https://img.shields.io/github/v/release/finolabs/finolabs-vibecode?label=&color=7FE2CE)](https://github.com/finolabs/finolabs-vibecode/releases/latest)

17 skills and 3 agents (fnl-reviewer, fnl-security-reviewer, fnl-navigator) for review routing, verification, setup, run hygiene and quota on demand.

```bash
claude plugin marketplace add finolabs/plugins
claude plugin install finolabs-vibecode@finolabs
```

### [Vietnamizer](https://github.com/finolabs/vietnamizer) &nbsp;[![release](https://img.shields.io/github/v/release/finolabs/vietnamizer?label=&color=7FE2CE)](https://github.com/finolabs/vietnamizer/releases/latest)

Meaning-first Vietnamese editing for AI drafts, literal translations and workplace writing. Keep the source voice by default; adapt to supplied writing samples when explicitly requested, with checks for added facts, lost qualifications and unnecessary rewrites.

**Evidence, with limits:** the matched Codex regression comparison improved from **10/12 to 12/12 cases** between 0.12.0 and 0.12.1. These are development cases, not an independent quality estimate. Reference-voice pilots remain mixed; there are no independent human ratings yet. See [regression results](https://github.com/finolabs/vietnamizer/blob/main/specs/018-mr-version-comparison/results.md), the [0.13.2 voice pilot](https://github.com/finolabs/vietnamizer/blob/main/specs/025-section-voice-pilot/results.md), and [skills.sh](https://skills.sh/fioenix/vietnamizer/vietnamizer).

```bash
claude plugin marketplace add finolabs/plugins
claude plugin install vietnamizer@finolabs
```

Or as a plain skill, one path per agent:

```bash
npx skills add finolabs/vietnamizer --skill vietnamizer
```

### [Markmap Skills](https://github.com/finolabs/markmap-skills) &nbsp;[![release](https://img.shields.io/github/v/release/finolabs/markmap-skills?label=&color=7FE2CE)](https://github.com/finolabs/markmap-skills/releases/latest)

Turn notes and documents into editable Markdown and interactive Markmap mindmaps. Branch grouping, depth and concise labels are generation guidelines. Self-contained HTML requires Node.js and `markmap-cli`; the CDN template requires internet access. No background daemon. See [outputs and requirements](https://github.com/finolabs/markmap-skills#outputs-and-requirements).

```bash
claude plugin marketplace add finolabs/plugins
claude plugin install markmap-skills@finolabs
```

### [Huly Skill](https://github.com/fioenix/huly-skill) &nbsp;[![release](https://img.shields.io/github/v/release/fioenix/huly-skill?label=&color=7FE2CE)](https://github.com/fioenix/huly-skill/releases/latest)

A CLI, MCP server ([`@fioenix/huly-mcp`](https://www.npmjs.com/package/@fioenix/huly-mcp)) and agent skill for [Huly](https://huly.io): tasks, sub-issues, comments, documents, milestones and reports, with a JSON mode for agent pipelines.

```bash
npx skills add fioenix/huly-skill
```

> **On Codex?** Register the shared FINOLABS catalog once with `codex plugin marketplace add finolabs/plugins`, then install with `codex plugin add <name>@finolabs`, for example `codex plugin add agybird@finolabs`.
>
> **On Antigravity?** Install each plugin from its repository: `agy plugin install https://github.com/finolabs/<name>`.
>
> Installed from an older catalog (`agybird@Finolabs`, `agybird@agybird`, `markmap-skills@fioenix-plugins`)? Follow the [migration and rollback guide](https://github.com/finolabs/agybird/blob/main/docs/migration.md) before changing registrations.

## Research

### [Ignis](https://github.com/fioenix/fn-ignis)

A self-hosted research harness that tests market hypotheses against social-source evidence from Threads, TikTok, YouTube, Google Trends and Instagram. It keeps observations, contrary evidence and open questions inspectable. **Under development:** see [release status](https://github.com/fioenix/fn-ignis#verification-and-release-status).

## Around the projects

Fioenix and FINOLABS build and maintain these projects. [Finos (@im.finos)](https://www.threads.com/@im.finos) is an AI agent that shares experiments and promotes Fioenix's GitHub profile and public repositories, distinct from Fioenix, the human maintainer. Use GitHub for source, documentation and issues; browse the [skills.sh catalog](https://skills.sh/fioenix) for skill discovery, and follow Finos on Threads for demos and discussion.

## Stack

`TypeScript` · `Python` · `Go` · `MCP` · `Agent Skills` · `Claude Code` · `Codex` · `Antigravity`

---

[All public repositories](https://github.com/fioenix?tab=repositories&type=public) · [FINOLABS](https://github.com/finolabs) · [Developer hub](https://finolabs.io) · [fioenix@finolabs.io](mailto:fioenix@finolabs.io)
