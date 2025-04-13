
# Face Age Editing with Fine-Tuned Diffusion Models: A Comparative Study

This project explores the capabilities of diffusion models for **face age editing** — generating realistic, identity-preserving images of individuals at different ages. We aim to fine-tune and evaluate various diffusion-based generative models on high-quality, age-labeled facial datasets to understand their performance and limitations.

## 🎯 Objectives

- Fine-tune multiple diffusion models (e.g., DDPM, Improved-DDPM, DDIM) and pipelines for the task of face age editing.
- Compare architectural differences and their impact on aging realism and accuracy.
- Evaluate performance using metrics like FID, IS, and MAE.

## 🧠 Background

Diffusion models have recently outperformed GANs in generative tasks, particularly in terms of stability and image quality. This project builds on recent advancements like **FADING** and **AgeDiff**, pushing further by experimenting with model architectures and fine-tuning strategies.

## 📊 Datasets

- **CelebA-HQ**: High-quality face images from CelebA  
  [GitHub Link](https://github.com/switchablenorms/CelebAMask-HQ)  
- **FFHQ**: 70K faces with wide demographic variation  
- **FFHQ-Aging**: Age-labeled subset tailored for face aging  
  [GitHub Link](https://github.com/royorel/FFHQ-Aging-Dataset)

## 🔧 Evaluation Metrics

- **FID (Fréchet Inception Distance)** – Realism  
- **IS (Inception Score)** – Quality and diversity  
- **MAE (Mean Absolute Error)** – Age prediction accuracy using a pre-trained age estimator

## 🖥️ Compute & Training

- Fine-tuning will be done on the **CHTC Condor** compute cluster.
- Models: ~100M–150M parameters, 512×512 resolution.
- Training: ~2–3s per batch, 80–100 epochs expected.

## 🤝 Collaboration Plan

Team members contributed equally across:
- Model development  
- Data preprocessing  
- Metric implementation  
- Experimentation and analysis
