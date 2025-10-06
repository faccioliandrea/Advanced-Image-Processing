# 🧠 Advanced Image Processing — Lab Sessions

This repository contains the laboratory exercises developed for the **Advanced Image Processing (DTA095A)** course.  
Each lab explores key concepts in image degradation, restoration, and modern optimization-based and deep-learning methods for inverse problems in imaging.

---

## 📘 Lab Overview

| Lab | Title | Topics | Status |
|------|-------|---------|---------|
| **Lab 1** | Noise & Spatial Filters / Deblurring: Inverse and Wiener | Noise modeling, spatial filtering, frequency-domain deblurring | ✅ Completed |
| **Lab 2** | ISTA Deblurring & ADMM Inpainting | Sparsity priors, Plug-and-Play, DRUNet integration | ✅ Completed |
| **Lab 3** | *(To be released)* | TBD | 🚧 Upcoming |

---

## 🧩 Lab 1 — Noise & Spatial Filters / Deblurring: Inverse and Wiener

### 🔍 Overview
This session investigates the effects of various noise types and filtering techniques on image quality, alongside classical deblurring using **Inverse** and **Wiener filters**.  
It highlights trade-offs between noise suppression and detail preservation under different degradation models.

### 🧪 Key Topics
- Noise models: AWGN, Poisson, Speckle, Salt-and-Pepper  
- Spatial domain filtering: Mean, Median, Bilateral, Bicubic  
- Frequency domain restoration: Inverse & Wiener filtering  
- Evaluation metrics: **PSNR**, **LPIPS**, and perceptual analysis  

### 📈 Findings
- Median filtering excels against impulse (salt-and-pepper) noise.  
- Wiener filtering achieves the best balance between noise control and deblurring robustness.  
- Inverse filtering is highly sensitive to noise amplification.  

---

## 🧠 Lab 2 — ISTA Deblurring / ADMM Inpainting

### 🔍 Overview
This lab focuses on **optimization-based** and **Plug-and-Play** restoration methods, exploring how different sparsity priors and regularizers affect image quality and convergence.  
Experiments include **ISTA** (Iterative Shrinkage-Thresholding Algorithm) in both pixel and wavelet domains, and **ADMM** for inpainting with both explicit and learned priors.

### 🧪 Key Topics
- **ISTA deblurring** with pixel vs. wavelet-domain sparsity  
- **ADMM-based inpainting** using:  
  - Total Variation (TV)  
  - Tikhonov regularization (identity & gradient)  
  - Learned priors (DRUNet Plug-and-Play)  
- Hyperparameter effects (λ, J, shrinkage strategies)  
- Quantitative evaluation via **PSNR** and **LPIPS**

### 📈 Findings
- Wavelet-domain ISTA provides superior robustness under high noise.  
- Decomposition depth `J` significantly affects denoising performance.  
- Plug-and-Play ADMM with DRUNet achieves best overall fidelity and perceptual quality.  
- DRUNet converges slower but outperforms classical regularizers.

---

## 🧭 Lab 3 — *To Be Released*

> 🔒 **Coming soon!**  

---

## ⚙️ Environment & Dependencies

All labs are implemented in **Python** using Jupyter Notebooks.

### Main libraries
```bash
numpy
torch
scikit-image
matplotlib
pywavelets
deepinv
