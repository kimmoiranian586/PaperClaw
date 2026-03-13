# PaperClaw

#CA: 8Sr83QJW12HMnxvg7HzHZvdFfj6G8j7AwzKmyBfRpump

**A production-ready OpenClaw skill library for academic research teams**

[![Skills](https://img.shields.io/badge/skills-27-blue?style=flat-square)]()
[![Literature](https://img.shields.io/badge/📚_literature-6-purple?style=flat-square)]()
[![Synthesis](https://img.shields.io/badge/🔬_synthesis-5-green?style=flat-square)]()
[![Collaboration](https://img.shields.io/badge/🤝_collaboration-5-orange?style=flat-square)]()
[![Output](https://img.shields.io/badge/✍️_output-6-red?style=flat-square)]()
[![Tracking](https://img.shields.io/badge/📡_tracking-5-yellow?style=flat-square)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey?style=flat-square)]()

<img width="1024" height="1024" alt="Image" src="https://github.com/user-attachments/assets/d1270796-a244-45f7-af51-4fb070dbfe1f" />

> **English** · 简体中文 *(coming soon)*

> [!NOTE]
> PaperClaw is a skill library, not a monolithic software package. You can install the full collection or copy only the skill folders that match your team's workflows.

---

## Overview

PaperClaw packages **27 production-ready `SKILL.md` files** for academic research team workflows across literature management, synthesis, collaboration, manuscript output, and research tracking. Each skill teaches an OpenClaw-compatible agent **when** to use a capability, **how** to invoke it, and **what kind of output** to produce.

PaperClaw is designed for research teams — labs, collaborative projects, cross-institution groups — who want a shared AI research layer rather than isolated personal tools. It is the **knowledge management and collaboration complement** to [LabClaw](https://github.com/wu-yc/LabClaw)'s biomedical execution toolkit.

| | LabClaw | PaperClaw |
|---|---|---|
| **Focus** | Biomedical tools & databases | Cross-field knowledge workflows |
| **Unit** | Solo researcher | Research team / lab |
| **Emphasis** | Execution (run analysis) | Synthesis & collaboration |
| **Scope** | Bio / pharma / med | Any academic field |

## At a Glance

| Domain | Skills | Focus |
|---|---|---|
| [📚 Literature](#-literature--6-skills) | **6** | Living reviews, monitoring, citation graphs, gap detection |
| [🔬 Synthesis](#-synthesis--5-skills) | **5** | Contradiction detection, consensus mapping, evidence grading |
| [🤝 Collaboration](#-collaboration--5-skills) | **5** | Annotation sharing, expertise mapping, knowledge handoffs |
| [✍️ Output](#️-output--6-skills) | **6** | Draft generation, grants, rebuttals, presentation decks |
| [📡 Tracking](#-tracking--5-skills) | **5** | Hypothesis versioning, preprint watch, citation alerts |

## Quick Start

OpenClaw loads workspace skills from `<workspace>/skills`. A practical setup:

```bash
git clone https://github.com/meowscles69/PaperClaw.git
mkdir -p ~/.openclaw/workspace/skills
cp -R PaperClaw/skills/* ~/.openclaw/workspace/skills/
```

Then start a **new OpenClaw session** so the skill folders are picked up. If you keep your workspace in git, merge only the folders you need rather than copying the full library.

## Repository Layout

```
PaperClaw/
├── README.md
└── skills/
    ├── literature/      # 6 skills: living reviews, arXiv monitoring, citation graphs, gap detection
    ├── synthesis/       # 5 skills: contradiction detection, consensus mapping, evidence grading
    ├── collaboration/   # 5 skills: annotation sharing, expertise mapping, knowledge handoffs
    ├── output/          # 6 skills: draft generation, grants, rebuttals, presentations
    └── tracking/        # 5 skills: hypothesis versioning, preprint watch, citation alerts
```

---

## 📚 Literature — 6 skills

> Tools for managing, discovering, and structuring the academic literature your team reads.

| Skill | Description |
|---|---|
| [`living-review`](skills/literature/living-review/SKILL.md) | Maintains a continuously updated, structured literature review for a research team. Ingests papers from multiple sources and synthesizes findings across the team's collective reading into a living document. |
| [`arxiv-monitor`](skills/literature/arxiv-monitor/SKILL.md) | Monitors arXiv for new papers matching team research interests. Scores relevance, deduplicates against existing library, and surfaces the most important new work — replacing manual daily browsing. |
| [`citation-graph`](skills/literature/citation-graph/SKILL.md) | Builds and analyzes citation networks around a body of papers. Reveals foundational works, emerging clusters, and the intellectual lineage of a research area. |
| [`gap-detection`](skills/literature/gap-detection/SKILL.md) | Analyzes a team's literature base to identify what has NOT been studied, contested, or resolved. Surfaces research gaps, methodological blind spots, and open questions. |
| [`semantic-scholar`](skills/literature/semantic-scholar/SKILL.md) | Queries the Semantic Scholar Academic Graph API for paper metadata, citations, author profiles, and semantic search across 200M+ papers. |
| [`zotero-integration`](skills/literature/zotero-integration/SKILL.md) | Connects to a team's Zotero library via the Web API. Reads, writes, and syncs paper collections, annotations, and notes — bridging existing reference workflows with PaperClaw. |

---

## 🔬 Synthesis — 5 skills

> Tools for extracting meaning across papers, not just within them.

| Skill | Description |
|---|---|
| [`contradiction-detection`](skills/synthesis/contradiction-detection/SKILL.md) | Scans a corpus of papers for conflicting empirical claims, methodological disagreements, or opposing conclusions. Surfaces genuine scientific contradictions before the team cites conflicting work. |
| [`consensus-mapping`](skills/synthesis/consensus-mapping/SKILL.md) | Identifies what the field broadly agrees on versus what remains contested. Produces a "state of knowledge" map separating settled science from active debate. |
| [`claim-tracker`](skills/synthesis/claim-tracker/SKILL.md) | Tracks specific scientific claims across the literature over time — who made the claim, who replicated it, who challenged it, and whether it still stands. |
| [`cross-paper-synthesis`](skills/synthesis/cross-paper-synthesis/SKILL.md) | Synthesizes findings across multiple papers into coherent narrative, structured comparison, or temporal evolution. Produces insights that only emerge from reading across the corpus as a whole. |
| [`evidence-grading`](skills/synthesis/evidence-grading/SKILL.md) | Evaluates the strength of evidence behind scientific claims based on study design, replication status, venue quality, and recency. Produces structured evidence grades. |

---

## 🤝 Collaboration — 5 skills

> Tools for making a lab's collective knowledge more than the sum of its parts.

| Skill | Description |
|---|---|
| [`annotation-sharing`](skills/collaboration/annotation-sharing/SKILL.md) | Enables a team to share, discuss, and build on PDF annotations across papers. Transforms isolated highlights into a shared knowledge layer. |
| [`expertise-mapping`](skills/collaboration/expertise-mapping/SKILL.md) | Maps expertise distribution across the team based on reading history and annotations. Answers "who knows the most about X?" and identifies knowledge gaps. |
| [`lab-knowledge-handoff`](skills/collaboration/lab-knowledge-handoff/SKILL.md) | Packages a departing team member's knowledge into a structured handoff document. Prevents institutional knowledge loss when students graduate or postdocs move on. |
| [`reading-coverage`](skills/collaboration/reading-coverage/SKILL.md) | Tracks which papers the team has collectively read and what important papers remain unread. Acts as the team's reading dashboard. |
| [`team-sync`](skills/collaboration/team-sync/SKILL.md) | Generates structured lab meeting agendas and paper discussion summaries based on recent team reading activity and open questions. |

---

## ✍️ Output — 6 skills

> Tools for turning research knowledge into manuscripts, grants, and presentations.

| Skill | Description |
|---|---|
| [`draft-generation`](skills/output/draft-generation/SKILL.md) | Generates manuscript sections grounded in the team's literature base — with all claims citation-traced and calibrated to evidence grades. |
| [`grant-writing`](skills/output/grant-writing/SKILL.md) | Generates agency-specific grant proposal sections (NIH, NSF, ERC, Wellcome) grounded in the team's literature and research history. |
| [`review-response`](skills/output/review-response/SKILL.md) | Drafts structured, evidence-backed responses to peer reviewer comments. Surfaces relevant literature, recommends strategy, and generates cover letters. |
| [`abstract-writing`](skills/output/abstract-writing/SKILL.md) | Drafts venue-appropriate abstracts in structured and unstructured formats at multiple word counts, including lay summaries. |
| [`rebuttal-writing`](skills/output/rebuttal-writing/SKILL.md) | Drafts concise, strategic rebuttals for conference reviews under tight word limits (NeurIPS, ICML, ICLR, ACL). |
| [`presentation-deck`](skills/output/presentation-deck/SKILL.md) | Generates structured slide outlines and content for conference talks, lab meetings, and thesis defenses calibrated to duration and audience. |

---

## 📡 Tracking — 5 skills

> Tools for maintaining a living record of the team's scientific thinking.

| Skill | Description |
|---|---|
| [`hypothesis-versioning`](skills/tracking/hypothesis-versioning/SKILL.md) | Maintains version-controlled registry of team hypotheses — tracking evolution, evidence, and reasoning behind each revision. |
| [`experiment-log`](skills/tracking/experiment-log/SKILL.md) | Maintains a structured, searchable log of experiments linking each run to its hypothesis, motivating papers, and conclusions. |
| [`reproducibility-check`](skills/tracking/reproducibility-check/SKILL.md) | Evaluates reproducibility of papers or team's own work against venue-specific standards (NeurIPS, Nature, ICML). Flags issues before reviewers do. |
| [`preprint-watch`](skills/tracking/preprint-watch/SKILL.md) | Monitors preprint servers for relevant work, tracks preprint-to-publication transitions, and alerts when cited preprints are updated. |
| [`citation-alert`](skills/tracking/citation-alert/SKILL.md) | Monitors citation activity for the team's own papers. Identifies who cites the team's work and classifies citation type (builds on / challenges / compares). |

---

## Skill Format

Every `SKILL.md` follows a consistent structure:

```
# Skill Name
## Overview        — what this skill enables
## When to Use     — trigger conditions for the AI agent
## Key Capabilities — specific tools, APIs, parameters
## Usage Examples  — concrete code or workflow examples
## Output Format   — what the skill returns
## Notes           — caveats, integrations, and tips
```

## Representative Workflows

| Workflow | Skills involved |
|---|---|
| Start a new research project | `arxiv-monitor` → `living-review` → `gap-detection` → `hypothesis-versioning` |
| Write a paper | `cross-paper-synthesis` → `draft-generation` → `abstract-writing` → `reproducibility-check` |
| Respond to reviewers | `review-response` → `evidence-grading` → `rebuttal-writing` |
| Lab meeting prep | `reading-coverage` → `team-sync` → `annotation-sharing` |
| Onboard a new team member | `expertise-mapping` → `reading-coverage` → `lab-knowledge-handoff` |
| Write a grant | `gap-detection` → `consensus-mapping` → `grant-writing` |

## Related Repositories

| Repository | Why it matters |
|---|---|
| [`wu-yc/LabClaw`](https://github.com/wu-yc/LabClaw) | Biomedical execution toolkit — 206 skills for biology, pharma, medicine, and literature search. PaperClaw is the collaboration and synthesis complement. |
| [`openclaw/openclaw`](https://github.com/openclaw/openclaw) | The main runtime that loads workspace skills and provides the agent workspace model PaperClaw is designed for. |
| [`mims-harvard/ToolUniverse`](https://github.com/mims-harvard/ToolUniverse) | Large AI-scientist tool ecosystem. Several PaperClaw skills integrate with ToolUniverse's literature search tools. |

## License

MIT License
