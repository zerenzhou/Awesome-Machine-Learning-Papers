# Computer Vision — Tech Tree

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

## Key Evolution Paths

| Path | Description |
|------|-------------|
| **Classification** | LeNet → AlexNet → VGG/Inception → ResNet → EfficientNet → ViT |
| **Detection** | R-CNN → Fast/Faster R-CNN → FPN / YOLO series |
| **Vision Transformer** | ViT → Swin Transformer → MAE (self-supervised) |
| **Generation** | GAN → DCGAN → StyleGAN → Diffusion → Latent Diffusion |
