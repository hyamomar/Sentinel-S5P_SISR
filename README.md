# Depth Separable Architecture for Sentinel-5P Super-Resolution

**Authors:**  
Hyam Omar Ali¹ ², Romain Abraham¹, Bruno Galerne¹ ³  

**Affiliations:**  
¹ Institut Denis Poisson, Université d’Orléans, Université de Tours, CNRS, France  
² Faculty of Mathematical Sciences, University of Khartoum, Sudan  
³ Institut Universitaire de France (IUF)

---

## Overview

This repository contains the implementation of the S5-DSCR model, a super-resolution approach for enhancing the spatial resolution of Sentinel-5P hyperspectral images using Depth Separable Convolution.

---

## Objectives

- Improve the spatial resolution of S5P data.
- Use DSC architecture to capture spatial and spectral features.
- Train separate models for each spectral band.

---

## Dataset

- Hyperspectral images from 15 S5P orbits.
- 8 spectral bands, ~500 channels each.
- Covers diverse spatial and spectral characteristics.

---

## Methodology

- Uses Depth Separable Convolution (DSC) for lightweight, efficient modeling.
- Applies per-band training to address spectral differences.
- Captures both spatial and inter-channel correlations.

---

## Results

- Outperforms existing SR methods for most spectral bands.
- Delivers sharper, more detailed spatial reconstructions.
- Enhances the usability of S5P data for atmospheric analysis.

---

## Citation

If you use this code, please cite:

```bibtex
@article{ali2025depth,
  title={Depth Separable Architecture for Sentinel-5P Super-Resolution},
  author={Ali, Hyam Omar and Abraham, Romain and Galerne, Bruno},
  journal={Preprint},
  year={2025}
}
