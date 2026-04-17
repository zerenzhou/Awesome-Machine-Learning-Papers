# Wireless & Communication Signals

Deep learning for physical-layer communications: autoencoder-based transceivers, modulation recognition, channel estimation, CSI feedback, MIMO detection, and semantic / joint source-channel coding. Papers are listed in reverse chronological order; ⭐ marks pioneering works.

## 2023

- **Beyond Transmitting Bits: Context, Semantics, and Task-Oriented Communications** — IEEE JSAC 2023
  [[Paper](https://arxiv.org/abs/2207.09353)]
  Comprehensive tutorial on semantic and task-oriented communications covering information-theoretic foundations, deep JSCC, and learning-based system design for 6G networks.

## 2022

- **Nonlinear Transform Source-Channel Coding for Semantic Communications** — IEEE JSAC 2022
  [[Paper](https://arxiv.org/abs/2112.10961)] [[Code](https://github.com/wsxtyrdd/NTSCC_JSAC22)]
  Introduced a learned nonlinear analysis transform as a semantic prior for joint source-channel coding, enabling content-aware rate-distortion optimization beyond vanilla DeepJSCC.

## 2020

- **Model-Driven Deep Learning for MIMO Detection** — IEEE TSP 2020 [`Algorithm Unrolling`]
  [[Paper](https://arxiv.org/abs/1907.09439)] [[Code](https://github.com/hehengtao/OAMP-Net)]
  Proposed OAMP-Net by unfolding orthogonal AMP into a trainable network for MIMO detection and joint channel estimation, with far fewer parameters than data-driven approaches.

## 2019

- **Learning to Detect** — IEEE TSP 2019 [`Algorithm Unrolling`]
  [[Paper](https://arxiv.org/abs/1805.07631)]
  Proposed DetNet by unfolding projected gradient descent into a deep network for MIMO detection, achieving near-optimal performance with learned parameters across channel distributions.

- **Deep Joint Source-Channel Coding for Wireless Image Transmission** — IEEE TCCN 2019
  [[Paper](https://arxiv.org/abs/1809.01733)]
  Proposed deep JSCC using CNNs to directly map image pixels to channel symbols, outperforming separation-based JPEG/JPEG2000 + capacity-achieving codes at low SNR.

- **Deep Learning-Based Channel Estimation** — IEEE Communications Letters 2019
  [[Paper](https://arxiv.org/abs/1810.05893)]
  Treated time-frequency channel response as a 2D image and applied deep image super-resolution and restoration techniques for pilot-based channel estimation.

## 2018

- **Deep Learning-Based Communication Over the Air** — IEEE JSTSP 2018
  [[Paper](https://arxiv.org/abs/1707.03384)]
  Demonstrated end-to-end learned autoencoder-based communications over real wireless channels using software-defined radios, validating deep learning for physical-layer design.

- **Over-the-Air Deep Learning Based Radio Signal Classification** — IEEE JSTSP 2018
  [[Paper](https://arxiv.org/abs/1712.04578)]
  Conducted comprehensive evaluation of deep learning for radio signal classification including ResNet architectures, across simulated and over-the-air channels with the RadioML 2018.01A dataset.

- **Power of Deep Learning for Channel Estimation and Signal Detection in OFDM Systems** — IEEE WCL 2018
  [[Paper](https://arxiv.org/abs/1708.08514)]
  Applied deep learning to jointly perform implicit channel estimation and signal detection in OFDM, bypassing traditional explicit CSI estimation pipelines.

- **Deep Learning for Massive MIMO CSI Feedback** — IEEE WCL 2018
  [[Paper](https://arxiv.org/abs/1712.08919)] [[Code](https://github.com/sydney222/Python_CsiNet)]
  Proposed CsiNet, a deep learning architecture that learns to compress and reconstruct massive MIMO channel state information, significantly outperforming compressive sensing methods.

## 2017

- ⭐ **An Introduction to Deep Learning for the Physical Layer** — IEEE TCCN 2017
  [[Paper](https://arxiv.org/abs/1702.00832)]
  Recast the entire communications system as an autoencoder trained end-to-end, jointly optimizing transmitter and receiver for block error rate minimization — establishing the deep learning for physical-layer paradigm.

## 2016

- ⭐ **Convolutional Radio Modulation Recognition Networks** — EANN 2016
  [[Paper](https://arxiv.org/abs/1602.04105)]
  First applied deep CNNs on raw IQ samples for automatic modulation recognition, demonstrating learned features outperform expert-crafted ones at low SNR.

- **Radio Machine Learning Dataset Generation with GNU Radio** — GNU Radio Conference 2016
  [[Paper](https://pubs.gnuradio.org/index.php/grcon/article/view/11)]
  Released the RadioML benchmark datasets for radio signal classification tasks, providing common baselines for the emerging radio machine learning community.

## Benchmark Datasets

| Dataset | Task | Scale | Description |
|:---|:---|:---|:---|
| **RadioML 2016.10a / 10b** | Modulation recognition | 220k / 1.2M samples, 11 classes | GNU Radio synthetic RF signals over varying SNR; DeepSig benchmark |
| **RadioML 2018.01a** | Modulation recognition | 2.56M samples, 24 classes | Over-the-air captures plus synthetic channels |
| **CSI Dataset (COST2100)** | CSI feedback | — | Standard channel for CsiNet-family evaluation |
| **DeepMIMO** | MIMO / beam prediction | Ray-tracing | Parametrized mmWave and massive-MIMO channel dataset |
| **ViWi / Raymobtime** | V2X / beam selection | Multi-modal | Vision-aided / ray-traced channel datasets |
