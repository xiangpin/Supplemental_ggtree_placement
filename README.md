<!-- README.md is generated from README.Rmd. Please edit that file -->

# Scalable method for exploring phylogenetic placement uncertainty with custom visualizations using treeio and ggtree

If you use this work in published research, please cite:

Scalable method for exploring phylogenetic placement uncertainty with
custom visualizations using treeio and ggtree

This repo contains source code and data to produce Supplementary
Material of the above paper.

<https://github.com/YuLab-SMU/Supplemental_ggtree_placement>

## 1. `exampledata`

This directory contains example input data files for phylogenetic
analysis and tree placements.

### `Holomycota`:

Contains jplace and CSV files related to the Holomycota dataset.

- **`HolomycotaV4_alignedtrim.jplace`**: Placement file for the
  Holomycota phylogenetic analysis.
- **`V4_group.csv`**: Associated metadata for the groups in the
  Holomycota dataset.

### `Mitsi`:

Contains files from the Mitsi dataset.

- **`rsbl20190182supp2.jplace`**: Placement file for the Mitsi dataset.
- **`rsbl20190182supp7.tre`**: Tree file corresponding to the placement
  data.

### `subtree`:

Contains data for a specific subtree analysis.

- **`Amt_tiplabel.csv`**: Tip label information for the Amt subtree.
- **`pplacer_Amt_subtree.jplace`**: Placement file for the Amt subtree
  analysis.

------------------------------------------------------------------------

## 2. `pdf`

This directory contains PDF files of the figures generated from the
analysis.

- **`Fig1.pdf`**Workflow diagram of treeio and ggtree in processing
  phylogenetic placement data, **`Fig2.pdf`**,
  **`Fig3.pdf`**,**`Fig4.pdf`**: Figures representing various
  visualizations of the phylogenetic analysis.
  **`FigS1.pdf`**:Supplementary figure showing detailed performance
  evaluations of treeio, including runtime and memory efficiency when
  processing large phylogenetic trees with diverse placement scenarios.

------------------------------------------------------------------------

## 3. `Rmarkdown`

This directory contains an R Markdown file used for generating the
supplementary files for the project.

- **`header.tex`**: LaTeX header for formatting the supplementary file.
- **`supplementary_filev2.Rmd`**: R Markdown source file for generating
  the supplementary file.
- **`supplementary_filev2.pdf`**: PDF version of the supplementary file.

------------------------------------------------------------------------

## 4. `tiff`

This directory contains TIFF versions of the figures for high-quality
image export.

- **`Fig2.tiff`**, **`Fig3.tiff`**, **`Fig4.tiff`**: High-resolution
  images of the figures in TIFF format.

------------------------------------------------------------------------

## 5. `simulated_data`

This directory contains files and scripts for simulated data analysis.

- **`scripts`**  
  Contains R scripts for generating and visualizing simulated data:
  - **`plot_simulated_jplace.R.r`**: Script for visualizing simulated
    `.jplace` files.  
  - **`run_simulate_jplace.R`**: Script for generating simulated
    `.jplace` data.
- **`simulated_jplace`**  
  Contains simulated `.jplace` files with different configurations:
  - **`simulate_tips100000_placement_nrow_1000000.jplace`**  
  - **`simulate_tips100000_placement_nrow_100000.jplace`**  
  - **`simulate_tips100000_placement_nrow_10000.jplace`**  
  - **`simulate_tips100000_placement_nrow_1000.jplace`**  
  - (and others with similar naming patterns).
- **`src`**  
  Contains alternative versions of scripts for generating and
  visualizing simulated data:
  - **`plot_simulated_jplace.R.r`**  
  - **`run_simulate_jplace.R`**
- **Other Files**  
  Test `.jplace` files with different sample sizes and row
  configurations for validation:
  - **`test_jp_1k_1kp.jplace`**, **`test_jp_1k_10kp.jplace`**,
    **`test_jp_1k_100kp.jplace`**, **`test_jp_1k_1000kp.jplace`**  
  - **`test_jp_10k_1kp.jplace`**, **`test_jp_10k_10kp.jplace`**,
    **`test_jp_10k_100kp.jplace`**, **`test_jp_10k_1000kp.jplace`**  
  - **`test_jp_50k_1kp.jplace`**, **`test_jp_50k_10kp.jplace`**,
    **`test_jp_50k_50kp.jplace`**, **`test_jp_50k_100kp.jplace`**  
  - **`test_jp_100k_1kp.jplace`**, **`test_jp_100k_10kp.jplace`**,
    **`test_jp_100k_50kp.jplace`**, **`test_jp_100k_100kp.jplace`**  
  - (and others with similar naming patterns).

------------------------------------------------------------------------

## Usage

- The `exampledata` directory contains the input data files used in the
  analysis.
- Figures are stored in both PDF and TIFF formats for use in
  publications or presentations.
- The `Rmarkdown` directory contains the source file for generating the
  supplementary materials, which can be edited or recompiled if needed.

------------------------------------------------------------------------

## Requirements

To reproduce the figures and analyses, you will need:

- **R** with necessary packages such as `ggtree`, `treeio`, `dplyr`, and
  `ggplot2`.
- **LaTeX** for compiling the R Markdown file to PDF.
