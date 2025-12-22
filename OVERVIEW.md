# SwiFT_v2 Manuscript Overview

**Last Updated**: 2024-12-22
**Branch**: final
**Status**: 🚧 Initial Planning

---

## 📄 Paper Metadata

### Working Title
*SwiFT: Self-Supervised 4D Swin Transformer for Large-Scale fMRI Pre-Training*

### Authors
- [ ] Finalize author list
- [ ] Determine author order
- [ ] Confirm affiliations

### Target Venue
- **Primary**: (TBD - e.g., NeurIPS, ICML, Medical Image Analysis)
- **Alternative**: (TBD)
- **Submission Deadline**: (TBD)

---

## 🎯 Current Status

### Timeline
- [ ] **Week 1-2**: Literature review & narrative planning
- [ ] **Week 3-4**: Figure generation & results compilation
- [ ] **Week 5-6**: First draft writing
- [ ] **Week 7-8**: Internal review & revision
- [ ] **Week 9**: Final polish & submission prep

### Drafting Progress
| Section | Status | Notes |
|---------|--------|-------|
| Abstract | ⬜ Not Started | |
| Introduction | ⬜ Not Started | |
| Related Work | ⬜ Not Started | |
| Methods | ⬜ Not Started | |
| Experiments | ⬜ Not Started | |
| Results | ⬜ Not Started | |
| Discussion | ⬜ Not Started | |
| Conclusion | ⬜ Not Started | |
| Supplementary | ⬜ Not Started | |

**Legend**: ⬜ Not Started | 🟨 In Progress | ✅ Complete | 🔄 Under Review

---

## 📖 Paper Narrative

### Story Arc
1. **Problem**: Large-scale fMRI analysis limited by labeled data scarcity
2. **Gap**: Existing methods don't leverage spatiotemporal structure + large unlabeled datasets
3. **Solution**: Self-supervised 4D Swin Transformer pre-training
4. **Evidence**: Strong performance on downstream tasks (HCP, UKB, ABCD)
5. **Impact**: Scalable foundation model for neuroimaging

### Key Message
*Self-supervised pre-training with 4D Swin Transformers enables effective transfer learning for fMRI analysis tasks, achieving state-of-the-art performance across multiple large-scale neuroimaging datasets.*

### Narrative Flow
```
Introduction
├─ Challenge: fMRI analysis requires large labeled datasets
├─ Opportunity: Abundant unlabeled fMRI data available
└─ Contribution: Self-supervised spatiotemporal pre-training

Methods
├─ 4D Swin Transformer architecture
├─ SimMIM-like masking strategy for fMRI
├─ Pre-training on large-scale datasets
└─ Transfer learning to downstream tasks

Experiments
├─ Pre-training datasets: HCP, UKB, ABCD
├─ Downstream tasks: Classification & regression
├─ Baselines: 3D CNNs, vanilla transformers, supervised-only
└─ Ablation studies: Architecture, masking, pre-training data

Results
├─ Performance improvements across all downstream tasks
├─ Transfer learning effectiveness
├─ Scalability to large datasets
└─ Computational efficiency (Intel XPU optimization)

Discussion
├─ Why 4D Swin Transformer works for fMRI
├─ Role of self-supervised pre-training
├─ Limitations & future work
└─ Broader impact for neuroimaging
```

---

## 🔑 Key Contributions

### Primary Contributions
1. **Novel Architecture**: First 4D Swin Transformer for spatiotemporal fMRI analysis
2. **Self-Supervised Pre-training**: SimMIM-adapted masking strategy for brain imaging
3. **Large-Scale Validation**: Comprehensive experiments on HCP, UKB, ABCD datasets
4. **Transfer Learning**: Effective fine-tuning for diverse downstream tasks

### Technical Innovations
- Spatiotemporal window attention for 4D volumes
- Brain-specific masking strategies
- Efficient distributed training on Intel XPUs
- K-fold cross-validation with propensity score matching

### Empirical Findings
- [ ] X% improvement over supervised baseline on task Y
- [ ] Transfer learning reduces required labeled data by Z%
- [ ] Scales to N subjects with M-fold speedup on Aurora

---

## 📊 Figures & Tables Plan

### Main Figures (Target: 6-8 figures)

#### Figure 1: Overview & Architecture
- **Panel A**: Problem illustration (fMRI analysis challenges)
- **Panel B**: SwiFT_v2 pipeline overview
- **Panel C**: 4D Swin Transformer architecture diagram
- **Status**: ⬜ Not Started
- **Location**: `figures/architecture/`

