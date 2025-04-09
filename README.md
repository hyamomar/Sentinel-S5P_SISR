# Depth Separable Architecture for Sentinel-5P Super-Resolution

Hyam Omar Ali¹ ², Romain Abraham¹, Bruno Galerne¹ ³  

¹ Institut Denis Poisson, Université d’Orléans, Université de Tours, CNRS, France  
² Faculty of Mathematical Sciences, University of Khartoum, Sudan  
³ Institut Universitaire de France (IUF)

---

## Overview

This repository contains the implementation of the S5-DSCR model, a novel super-resolution (SR) approach designed to enhance the spatial resolution of Sentinel-5 Precursor (S5P) satellite data. The S5P satellite provides extensive hyperspectral (HS) images across eight spectral bands, each containing approximately 500 channels. The S5-DSCR model leverages Depth Separable Convolution (DSC) architecture to effectively exploit cross-channel correlations, thereby improving the spatial resolution of S5P data

---

## Objectives

- Improve the spatial resolution of S5P data by addressing the physical limitations of S5P's spatial resolution by applying advanced SR techniques.
- Use DSC architecture to exploit spatial and spectral relationships within hyperspectral images.
- Train the model separately for each of the eight spectral bands of S5P data to account for their unique spectral characteristics.

---

## Dataset

- Hyperspectral images from 15 S5P orbits.
- 8 spectral bands, ~500 channels each.
- Covers diverse spatial and spectral characteristics.
- The dataset comprises hyperspectral images collected from 15 distinct S5P orbits, representing diverse spatial and spectral characteristics to provide comprehensive coverage of Earth's surface. Each spectral band contains approximately 500 channels, offering rich spectral information for SR processing.
- The dataset comprises HS images from 15 different orbits of the S5P satellite, representing diverse spatial and spectral characteristics to ensure comprehensive coverage of Earth's surface. Each spectral band contains around 500 channels, providing a rich dataset for model training and evaluation.

---

## Methodology

The S5-DSCR model employs DSC architecture to perform spatial super-resolution by effectively capturing interdependencies across all spectral channels while reducing computational complexity. We coupled DSC with residual connections to enhance feature extraction and stability.

---

## Results

- Outperforms existing SR methods for most spectral bands.
- Delivers sharper, more detailed spatial reconstructions.
- Enhances the usability of S5P data for atmospheric analysis.
- Quantitative evaluations demonstrate that the S5-DSCR model outperforms existing methods in enhancing the spatial resolution of S5P data for the majority of spectral bands. The model successfully captures fine details necessary for precise analysis, thereby advancing capabilities in air quality monitoring and remote sensing applications.
- Quantitative evaluations demonstrate that the S5-DSCR model outperforms existing super-resolution methods across the majority of spectral bands. The use of DSC architecture enables the model to capture fine details necessary for precise analysis, paving the way for advancements in air quality monitoring and remote sensing applications
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
