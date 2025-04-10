# Depth Separable Architecture for Sentinel-5P Super-Resolution

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




![Alt text](images/architecture.png)
<p align="center"><em>Figure 1: Architecture of S5-DSCR (L=5) and S5-DSCR-S (L=1) models</em></p>



![Alt text](images/DSC.png)
<p align="center"><em>Figure 2: DSC module</em></p>



---

## Results

![Alt text](images/BD3.png)
![Alt text](images/BD5.png)
![Alt text](images/BD7.png)
<p align="center"><em>Figure 3: SR results of S5-DSCR model for, from top to bottom,  bands 3, 5 and 7, with, from left to right, LR, ground truth HR, and our result. For visualization, each image is displayed in the first three PCA components of the ground truth</em></p>


---

## Citation

If you use this code, please cite:

```bibtex
@article{ali2025depth,
  title={Depth Separable architecture for Sentinel-5P Super-Resolution},
  author={Ali, Hyam Omar and Abraham, Romain and Galerne, Bruno},
  journal={arXiv preprint arXiv:2501.17210},
  year={2025}
}