#### Figure 2: Pre-training Strategy
- **Panel A**: SimMIM masking visualization for fMRI
- **Panel B**: Pre-training loss curves
- **Panel C**: Learned representations (t-SNE/UMAP)
- **Status**: ⬜ Not Started
- **Location**: `figures/pretraining/`

#### Figure 3: Downstream Task Performance
- **Panel A**: Classification accuracy across tasks
- **Panel B**: Regression performance (MAE/R²)
- **Panel C**: Comparison with baselines
- **Status**: ⬜ Not Started
- **Location**: `figures/results/`

#### Figure 4: Transfer Learning Analysis
- **Panel A**: Performance vs. pre-training data size
- **Panel B**: Fine-tuning efficiency (data vs. accuracy)
- **Panel C**: Cross-dataset transfer
- **Status**: ⬜ Not Started
- **Location**: `figures/results/`

#### Figure 5: Ablation Studies
- **Panel A**: Architecture variants (window size, depth)
- **Panel B**: Masking strategies
- **Panel C**: Pre-training objectives
- **Status**: ⬜ Not Started
- **Location**: `figures/ablation/`

#### Figure 6: Attention Visualization
- **Panel A**: Spatial attention maps
- **Panel B**: Temporal attention patterns
- **Panel C**: Interpretability analysis
- **Status**: ⬜ Not Started
- **Location**: `figures/interpretability/`

### Main Tables (Target: 3-5 tables)

#### Table 1: Dataset Statistics
- Rows: HCP, UKB, ABCD
- Columns: Subjects, scans, tasks, demographics
- **Status**: ⬜ Not Started
- **Location**: `data/tables/dataset_statistics.csv`

#### Table 2: Architecture Specifications
- Rows: Layers, parameters, FLOPs
- Columns: SwiFT variants
- **Status**: ⬜ Not Started
- **Location**: `data/tables/architecture_specs.csv`

#### Table 3: Main Results
- Rows: Downstream tasks
- Columns: Methods (SwiFT, baselines)
- Metrics: Accuracy, AUC, MAE, R²
- **Status**: ⬜ Not Started
- **Location**: `data/tables/main_results.csv`

#### Table 4: Ablation Results
- Rows: Configuration variants
- Columns: Performance metrics
- **Status**: ⬜ Not Started
- **Location**: `data/tables/ablation_results.csv`

---

## 📚 Reference Papers

### Must-Cite Papers

#### Transformers & Vision Transformers
- [ ] **Attention Is All You Need** (Vaswani et al., 2017) - Original transformer
- [ ] **ViT: An Image is Worth 16x16 Words** (Dosovitskiy et al., 2021) - Vision transformer
- [ ] **Swin Transformer** (Liu et al., 2021) - Hierarchical vision transformer
- [ ] **Video Swin Transformer** (Liu et al., 2022) - 3D extension

#### Self-Supervised Learning
- [ ] **SimCLR** (Chen et al., 2020) - Contrastive learning
- [ ] **MAE** (He et al., 2022) - Masked autoencoding
- [ ] **SimMIM** (Xie et al., 2022) - Simple masked image modeling
- [ ] **BEiT** (Bao et al., 2022) - BERT pre-training for images

#### fMRI Deep Learning
- [ ] **BrainNetCNN** (Kawahara et al., 2017) - Brain connectivity CNN
- [ ] **BrainGB** (Cui et al., 2022) - Graph neural networks for brain
- [ ] **fMRI Transformer** (if exists) - Recent transformer for fMRI
- [ ] **S4 for fMRI** (Recent work) - State space models

#### Medical Imaging Pre-training
- [ ] **MedViT** - Medical imaging transformers
- [ ] **TransUNet** - Transformers for medical segmentation
- [ ] **Self-supervised for Medical** - Domain-specific pre-training

### Paper Categories
Organize PDFs in `papers/` by category:
- `transformers/` - Transformer architectures
- `fmri_analysis/` - fMRI-specific deep learning
- `pretraining/` - Self-supervised learning methods
- `medical_imaging/` - Medical imaging applications
- `neuroscience/` - Domain background

---

## ✅ Action Items

### High Priority (This Week)
- [ ] Finalize target venue and submission deadline
- [ ] Complete literature review (read 15-20 key papers)
- [ ] Generate Figure 3 (main results)
- [ ] Draft methods section (architecture description)
- [ ] Compile all experimental results into tables

### Medium Priority (Next 2 Weeks)
- [ ] Create architecture diagrams (Figure 1C)
- [ ] Run ablation studies if missing
- [ ] Generate attention visualization (Figure 6)
- [ ] Draft introduction (problem + contributions)
- [ ] Draft results section

