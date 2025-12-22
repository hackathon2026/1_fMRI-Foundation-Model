# Manuscript Workspace Structure

**Created**: 2024-12-22
**Project**: SwiFT_v2 - Self-Supervised 4D Swin Transformer for fMRI Analysis

---

## 📁 Complete Directory Tree

```
manuscript/
│
├── 📄 OVERVIEW.md                    # 📌 MASTER DOCUMENT - Start here!
├── 📄 QUICK_START.md                 # Quick reference guide
├── 📄 STRUCTURE_SUMMARY.md           # This file
│
├── 📚 papers/                         # Reference papers (PDFs)
│   ├── README.md                     # Paper organization guide
│   ├── transformers/                 # Vision transformer papers
│   ├── fmri_analysis/                # Brain imaging DL papers
│   └── pretraining/                  # Self-supervised learning papers
│
├── ✍️  drafts/                        # Writing workspace
│   └── current_draft.md              # Active working draft (template included)
│
├── 📊 figures/                        # All visualizations
│   ├── architecture/                 # Model diagrams (Figure 1)
│   ├── results/                      # Performance plots (Figures 3-4)
│   └── ablation/                     # Ablation studies (Figure 5)
│
├── 📈 data/                           # Supporting data
│   ├── tables/                       # Result tables (CSV format)
│   └── statistics/                   # Statistical test results
│
├── 🔧 scripts/                        # Helper scripts
│   └── README.md                     # Script documentation
│
├── 📎 supplements/                    # Supplementary materials
│
└── 📝 reviews/                        # Submission tracking
    └── submission_history.md         # Review rounds & responses
```

---

## 🎯 Key Files

### Core Documents
| File | Purpose | Update Frequency |
|------|---------|------------------|
| `OVERVIEW.md` | Master tracking, planning, status | Daily/Weekly |
| `QUICK_START.md` | Quick reference guide | Rarely (reference only) |
| `drafts/current_draft.md` | Active manuscript writing | Daily |

### Organization Files
| File | Purpose |
|------|---------|
| `papers/README.md` | Reference paper organization |
| `scripts/README.md` | Script documentation |
| `reviews/submission_history.md` | Review tracking |

---

## 📋 What's in Each Directory

### `/papers/` - Reference Management
**Purpose**: Store and organize reference PDFs for AI agent access

**Subdirectories**:
- `transformers/` - ViT, Swin, Video Transformers
- `fmri_analysis/` - BrainNetCNN, fMRI-specific DL
- `pretraining/` - SimCLR, MAE, SimMIM, BEiT

**Usage**:
1. Upload PDFs with naming: `FirstAuthor_YYYY_Title.pdf`
2. AI can read via: `mcp__pdf-reader-mcp__read_pdf`
3. Track in OVERVIEW.md "Reference Papers" section

---

### `/drafts/` - Writing Workspace
**Purpose**: Version-controlled manuscript drafts

**Key File**: `current_draft.md` - Full paper template with:
- Abstract, Introduction, Methods, Experiments, Results, Discussion
- Section-by-section guidance
- Placeholder text for structure

**Versioning**:
- Save milestones: `v1_20241222_initial.md`
- Track progress in OVERVIEW.md "Drafting Progress" table

---

### `/figures/` - Visualizations
**Purpose**: Organized figure storage by type

**Subdirectories**:
- `architecture/` - Model diagrams, 4D Swin Transformer architecture
- `results/` - Main performance plots, comparisons
- `ablation/` - Ablation study visualizations

**Workflow**:
1. Create generation script in `scripts/`
2. Save outputs to appropriate subdir
3. Update OVERVIEW.md figure status
4. Reference in `current_draft.md`

---

### `/data/` - Supporting Data
**Purpose**: Store experimental results and analyses

**Subdirectories**:
- `tables/` - CSV files with results (main_results.csv, ablation_results.csv)
- `statistics/` - Statistical test outputs, significance tests

**Usage**:
- Source data for figures and tables
- Input to `scripts/` for processing
- Referenced in paper for reproducibility

---

### `/scripts/` - Automation
**Purpose**: Reproducible figure/table generation

**Planned Scripts** (see `scripts/README.md`):
- `generate_figures.py` - Master figure generator
- `compile_results.py` - Aggregate results to tables
- `statistical_tests.py` - Significance testing

---

### `/supplements/` - Supplementary Materials
**Purpose**: Additional materials beyond main paper

**Typical Contents**:
- Extended results
- Additional ablation studies
- Detailed architecture specifications
- Hyperparameter sensitivity analysis

---

### `/reviews/` - Submission Tracking
**Purpose**: Track submission process and reviews

**Key File**: `submission_history.md` - Template for:
- Submission timeline
- Reviewer comments
- Response strategy
- Revision plans

---

## 🔄 Recommended Workflow

### Phase 1: Setup (✅ Complete)
- [x] Create directory structure
- [x] Set up OVERVIEW.md
- [x] Create templates and guides

### Phase 2: Planning (Current)
- [ ] Upload reference papers to `papers/`
- [ ] Update OVERVIEW.md narrative
- [ ] Define figure/table plan
- [ ] Set submission target

### Phase 3: Execution
- [ ] Generate all figures
- [ ] Compile result tables
- [ ] Draft sections
- [ ] Internal review

### Phase 4: Submission
- [ ] Final polish
- [ ] Format for venue
- [ ] Submit!

---

## 💡 Pro Tips

### Keep OVERVIEW.md Updated
✅ Update section status after each writing session
✅ Check off action items as completed
✅ Add new ideas to "Notes & Ideas"
✅ Track weekly progress

### Use AI Agents Effectively
✅ "Read `papers/transformers/Liu_2021_SwinTransformer.pdf` and summarize..."
✅ Reference papers by full path for AI to access PDFs
✅ Ask for comparisons across multiple papers

### Organize as You Go
✅ Name files consistently
✅ Update README files when adding new categories
✅ Version drafts before major changes
✅ Save intermediate analysis results

---

## 📊 Current Status

**Workspace**: ✅ Fully set up and ready
**Next Steps**:
1. Upload reference papers
2. Review OVERVIEW.md and customize
3. Start literature review
4. Generate first figures

**Quick Actions**:
```bash
# View structure
ls -la manuscript/

# Open master document
open manuscript/OVERVIEW.md

# Start writing
open manuscript/drafts/current_draft.md

# Upload a paper
cp /path/to/paper.pdf manuscript/papers/transformers/FirstAuthor_YYYY_Title.pdf
```

---

## 🆘 Need Help?

1. **Start here**: Read `OVERVIEW.md` (comprehensive guide)
2. **Quick reference**: Check `QUICK_START.md`
3. **Paper organization**: See `papers/README.md`
4. **Scripts**: Check `scripts/README.md`

---

**Your manuscript workspace is ready! 🚀**

Begin by customizing `OVERVIEW.md` to match your specific paper goals and timeline.
