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
