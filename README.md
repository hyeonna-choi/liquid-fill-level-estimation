# Liquid Fill-Level Estimation for Dual-Transparent Labware

> ViT-based liquid fill-level estimation from **multi-view RGB-D**, trained on a fully
> **synthetic Blender pipeline** for dual-transparent laboratory glassware.

🔗 **Project page:** https://hynaaaai.github.io/liquid-fill-level-estimation

<!-- Add a teaser image once available:
![teaser](docs/static/images/teaser.png)
-->

## Overview

Estimating the liquid level inside transparent labware is a core perception step for
autonomous biological experiments. It is hard because **both the container and the liquid
are transparent** and refraction distorts the scene, while manual fill-level annotation does
not scale. We sidestep annotation entirely with a synthetic data pipeline and learn a
multi-view RGB-D estimator.

## Method

1. **Synthetic generation (Blender Python)** — randomized camera poses, HDRI backgrounds,
   labware geometry, and fill levels (1–100%).
2. **Multi-view RGB-D rendering** — paired color + depth with exact ground-truth labels.
3. **ViT estimator** — fuses multi-view RGB-D inputs and regresses the fill level.

## Repository structure

```
.
├── docs/                # GitHub Pages project page (the website)
│   ├── index.html
│   └── static/
├── src/                 # (TODO) data generation + model training code
├── README.md
└── LICENSE
```

## Setup

```bash
# TODO: fill in once code is added
git clone https://github.com/hynaaaai/liquid-fill-level-estimation.git
cd liquid-fill-level-estimation
pip install -r requirements.txt
```

## Status

🚧 Work in progress (2026). Code and dataset release pending institutional review.

## Author

**Hyeonna Choi** — AI Robot Research Institute, KIMM · Jeju National University
· [hynaaaai@gmail.com](mailto:hynaaaai@gmail.com)
