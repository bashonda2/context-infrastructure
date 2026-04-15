Release Notes
v3.2 — April 14, 2026
REPLACED: Templates with prompts. The framework no longer ships starter templates for users to download and edit by hand. Instead, the prompts/ directory contains setup prompts for each of the five documents. Users paste a prompt into their AI tool of choice (Cursor, Claude Code, Goose, Claude.ai, ChatGPT, or any other agent), the agent interviews them about their project, and the agent generates the document tailored to their work. This change reflects the framework's own thesis: AI agents become useful when they operate from structured context, and they are equally capable of creating that structured context when given the right instructions. Templates assumed humans should do the work the AI is capable of doing. Prompts close the loop.
REWRITE: Quick Start section. Restructured to lead with the prompts approach as the primary onboarding path, with the maintenance discipline (Tenth Man, Kaizen, splits, cross-references) following as the practices the user adopts after the initial setup. The Quick Start now reflects how the framework is actually adopted in 2026: inside an AI tool, with the AI doing the heavy lifting from the first interaction.
NEW: Tool-agnostic onboarding. Because prompts work in any AI tool that can read text, the framework is now portable across the entire AI tooling ecosystem without tool-specific instructions. The same prompts work in Cursor, Claude Code, Goose, Claude.ai, ChatGPT, and any future tool that can follow text instructions. This makes the framework more durable across time as tools evolve.
v3.1 — April 13, 2026
EXPANDED: Tenth Man Rule. Replaced the 5-check version with the full 8-check production checklist used in actual operational systems. Added the three sophisticated checks that distinguish a self-correcting system from a self-checking one: changed truth, cascade risk, and seed candidates. These are the checks that catch the silent-failure modes that the simpler version misses.
NEW: Continuous Improvement (Kaizen) section. Added a dedicated section explaining the Kaizen discipline that complements the Tenth Man Rule. Tenth Man audits accuracy; Kaizen audits process. The two together create a system that is both self-correcting and self-improving. Includes the full Kaizen process, principles, patterns, and the comparison table between the two engines.
NEW: Optional sixth document (Kaizen log). Acknowledged that projects with active improvement cycles warrant a dedicated Kaizen document, while smaller projects can keep proposals in the Quality Contract. The 5-document core architecture remains the foundation.
NEW: TL;DR at top of document. Single-paragraph summary for readers who will not read the full document.
NEW: Peripheral vision rule in the Tenth Man section. Names the principle that governs the tension between "keep Active Memory lean" and "keep Active Memory rich enough for the audit to find unexpected things."
NEW: Memory quality rule in the Deep Memory and Seeds section. Names the counterweight to the "keep it short" instinct: the test for memory quality is whether a fresh session can operate from the SOT alone.
EXPANDED: Session Protocol. End-of-session checklist now explicitly includes the Tenth Man audit (end-of-session pass) and seed trigger check, matching production practice. End-of-day Kaizen review added as a separate cadence.
EXPANDED: Maintenance Cadence table. Added Tenth Man audit as its own row at the top with explicit time estimate. Reordered to surface the most-frequent disciplines first.
NEW: Karpathy reference. Added Karpathy's April 10 LLM Wiki gist to the references section to match the body citation.
EDIT: SovereigntAI numbers softened. Replaced specific quantitative claims about token waste percentages and cost reduction figures with qualitative language ("the majority of AI tokens are wasted re-reading context, and managed context can match frontier model quality at substantially lower cost") pending publication of the underlying research.
EDIT: Practitioner section. Added a paragraph on the role of Kaizen in practice, complementing the existing reflection on the Tenth Man discipline.
EDIT: AI Partner perspective. Added a sentence explaining why Kaizen exists as a separate engine from the Tenth Man.
EDIT: Cross-Reference Discipline table. Added Kaizen Log row.
EDIT: Table alignment. Standardized markdown table syntax for cross-renderer compatibility.
v3.0 — April 13, 2026
NEW: Title and framing. Renamed from "Source of Truth Style Guide" to "The Context Infrastructure Framework." Subtitle now names the compounding dynamic explicitly: persistent memory for AI agents that compounds across sessions.
NEW: "The Moment This Framework Was Built For" section. Connects the framework to the four converging conversations of 2026: Karpathy's LLM Wiki framing, the Genesis Mission, the post-Glasswing threat landscape, and the arrival of capable open models like Gemma 4. Positions the framework as the production-tested instance of patterns now being discussed theoretically across the AI ecosystem.
NEW: "Why It Compounds" section. Names the central claim explicitly: this is not just persistent memory, it is memory that improves with use.
REWRITE: "What This Is" opening section. Replaces the previous problem-statement opening with a tighter framing that leads with the compounding claim.
REWRITE: "Beyond Code" section. Genericized from a single operational case study to a broader treatment covering operations, research, and knowledge work.
REWRITE: "From the Practitioner" section. Replaced the prior author-perspective material with a first-person practitioner reflection on what the framework actually feels like to use.
REWRITE: "From the AI Partner's Perspective" section. Tightened and reframed Goose's contribution to focus on the failure-driven design principle that distinguishes the framework.
SCRUB: Project-identifying specifics. Removed all references to specific employer projects, internal tool names, named individuals, and exact architecture counts that could fingerprint particular work. Quantitative claims from external research are preserved with their original citations. The author's own production experience is now described in qualitative ranges rather than precise counts.
LICENSE: Apache 2.0 (was previously implied open-source; now explicit).
PUBLICATION: First version released publicly via dedicated GitHub repository with templates, examples, and changelog.
v2.2 — April 8, 2026
NEW: Maintenance Cadence — defined frequencies for seeding (every session), SOT quality review (weekly), deep seeding pass (weekly), and Kaizen review (daily). Prevents bloat accumulation.
Moved from v2.1 same day based on production experience: first seeding pass revealed no cadence existed for ongoing maintenance.
v2.1 — April 8, 2026
NEW: Deep Memory and Seeds section — formalized link preservation as a hard rule. Links are non-compressible. Added seed quality checklist.
NEW: Version Management section — monthly version check cadence.
NEW: Release Notes — version history for users to track improvements.
First production seeding pass completed: substantial compression achieved from Active Memory to Deep Memory with zero information loss. All document links preserved.
v2.0 — April 2, 2026
Added 5-document architecture (expanded from 4-document in v1.0).
Added Tenth Man Rule (self-auditing framework).
Added hot/warm/cold memory model.
Added cross-reference discipline.
Added operations use case (beyond code).
Added AI partner perspective.
Added People & Relationships as dedicated document.
Added Projects & Ventures as dedicated document.
v1.0 — April 2, 2026
Initial release. 4-document architecture (Source of Truth, Data Reference, Quality Contract, Operational Playbook).
Based on production experience across multiple AI-assisted development projects.
Incorporated Vasilopoulos (2026) codified context research.
Incorporated production research on managed context performance.
This framework is open source under the Apache License 2.0. Adapt it for your domain, your tools, your team. The principles are universal — the implementations are yours.

© 2026 Aaron Blonquist. Licensed under Apache 2.0.
