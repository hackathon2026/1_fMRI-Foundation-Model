# Manuscript Scripts

Helper scripts for generating figures, tables, and analyses for the manuscript.

## Contents

### Figure Generation
- `generate_figures.py` - Master script for all figures
- `plot_architecture.py` - Architecture diagrams (Figure 1)
- `plot_results.py` - Performance plots (Figures 3-4)
- `plot_attention.py` - Attention visualizations (Figure 6)

### Data Processing
- `compile_results.py` - Aggregate experimental results into tables
- `statistical_tests.py` - Perform significance testing
- `format_tables.py` - Convert raw data to LaTeX tables

### Analysis
- `ablation_analysis.py` - Ablation study analysis
- `compute_metrics.py` - Calculate all evaluation metrics
- `cross_dataset_analysis.py` - Transfer learning analysis

## Usage

### Generate All Figures
```bash
python generate_figures.py --results_dir ../data/ --output_dir ../figures/
```

### Create Results Tables
```bash
python compile_results.py --input ../data/tables/ --output main_results.tex
```

### Run Statistical Tests
```bash
python statistical_tests.py --baseline supervised --method swift
```

## Dependencies

See main project requirements. Key packages:
- matplotlib, seaborn (plotting)
- pandas, numpy (data processing)
- scipy, statsmodels (statistics)
- plotly (interactive visualizations)

## Output Organization

- Figures → `../figures/`
- Tables → `../data/tables/`
- Statistics → `../data/statistics/`

## Notes

- All scripts should be reproducible with fixed random seeds
- Save intermediate results for debugging
- Include documentation for complex analyses
- Use configuration files for styling consistency
