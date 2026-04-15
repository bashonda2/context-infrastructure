# The Context Infrastructure Framework

**Persistent memory for AI agents that compounds across sessions.**

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Version](https://img.shields.io/badge/Version-3.2-green.svg)](FRAMEWORK.md)
[![Status](https://img.shields.io/badge/Status-Production--Tested-brightgreen.svg)](FRAMEWORK.md)

---

## The Problem

AI tools forget everything between sessions. Every new conversation starts from zero — no memory of prior decisions, established conventions, or past mistakes. On small projects this is manageable. On anything beyond a prototype, it becomes the dominant failure mode.

Most "use AI better" approaches treat each session as independent. You write a good prompt, you get a good answer, you start over tomorrow. The improvement is linear at best.

This framework solves the problem differently — and the result compounds.

## The Solution

Five structured documents that AI agents read at the start of every session and update at the end. A self-auditing rule that catches what the agent missed. A continuous improvement engine that refines the system itself. Together, they create persistent context that gets *better* with use, not just longer.

The five components:

- **5-document architecture** — Source of Truth, People & Relationships, Quality Contract, Operational Playbook, Projects & Ventures. Each document answers ONE question. Never mix concerns.
- **Hot/warm/cold memory tiers** — separate the context the AI reads every session from the context it consults when needed.
- **The Tenth Man Rule** — an 8-check self-auditing protocol run at the start and end of every session. Catches staleness, contradictions, gaps, changed truth, cascade risk, seed candidates, unvalidated assumptions, and missing honest findings.
- **Kaizen** — a continuous improvement engine that audits the framework's own practices at the end of every working day. Tenth Man asks "is this still true?" Kaizen asks "is this the best way?"
- **Cross-reference discipline** — every fact has ONE canonical home. Everywhere else uses references. Eliminates the contradiction failure mode that breaks long-running projects.

The complete framework is in [FRAMEWORK.md](FRAMEWORK.md) — about 30 minutes of reading.

## Why Now

In April 2026, four independent signals are converging on the same conclusion: context infrastructure is the rate-limiting step for the next generation of AI usefulness.

**Andrej Karpathy's "LLM Wiki" framing** publicly described what he called "the tractable form of brain upload" — the idea that a sufficiently rich corpus plus a capable LLM is, in practice, a near-term implementation of personal AI modeling. He sketched the pattern abstractly. This framework is one production-tested instance of it.

**The Genesis Mission** — the U.S. Department of Energy's Manhattan-Project-scale federal AI initiative — confirmed at scale that "the data is the heart of the equation." Structured, validated context layers are the bottleneck unlock for AI usefulness in scientific discovery. The federal government just validated the same thesis this framework demonstrates at smaller scale.

**Project Glasswing** revealed that frontier models can now find and exploit software vulnerabilities autonomously. The architectural response is sovereign, local, structured-context approaches — context infrastructure that runs on user-owned systems and surfaces only what each task requires.

**Capable open models** like Gemma 4 made native deep-thinking reasoning available on consumer hardware. Combined with structured context infrastructure, capable local models can match frontier closed models on the specific tasks the SOT has been shaped around. The hardware exists. The models exist. The missing piece, until now, has been the structured context layer.

This framework is one production-tested approach to that work, offered openly.

## Evidence

Every concept in the framework traces back to a specific failure encountered in production. None of it is theoretical. The release notes show every improvement and what triggered it.

The framework draws from three sources:

- **Production experience** refining and extending these patterns across hundreds of AI-assisted sessions over multiple weeks of real work.
- **Academic research** — Vasilopoulos (2026) formalizes a three-tier context architecture developed across 283 sessions on a 108,000-line distributed system, with quantitative evidence that structured context reduces errors and improves consistency over time.
- **Production benchmark research** has shown that the majority of AI tokens are wasted re-reading context, and that managed context can match frontier model quality at substantially lower cost. A methodology companion document with full quantitative results is forthcoming.

The Tenth Man Rule and the Kaizen engine exist because they fixed real failures. Every check in the 8-check audit corresponds to a specific class of error the framework caught. The framework is repaired from practice, not designed from theory.

## Quick Start

The fastest way to start is to let your AI tool create your Source of Truth for you.

1. **Read the framework** — [FRAMEWORK.md](FRAMEWORK.md) takes about 30 minutes. Worth it before you start.
2. **Open the [`prompts/`](prompts/) directory** and copy the Source of Truth setup prompt.
3. **Paste it into your AI tool of choice** — Cursor, Claude Code, Goose, Claude.ai, ChatGPT, or any other agent that can read and write files.
4. **Answer the agent's questions** about your project. The agent generates your Source of Truth in about 15 minutes, tailored to your specific work.

That's the entire onboarding. After step 4, you have a working SOT and the framework's maintenance discipline takes over from there. Add the other four documents (People, Quality Contract, Playbook, Projects) when your project grows enough to warrant them — usually after a few weeks of accumulated context, not on day one.

The framework is intentionally tool-agnostic. Prompts work in any AI tool that can follow text instructions. As tools evolve, the prompts keep working.

## What's in This Repo

- **[FRAMEWORK.md](FRAMEWORK.md)** — the complete framework document (~530 lines, ~30 minutes to read).
- **[`prompts/`](prompts/)** — setup prompts for each of the five documents. Paste these into your AI tool to generate your own SOT system.
- **[`examples/`](examples/)** — anonymized examples of mature SOT systems in production use.
- **[CHANGELOG.md](CHANGELOG.md)** — version history and release notes.
- **[LICENSE](LICENSE)** — Apache 2.0.
- **[NOTICE](NOTICE)** — copyright and attribution.

## Status & Contributing

Current version: **3.2** (April 14, 2026). See [CHANGELOG.md](CHANGELOG.md) for full history.

This framework is published as a working artifact, not as a managed product. Issues and discussions are welcome. Pull requests will be considered but not guaranteed to be merged — the framework's evolution is driven by production use, not feature requests.

If you build something on top of this, I'd love to hear about it. Find me on X at [@aaronblonquist](https://x.com/aaronblonquist).

## License

Apache License 2.0. Use, adapt, fork, and ship inside your own tooling. The implementations are yours; the principles are universal.

Copyright © 2026 Aaron Blonquist. See [LICENSE](LICENSE) for details.
