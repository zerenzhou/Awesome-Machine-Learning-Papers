# Computer Vision (CV)

A collection of must-read computer vision papers from top venues.

## Tech Tree

```mermaid
graph TD
    classDef cls fill:#DBEAFE,stroke:#2563EB
    classDef det fill:#D1FAE5,stroke:#059669
    classDef vit fill:#FED7AA,stroke:#EA580C
    classDef gen fill:#E9D5FF,stroke:#7C3AED
    classDef star fill:#FFD700,stroke:#B8860B

    LeNet["LeNet (1998)"]:::cls --> AlexNet["⭐ AlexNet (2012)"]:::star
    AlexNet --> VGG["VGG (2014)"]:::cls
    AlexNet --> GoogLeNet["Inception (2015)"]:::cls
    VGG --> ResNet["⭐ ResNet (2016)"]:::star
    ResNet --> DenseNet["DenseNet (2017)"]:::cls
    ResNet --> EfficientNet["EfficientNet (2019)"]:::cls

    AlexNet -.-> RCNN["R-CNN (2014)"]:::det
    RCNN --> FastRCNN["Fast R-CNN (2015)"]:::det
    FastRCNN --> FasterRCNN["⭐ Faster R-CNN (2015)"]:::star
    FasterRCNN --> FPN["FPN (2017)"]:::det
    RCNN --> YOLO["YOLO (2016)"]:::det

    ResNet -.-> ViT["⭐ ViT (2021)"]:::star
    ViT --> SwinT["Swin Transformer (2021)"]:::vit
    ViT --> MAE["MAE (2022)"]:::vit

    GAN["⭐ GAN (2014)"]:::star --> DCGAN["DCGAN (2016)"]:::gen
    DCGAN --> StyleGAN["StyleGAN (2019)"]:::gen
    GAN --> Pix2Pix["Pix2Pix (2017)"]:::gen
    GAN -.-> Diffusion["DDPM (2020)"]:::gen
    Diffusion --> LatentDiff["Latent Diffusion (2022)"]:::gen
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Image Classification](https://img.shields.io/badge/Image_Classification-DBEAFE?style=flat-square) | CNN backbone architectures for visual feature extraction, from AlexNet's breakthrough to efficient modern designs |
| ![Object Detection](https://img.shields.io/badge/Object_Detection-D1FAE5?style=flat-square) | Region-based and single-shot detectors that locate and classify objects in images |
| ![Vision Transformer](https://img.shields.io/badge/Vision_Transformer-FED7AA?style=flat-square) | Attention-based architectures replacing or augmenting CNN feature extraction for visual understanding |
| ![Generative Models](https://img.shields.io/badge/Generative_Models-E9D5FF?style=flat-square) | Image synthesis methods from adversarial training (GAN) to denoising diffusion processes |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2024](2024.md)
- [2023](2023.md)
- [2022](2022.md)
- [2021](2021.md)
- [2017](2017.md)
- [2016](2016.md)
