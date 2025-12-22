# Reference Papers

This directory contains PDF files of key reference papers for the SwiFT_v2 manuscript.

## Organization

Papers are organized into subdirectories by topic:

### `/transformers/`
Vision transformer and attention mechanism papers:
- Original Transformer (Vaswani et al., 2017)
- Vision Transformer (Dosovitskiy et al., 2021)
- Swin Transformer (Liu et al., 2021)
- Video Swin Transformer (Liu et al., 2022)

### `/fmri_analysis/`
Deep learning for fMRI analysis:
- BrainNetCNN and connectivity models
- Graph neural networks for brain imaging
- Recent transformer applications to neuroimaging
- State-space models for fMRI

### `/pretraining/`
Self-supervised and pre-training methods:
- SimCLR, MoCo (contrastive learning)
- MAE, SimMIM (masked autoencoding)
- BEiT (BERT for images)
- Domain-specific pre-training strategies

### `/medical_imaging/` (Optional)
Medical imaging transformers and applications:
- MedViT, TransUNet
- Self-supervised for medical imaging
- Domain adaptation techniques

### `/neuroscience/` (Optional)
Domain background and neuroscience papers:
- fMRI methodology
- Brain network analysis
- Neuroimaging datasets (HCP, UKB, ABCD)

## File Naming Convention

Use descriptive names with author and year:
```
FirstAuthor_YYYY_ShortTitle.pdf
```

Examples:
- `Liu_2021_SwinTransformer.pdf`
- `Xie_2022_SimMIM.pdf`
- `Dosovitskiy_2021_VisionTransformer.pdf`

## AI Agent Access

All PDFs in this directory are accessible to AI agents via the `mcp__pdf-reader-mcp__read_pdf` tool for:
- Content extraction
- Citation information
- Key methodology review
- Figure/table analysis

## Bibliography Management

- Export citations to `../references.bib` for LaTeX
- Use consistent citation keys: `firstauthor:year:keyword`
- Track papers in OVERVIEW.md under "Reference Papers" section

## Usage Notes

- Keep only essential papers (aim for 20-30 core references)
- Archive less relevant papers separately
- Update OVERVIEW.md when adding new papers
- Note key insights/quotes in paper annotations or separate notes file
