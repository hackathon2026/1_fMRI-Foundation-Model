# Manuscript Quick Start Guide

**Created**: 2024-12-22

---

## 🎯 Getting Started

### Step 1: Understand the Structure
Read `OVERVIEW.md` - it's your mission control for the entire manuscript process.

### Step 2: Organize References
1. Upload PDF papers to appropriate folders in `papers/`:
   - `papers/transformers/` - Vision transformer papers
   - `papers/fmri_analysis/` - Brain imaging papers
   - `papers/pretraining/` - Self-supervised learning papers

2. Follow naming convention: `FirstAuthor_YYYY_ShortTitle.pdf`

3. Update OVERVIEW.md "Reference Papers" section as you add papers

### Step 3: Generate Results
1. Run experiments and save results to `data/tables/`
2. Create figure generation scripts in `scripts/`
3. Save figures to appropriate subdirectories in `figures/`

### Step 4: Start Writing
1. Work in `drafts/current_draft.md`
2. Use the provided template as starting point
3. Save versions as `drafts/vN_YYYYMMDD_description.md`

---

## 📁 Directory Map

```
manuscript/
├── OVERVIEW.md              ← START HERE - Master tracking document
├── QUICK_START.md          ← This file
│
├── papers/                  ← Reference PDFs organized by topic
│   ├── transformers/
│   ├── fmri_analysis/
│   ├── pretraining/
│   └── README.md           ← Paper organization guide
│
├── drafts/                  ← All writing drafts
│   └── current_draft.md    ← Work here
│
├── figures/                 ← All visualizations
│   ├── architecture/       ← Model diagrams
│   ├── results/            ← Performance plots
│   └── ablation/           ← Ablation studies
│
├── data/                    ← Supporting data
│   ├── tables/             ← Result tables (CSV)
│   └── statistics/         ← Statistical analysis
│
├── scripts/                 ← Helper scripts
│   └── README.md           ← Script documentation
│
├── supplements/            ← Supplementary materials
│
└── reviews/                ← Review tracking
    └── submission_history.md
```

---

## 🔄 Typical Workflow

### Phase 1: Planning (Week 1-2)
1. ✅ Set up workspace (DONE)
2. Read and organize reference papers
3. Outline narrative in OVERVIEW.md
4. Define figure/table plan

### Phase 2: Results (Week 3-4)
1. Generate all main figures
2. Compile result tables
3. Run statistical tests
4. Create ablation studies

### Phase 3: Writing (Week 5-6)
1. Draft introduction
2. Draft methods
3. Draft results
4. Draft discussion

### Phase 4: Revision (Week 7-8)
1. Internal review
2. Revise based on feedback
3. Polish writing
4. Finalize figures

### Phase 5: Submission (Week 9)
1. Format for venue
2. Final proofreading
3. Submit!

---

## 💡 Tips

### For Writing
- Update OVERVIEW.md section status as you progress
- Keep `current_draft.md` as your active working file
- Version drafts regularly (`v1_YYYYMMDD.md`)
- Use AI agents to read papers: reference PDFs by path

### For Figures
- Create scripts in `scripts/` for reproducibility
- Save raw figures for editing
- Export publication-quality PDFs
- Update OVERVIEW.md figure status

### For References
- Add papers to appropriate `papers/` subdirectory
- Use consistent naming: `FirstAuthor_YYYY_Title.pdf`
- Note key insights in OVERVIEW.md
- Build `references.bib` as you go

### For Collaboration
- Update OVERVIEW.md communication log
- Track decisions in "Notes & Ideas" section
- Use submission_history.md for reviews

---

## 🚀 Next Actions

Based on OVERVIEW.md, your immediate next steps are:

### This Week
- [ ] Upload key reference papers to `papers/`
- [ ] Read 15-20 core papers
- [ ] Generate Figure 3 (main results)
- [ ] Draft methods section

### Next Week
- [ ] Create architecture diagrams
- [ ] Draft introduction
- [ ] Compile all result tables

---

## 🆘 Common Tasks

### Adding a Reference Paper
```bash
# 1. Download PDF
# 2. Rename: FirstAuthor_YYYY_Title.pdf
# 3. Place in appropriate papers/ subdirectory
# 4. Update OVERVIEW.md reference list
```

### Creating a New Figure
```bash
# 1. Create script: scripts/plot_figureN.py
# 2. Generate figure → figures/appropriate_subdir/
# 3. Update OVERVIEW.md figure status
# 4. Reference in current_draft.md
```

### Asking AI to Read a Paper
```
"Read papers/transformers/Liu_2021_SwinTransformer.pdf and summarize
the key architectural innovations relevant to 4D medical imaging"
```

### Checking Progress
```
# Open OVERVIEW.md
# Check "Drafting Progress" table
# Update section status (⬜ → 🟨 → ✅)
# Review weekly goals
```

---

## 📞 Quick Reference

### Important Files
- Mission control: `OVERVIEW.md`
- Active draft: `drafts/current_draft.md`
- Paper organization: `papers/README.md`
- Script guide: `scripts/README.md`

### Folder Purposes
- `papers/` - Read and reference
- `drafts/` - Write and revise
- `figures/` - Visualize and present
- `data/` - Analyze and tabulate
- `scripts/` - Generate and automate
- `supplements/` - Additional materials
- `reviews/` - Track submissions

---

**Remember**: Keep OVERVIEW.md updated - it's your single source of truth!

**Good luck with your manuscript! 📝✨**
