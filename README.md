# Synthetic Data Generation for Skin Disease Classification

## Overview

This project explores the use of Generative AI and deep learning models to generate synthetic
skin-disease images and investigate their usefulness for downstream disease classification.

The project compares multiple generative approaches:

- Variational Autoencoder (VAE)
- Deep Convolutional GAN (DCGAN)
- Diffusion Models

A Vision Transformer (ViT) is used for image classification.

---

## Problem

Medical image datasets can be limited in size and diversity.

This project investigates whether synthetic images generated using modern generative models can
provide additional data for training and evaluating a skin-disease classification system.

---

## Approach

```text
Skin Disease Dataset
        │
        ├──────────────┐
        ↓              ↓
       VAE           DCGAN
        │              │
        └──────┬───────┘
               │
               ↓
         Diffusion Model
               │
               ↓
       Synthetic Images
               │
               ↓
       Vision Transformer
               │
               ↓
      Disease Classification
```
---
## Models

### 1. Variational Autoencoder (VAE)

Used to learn a latent representation of skin-disease images and generate new samples.

### 2. Deep Convolutional GAN (DCGAN)

Used to generate synthetic skin-disease images through adversarial training.

### 3. Diffusion Model

Used to generate synthetic images through an iterative denoising process.

### 4. Vision Transformer (ViT)

Used for downstream image classification and evaluation.

---

## Dataset

The project uses the **HAM10000 skin lesion dataset**.

The dataset contains dermatoscopic images of different skin-lesion categories and is used as the
basis for the synthetic data generation and classification experiments.

---

## Technologies

- Python
- Deep Learning
- Generative AI
- VAE
- DCGAN
- Diffusion Models
- Vision Transformers
- Computer Vision
- Medical Image Processing

---

## Project Structure

```text
.
├── DCGAN_.ipynb
├── Diffusion_.ipynb
├── VAE_PEC.ipynb
├── vit_.ipynb
├── Gen AI_Report - Copy.pdf
├── Synthetic_data_generation_ppt.pdf
└── README.md
