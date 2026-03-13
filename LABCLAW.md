# LabClaw × PaperClaw

**Sister library contribution by [wu-yc](https://github.com/wu-yc)**

---

## About LabClaw

[LabClaw](https://github.com/wu-yc/LabClaw) is a production-ready OpenClaw skill library for **autonomous biomedical research**, packaging **206 `SKILL.md` files** across biology, drug discovery, medicine, data science, and literature search.

It is the **execution complement** to PaperClaw's knowledge and collaboration layer.

| | PaperClaw | LabClaw |
|---|---|---|
| **Focus** | Cross-field knowledge workflows | Biomedical tools & databases |
| **Unit** | Research team / lab | Solo researcher |
| **Emphasis** | Synthesis & collaboration | Execution (run analysis) |
| **Scope** | Any academic field | Bio / pharma / med |
| **Skills** | 27 | 206 |

---

## LabClaw Skill Domains

| Domain | Skills | Focus |
|---|---|---|
| [🧬 Biology & Life Sciences](https://github.com/wu-yc/LabClaw/blob/main/skills/bio) | **73** | Bioinformatics, single-cell, genomics, proteomics, multi-omics, databases, lab platforms |
| [💊 Pharmacy & Drug Discovery](https://github.com/wu-yc/LabClaw/blob/main/skills/pharma) | **36** | Cheminformatics, molecular ML, docking, target research, pharmacology, drug databases |
| [🏥 Medical & Clinical](https://github.com/wu-yc/LabClaw/blob/main/skills/med) | **20** | Clinical trials, precision medicine, oncology, infectious disease, medical imaging |
| [⚙️ General & Data Science](https://github.com/wu-yc/LabClaw/blob/main/skills/general) | **48** | Statistics, machine learning, data management, visualization, scientific writing |
| [📚 Literature & Search](https://github.com/wu-yc/LabClaw/blob/main/skills/literature) | **29** | Academic search, biomedical databases, multi-source discovery, patents, grants, citations |

---

## How the Two Libraries Work Together

PaperClaw and LabClaw are designed to be used side-by-side in the same OpenClaw workspace. A combined install gives research teams both execution depth (LabClaw) and synthesis/collaboration breadth (PaperClaw).

```bash
# Install both libraries into your OpenClaw workspace
git clone https://github.com/meowscles69/PaperClaw.git
git clone https://github.com/wu-yc/LabClaw.git

mkdir -p ~/.openclaw/workspace/skills
cp -R PaperClaw/skills/* ~/.openclaw/workspace/skills/
cp -R LabClaw/skills/* ~/.openclaw/workspace/skills/
```

### Representative cross-library workflows

| Workflow | PaperClaw skills | LabClaw skills |
|---|---|---|
| Single-cell research project | `living-review` → `gap-detection` | `scanpy` → `scvi-tools` → `tooluniverse-single-cell` |
| Drug discovery pipeline | `cross-paper-synthesis` → `evidence-grading` | `rdkit` → `diffdock` → `tooluniverse-drug-repurposing` |
| Grant writing | `consensus-mapping` → `grant-writing` | `pubmed-search` → `tooluniverse-literature-deep-research` |
| Respond to reviewers | `review-response` → `rebuttal-writing` | `statistical-analysis` → `reproducibility-checklist` |
| Onboard new team member | `expertise-mapping` → `lab-knowledge-handoff` | `literature-review` → `scientific-writing` |

---

## Credits

LabClaw is curated by **Yingcheng (Charles) Wu** at Le Cong Lab (Stanford) & Mengdi Wang Lab (Princeton).

→ [github.com/wu-yc/LabClaw](https://github.com/wu-yc/LabClaw)

---

*MIT License*
