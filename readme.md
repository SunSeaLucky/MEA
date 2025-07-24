<div align="center">
<h1> Uncovering and Mitigating Destructive Multi-Embedding Attacks in Deepfake Proactive Forensics </h1>
</div>

## ⭐ Abstract

With the rapid evolution of deepfake technologies and the wide dissemination of digital media, personal privacy is facing increasingly serious security threats. Deepfake proactive forensics, which involves embedding imperceptible watermarks to enable reliable source tracking, serves as a crucial defense against these threats. Although existing methods show strong forensic ability, they rely on an idealized assumption of single watermark embedding, which proves impractical in real-world scenarios. In this paper, we formally define and demonstrate the existence of Multi-Embedding Attacks (MEA) for the first time. When a previously protected image undergoes additional rounds of watermark embedding, the original forensic watermark can be destroyed or removed, rendering the entire proactive forensic mechanism ineffective. To address this vulnerability, we propose a general training paradigm named Adversarial Interference Simulation (AIS). Rather than modifying the network architecture, AIS explicitly simulates MEA scenarios during fine-tuning and introduces a resilience-driven loss function to enforce the learning of sparse and stable watermark representations. Our method enables the model to maintain the ability to extract the original watermark correctly even after a second embedding. Extensive experiments demonstrate that our plug-and-play AIS training paradigm significantly enhances the robustness of various existing methods against MEA.
## 🚀 Introduction

<div align="center">
    <img width="600" alt="image" src="figures/introduction.png?raw=true">
</div>


Illustration of the ideal proactive forensics pipeline and the threat posed by Multi-Embedding Attacks (MEA). (a) In the standard pipeline, the embedded forensic watermark is expected to withstand manipulations such as deepfake generation. (b) However, additional watermark embeddings by third parties (e.g., social media platforms or malicious actors) can overwrite and degrade the original watermark, leading to a complete failure of the proactive forensics mechanism.

## 📻 Overview

<div align="center">
    <img width="1000" alt="image" src="figures/method.png?raw=true">
</div>

<div align="center">
Overview of the proposed framework. </div>

## 📆 TODO LIST
Our complete codebase will be released upon paper acceptance.
- [x] [2025.7.24] Release the project page.
- [x] [2025.7.24] Release instructions for dataset preparation.
- [ ] Release the complete model code.
- [ ] Release the training and inference code.
- [ ] Release the pretrained model.

## 🎮 Getting Started

### 1. Install Environment

`python -m pip install -r requirements.txt`

### 2. Dataset Preparation

- We used several public deepfake datasets, as shown in the following table. You can enter the dataset website to download the original data.

### 3. Train

Upon Acceptance -> Codebase Liberation Activated 🔓

### 4. Test

Upon Acceptance -> Codebase Liberation Activated 🔓

### 5. Pretrained Model
Upon Acceptance, we will provide the pretrained model. 

## 🖼️ Visualization

<div align="center">
<img width="600" alt="image" src="figures/visualization.png?raw=true">
</div>

<div align="center">
Visual effects of the manipulations on the watermarked images.
</div>

## ✨ Quantitative comparison

<div align="center">
    <img width="1000" alt="image" src="figures/table.png?raw=true">
</div>

<div align="center">
Robustness Evaluation: Resisting Intra-model MEA
</div>

