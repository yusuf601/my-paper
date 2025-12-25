# Segmentation of Provinces Prone to Food Crises Based on Commodity Price Volatility Patterns Using Fuzzy C-Means Clustering

> A data-driven approach to identify provincial vulnerability to food price instability using fuzzy clustering on time series commodity price data

[![Build LaTeX](https://github.com/yusuf601/my-paper/actions/workflows/latex_ci.yml/badge.svg)](https://github.com/yusuf601/my-paper/actions)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## Overview

This research addresses food security challenges in Indonesia by analyzing price volatility patterns of strategic food commodities across 34 provinces. Using daily price time series data from 11 essential commodities (rice, chili, garlic, onion, cooking oil, sugar, beef, chicken, eggs, and wheat flour), we apply Fuzzy C-Means (FCM) clustering to identify regional vulnerability to food price instability.

The study extracts five key statistical features from time series data—mean price, coefficient of variation (volatility), trend, autocorrelation, and skewness—to characterize price dynamics across regions. Unlike traditional hard clustering methods, FCM allows provinces to belong to multiple clusters with varying membership degrees, effectively capturing the uncertainty and gradual transitions between different risk levels.

Key findings reveal significant heterogeneity in food price instability risk across Indonesian provinces, which can be categorized into low and high-risk clusters. Results show that provinces in Java Island consistently exhibit higher price volatility, while Kalimantan provinces demonstrate more stable price patterns. This volatility-based analysis provides an alternative perspective for food security assessment and supports more targeted regional policies for price stabilization and food crisis mitigation.

**Research Objectives:**
- Segment 34 Indonesian provinces based on food commodity price volatility patterns
- Identify provinces with high price volatility indicating vulnerability to food crises  

**Keywords:** food price volatility, fuzzy C-means, time series analysis, regional cllustering,food security

## Download PDF

You can download the compiled PDF without building locally:

1. Navigate to the [**Actions**](https://github.com/yusuf601/my-paper/actions) tab
2. Click on the **latest successful workflow run** (marked with ✓)
3. Scroll to the **Artifacts** section
4. Click on **`paper-pdf`** to download

> **Note:** Only successful workflow runs (green checkmark ✓) will have the PDF artifact available.

## Build Locally

### Prerequisites

This paper requires a full LaTeX distribution. Install using:

**Debian/Ubuntu:**
```bash
sudo apt install texlive-full
```

**Arch Linux:**
```bash
sudo pacman -S texlive-full
```

**macOS (with Homebrew):**
```bash
brew install --cask mactex
```

### Compilation

1. Clone the repository:
   ```bash
   git clone https://github.com/yusuf601/my-paper.git
   cd repo-name
   ```

2. Compile the LaTeX document:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

   Or use latexmk for automatic compilation:
   ```bash
   latexmk -pdf main.tex
   ```

## Repository Structure

```bash
.
├── dbi_pc.png #metrick evaluation
├── final_AI.zip #source from overleaf
├── final_paper 
├── final_paper.tex #source code paper
├── flowchart.jpg #flow research image
├── heatmap_feature.png #feature correlation heatmap visualization
├── heatmap_missing correlation.png #missing value correlation visualization
├── heatmap_missing_correlation.png #missing value correlation visualization
├── LICENSE #license MIT
├── lofi.png #lofi(trash)
├── membership_distribution.png #membershio distribution visualization
├── overlap_missing_days.png #overlap missing value visualization
├── peta_cluster.png #result choropleth map
└── readme.md #this file
```

## Citation

If you use this work, please cite:

```
@article{Muh Yusuf,
  title={Segmentasi Provinsi Rawan Krisis Pangan Berdasarkan Pola \textit{Volatilitas} Harga Komoditas Menggunakan},
  author={Muh Yusuf},
  journal={Jurnal Teknik Informatika dan Sistem Informasi (JuTISI)},
  year={2025},
  url={https://github.com/yusuf601/my-paper}
}
```

## License

This work is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.

## Contact

- **Author:** Muh Yusuf
- **Email:** yusuf@uho.edu
- **Institution:** Universitas HaluOleo

## Acknowledgments

Add acknowledgments here (funding sources, advisors, contributors, etc.).

---

**Last updated:** December 2025
```
