# Computer Vision (CV)

A collection of must-read computer vision papers from top venues.

## Tech Tree

```mermaid
graph TD
    subgraph CNN Era
        LeNet["LeNet (1998)"] --> AlexNet["⭐ AlexNet (2012)"]
        AlexNet --> VGG["VGG (2014)"]
        AlexNet --> GoogLeNet["Inception (2015)"]
        VGG --> ResNet["⭐ ResNet (2016)"]
        ResNet --> DenseNet["DenseNet (2017)"]
        ResNet --> EfficientNet["EfficientNet (2019)"]
    end

    subgraph Object Detection
        AlexNet --> RCNN["R-CNN (2014)"]
        RCNN --> FastRCNN["Fast R-CNN (2015)"]
        FastRCNN --> FasterRCNN["⭐ Faster R-CNN (2015)"]
        FasterRCNN --> FPN["FPN (2017)"]
        RCNN --> YOLO["YOLO (2016)"]
    end

    subgraph Vision Transformer
        ResNet --> ViT["⭐ ViT (2021)"]
        ViT --> SwinT["Swin Transformer (2021)"]
        ViT --> MAE["MAE (2022)"]
    end

    subgraph Generative Models
        GAN["⭐ GAN (2014)"] --> DCGAN["DCGAN (2016)"]
        DCGAN --> StyleGAN["StyleGAN (2019)"]
        GAN --> Pix2Pix["Pix2Pix (2017)"]
        GAN -.-> Diffusion["DDPM (2020)"]
        Diffusion --> LatentDiff["Latent Diffusion (2022)"]
    end

    style AlexNet fill:#FFD700
    style ResNet fill:#FFD700
    style FasterRCNN fill:#FFD700
    style ViT fill:#FFD700
    style GAN fill:#FFD700
```

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2022](2022.md)
- [2021](2021.md)
- [2017](2017.md)
- [2016](2016.md)
