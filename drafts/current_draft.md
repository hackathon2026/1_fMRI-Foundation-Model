# SwiFT: Self-Supervised 4D Swin Transformer for Large-Scale fMRI Pre-Training

**Draft Status**: 🚧 Initial Template
**Last Updated**: 2024-12-22
**Version**: 0.1

---

## Abstract

*[200-250 words]*

Background, problem, method, results, impact...

**Keywords**: fMRI analysis, self-supervised learning, transformer, pre-training, transfer learning

---

## 1. Introduction

### 1.1 Motivation

*Paragraph 1: The challenge of fMRI analysis*
- Neuroimaging provides insights into brain function
- Deep learning shows promise but requires large labeled datasets
- Acquiring labels is expensive and expert-dependent
- Gap: How to leverage abundant unlabeled fMRI data?

*Paragraph 2: Opportunity with self-supervised learning*
- Self-supervised pre-training succeeds in NLP and vision
- Unlabeled fMRI data widely available (HCP, UKB, ABCD)
- Spatiotemporal structure can guide pre-training objectives
- Transfer learning can reduce labeling requirements

*Paragraph 3: Technical gap*
- Existing fMRI methods: CNNs, graph networks
- Transformers: successful in vision but not adapted for 4D fMRI
- Need: Architecture that captures spatiotemporal dependencies
- Need: Pre-training strategy suited for brain imaging

### 1.2 Contributions

We present **SwiFT** (Self-supervised Windowed Fourier-based Transformer), a novel framework for fMRI analysis:

1. **4D Swin Transformer architecture** adapted for spatiotemporal fMRI volumes
2. **Self-supervised pre-training** using masked autoencoding on large-scale neuroimaging datasets
3. **Comprehensive evaluation** on HCP, UKB, and ABCD datasets across diverse downstream tasks
4. **Scalable implementation** on Intel XPUs enabling efficient large-scale training

Our experiments demonstrate X% improvement over supervised baselines and effective transfer learning with reduced labeled data requirements.

---

## 2. Related Work

### 2.1 Transformers for Vision

- ViT, Swin Transformer, Video Transformers
- Hierarchical attention, window partitioning
- Scaling properties and inductive biases

### 2.2 Self-Supervised Learning

- Contrastive learning (SimCLR, MoCo)
- Masked prediction (MAE, SimMIM, BEiT)
- Adaptation to different modalities

### 2.3 Deep Learning for fMRI

- 3D CNNs for brain imaging
- Graph neural networks for connectivity
- Recurrent models for temporal dynamics
- Attention mechanisms in neuroimaging

### 2.4 Positioning

*How SwiFT differs from prior work*

---

## 3. Methods

### 3.1 Problem Formulation

**Input**: 4D fMRI volume $X \in \mathbb{R}^{H \times W \times D \times T}$
- Spatial dimensions: $H, W, D$
- Temporal dimension: $T$

**Pre-training objective**: Learn representations from unlabeled data

**Downstream tasks**: Classification and regression with limited labels

### 3.2 4D Swin Transformer Architecture

#### 3.2.1 Overall Architecture

*Describe hierarchical structure*

#### 3.2.2 4D Shifted Window Attention

*Explain spatiotemporal window attention mechanism*

#### 3.2.3 Architecture Variants

*Table of model configurations (small, base, large)*

### 3.3 Self-Supervised Pre-training

#### 3.3.1 Masking Strategy

*Adapt SimMIM for fMRI*
- Random masking ratio
- Brain-specific considerations
- Reconstruction target

#### 3.3.2 Pre-training Objective

*Loss function and optimization*

### 3.4 Transfer Learning

#### 3.4.1 Fine-tuning Strategy

*How to adapt pre-trained model to downstream tasks*

#### 3.4.2 K-Fold Cross-Validation

*Propensity score matching for balanced splits*

---

## 4. Experiments

### 4.1 Datasets

#### 4.1.1 Pre-training Data
- **HCP**: N subjects, task paradigms
- **UKB**: N subjects, demographics
- **ABCD**: N subjects, characteristics

#### 4.1.2 Downstream Tasks
- Classification: Sex, age group, ...
- Regression: Age, cognitive scores, ...

### 4.2 Implementation Details

- **Framework**: PyTorch, PyTorch Lightning, DeepSpeed
- **Hardware**: Aurora supercomputer, Intel XPUs
- **Hyperparameters**: Learning rate, batch size, epochs
- **Optimization**: AdamW, cosine schedule

### 4.3 Baselines

- Supervised-only training
- 3D CNNs
- Vanilla transformers
- Graph neural networks

### 4.4 Evaluation Metrics

- Classification: Accuracy, AUC, AUPRC
- Regression: MAE, MSE, R²
- Statistical testing: Paired t-tests, significance levels

---

## 5. Results

### 5.1 Main Results

*Table 3: Performance across downstream tasks*

Key findings:
- SwiFT achieves X% improvement over supervised baseline
- Transfer learning reduces labeled data requirement by Y%
- Consistent gains across all datasets

### 5.2 Ablation Studies

#### 5.2.1 Architecture Components
- Window size effects
- Model depth and width
- Attention mechanism variants

#### 5.2.2 Pre-training Strategy
- Masking ratio impact
- Pre-training data size
- Pre-training duration

#### 5.2.3 Transfer Learning
- Fine-tuning strategies
- Data efficiency analysis
- Cross-dataset transfer

### 5.3 Visualization and Interpretability

*Figure 6: Attention maps and learned features*

---

## 6. Discussion

### 6.1 Why Does SwiFT Work?

- Spatiotemporal attention captures brain dynamics
- Self-supervised pre-training learns generalizable features
- Transfer learning leverages large-scale unlabeled data

### 6.2 Limitations

- Computational requirements
- Domain specificity
- Interpretability challenges

### 6.3 Future Directions

- Multi-modal pre-training (structural + functional)
- Clinical applications
- Real-time fMRI analysis
- Larger-scale pre-training

### 6.4 Broader Impact

- Democratizing neuroimaging analysis
- Reducing labeling costs
- Enabling discovery in smaller datasets

---

## 7. Conclusion

We presented SwiFT, a self-supervised 4D Swin Transformer for fMRI analysis. Through comprehensive experiments on HCP, UKB, and ABCD datasets, we demonstrated that self-supervised pre-training enables effective transfer learning and achieves state-of-the-art performance on diverse downstream tasks. Our work opens new directions for foundation models in neuroimaging.

---

## Acknowledgments

*Funding, compute resources (Aurora/ALCF), collaborators*

---

## References

*See references.bib*

---

## Supplementary Materials

### A. Additional Architecture Details

### B. Extended Experimental Results

### C. Hyperparameter Sensitivity

### D. Computational Cost Analysis

### E. Qualitative Results

---

**Writing Notes**:
- Keep introduction concise (1.5-2 pages)
- Methods should be reproducible
- Results should be clear and focused
- Discussion should be balanced (strengths + limitations)
- Figures should be self-contained with detailed captions