### Low Priority (Later)
- [ ] Supplementary materials
- [ ] Code release preparation
- [ ] Demo/visualization for website
- [ ] Pre-print submission (arXiv)

### Research Gaps to Address
- [ ] Compare with latest fMRI methods (2023-2024)
- [ ] Statistical significance testing
- [ ] Cross-dataset generalization experiments
- [ ] Computational cost analysis

---

## 📝 Writing Guidelines

### Voice & Style
- **Tense**: Past tense for methods/results, present for contributions
- **Voice**: Active voice preferred
- **Clarity**: Avoid jargon, define domain terms
- **Conciseness**: Aim for 8-10 pages (main paper)

### Target Audience
- ML researchers (70%): Emphasize architecture novelty
- Neuroscience researchers (30%): Emphasize domain impact

### Key Terms to Use Consistently
- "4D Swin Transformer" (not "spatiotemporal transformer")
- "Self-supervised pre-training" (not "unsupervised")
- "Transfer learning" (for downstream tasks)
- "fMRI analysis" (not "neuroimaging" unless broader context)

---

## 👥 Collaboration

### Author Contributions
- [ ] Define contribution categories (CRediT taxonomy)
- [ ] Assign responsibilities

### Communication Log
| Date | Topic | Decisions |
|------|-------|-----------|
| 2024-12-22 | Manuscript workspace setup | Created folder structure |

---

## 💡 Notes & Ideas

### Open Questions
1. Should we emphasize scalability (Aurora) or generalizability (multiple datasets)?
2. How much neuroscience interpretation vs. ML methodology?
3. Include computational cost comparison in main paper or supplement?

### Potential Additions
- [ ] Comparison with state-space models (S4, Mamba)
- [ ] Zero-shot transfer experiments
- [ ] Multi-modal pre-training (T1, fMRI)
- [ ] Clinical application case study

### Reviewer Anticipation
**Likely Questions**:
1. Why 4D Swin over 3D CNNs or vanilla transformers?
2. How does masking strategy affect different brain regions?
3. What is the computational cost trade-off?
4. Does it work for clinical populations?

**Preparation**:
- Strong ablation studies (Figure 5)
- Computational analysis (Table 5 or supplement)
- Discussion of limitations and future work

---

## 📁 File Organization

### Drafts Versioning
- `drafts/v1_YYYYMMDD_initial.md` - First complete draft
- `drafts/v2_YYYYMMDD_revised.md` - Post-review revision
- `drafts/current_draft.md` - Always points to latest

### Figures Naming Convention
- `fig1_overview_vN.pdf` - Main figure files
- `fig1_panel_a_raw.png` - Individual panels
- `fig1_script.py` - Generation script

### Data Files
- `tables/*.csv` - Raw data tables
- `statistics/*.json` - Statistical test results
- `benchmarks/*.json` - Comparison data

---

## 🔗 Quick Links

### Internal Resources
- Main codebase: `/Users/jub/Projects/SwiFT_v2/`
- Downstream results: `/Users/jub/Projects/SwiFT_v2/downstream_optuna/`
- Helper docs: `/Users/jub/Projects/SwiFT_v2/downstream_optuna/helper_documents/`

### External Resources
- Paper templates: (Add conference LaTeX template)
- Style guide: (Add venue-specific guidelines)
- Shared drive: (Add collaborative workspace link)

---

## 📈 Progress Tracking

### Weekly Goals
**Week of 2024-12-22**:
- [x] Create manuscript workspace
- [ ] Complete literature review
- [ ] Generate main results figure
- [ ] Draft methods section

**Week of 2024-12-29**:
- [ ] Complete all figures
- [ ] Draft introduction & results
- [ ] Internal review round 1

### Milestones
- [ ] **Milestone 1**: All figures complete (Target: TBD)
- [ ] **Milestone 2**: First full draft (Target: TBD)
- [ ] **Milestone 3**: Internal review complete (Target: TBD)
- [ ] **Milestone 4**: Submission ready (Target: TBD)

---

## 🎓 Citation Management

### BibTeX Organization
- Create `references.bib` with categories:
  - `@transformers` - Architecture papers
  - `@pretraining` - Self-supervised methods
  - `@fmri` - Domain papers
  - `@datasets` - HCP, UKB, ABCD citations

### Citation Tracking
- [ ] Set up Zotero/Mendeley/BibTeX management
- [ ] Export bibliography from papers folder
- [ ] Sync with collaborative workspace

---

**End of Overview**

*This document is living and should be updated regularly as the manuscript progresses.*
