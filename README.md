# Brain-Conditioned Visual Reconstruction using EEG Signals

## Overview

This project focuses on reconstructing visual information from EEG (Electroencephalography) signals using a deep learning framework. The model learns meaningful brain representations through multi-branch feature extraction and latent space learning, followed by image reconstruction.

---

## Project Workflow

```
EEG Dataset (.pth)
        │
        ▼
Preprocessing
        │
        ▼
Feature Extraction
 ├── Temporal Features
 ├── Spatial Features
 └── Channel Attention Features
        │
        ▼
Feature Fusion
        │
        ▼
Encoder
        │
        ▼
Latent Space Representation
        │
        ▼
Swin Denoising Diffusion
        │
        ▼
Decoder
        │
        ▼
Image Reconstruction
        │
        ▼
Performance Evaluation
```

---

## Dataset

- EEG Dataset (.pth format)
- Tiny ImageNet (Target Images)

---

## Preprocessing

The following preprocessing steps were performed:

- Loading EEG dataset
- Missing value checking
- Data normalization
- Butterworth Bandpass Filtering
- Artifact removal
- Short-Time Fourier Transform (STFT)
- Wavelet Transform

---

## Feature Extraction

The model extracts three complementary EEG representations:

- Temporal Features
- Spatial Features
- Channel Attention Features

These features are fused to obtain a comprehensive representation of brain activity.

---

## Model Architecture

- Multi-Branch GRU Encoder
- Feature Fusion
- Latent Space Representation (256-Dimensional)
- Swin Denoising Diffusion Module
- Decoder for Image Reconstruction

---

## Visualization

The learned representations are visualized using:

- t-SNE of Temporal Features
- t-SNE of Spatial Features
- t-SNE of Channel Features
- t-SNE of Fused Features
- t-SNE of Latent Space

---

## Performance Evaluation

The reconstructed images will be evaluated using:

- Cosine Similarity
- Mean Squared Error (MSE)
- Structural Similarity Index (SSIM)
- Peak Signal-to-Noise Ratio (PSNR)

---

## Technologies Used

- Python
- PyTorch
- NumPy
- Scikit-learn
- MNE
- Matplotlib
- OpenCV
- Tiny ImageNet

---

## Project Status

✔ EEG Preprocessing Completed

✔ Multi-Branch Feature Extraction Completed

✔ Feature Fusion Completed

✔ Latent Space Representation Completed

✔ Feature Visualization Completed

🔄 Swin Denoising Diffusion (In Progress)

🔄 Decoder Training (In Progress)

🔄 Image Reconstruction (In Progress)

🔄 Performance Evaluation (Pending)

---



