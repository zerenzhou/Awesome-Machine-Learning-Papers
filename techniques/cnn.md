# CNN

A collection of must-read papers on convolutional neural network architectures from top venues.

- ⭐ **ImageNet Classification with Deep Convolutional Neural Networks** — NeurIPS 2012 [`CV`]
  [[Paper](https://papers.nips.cc/paper/2012/hash/c399862d3b9d6b76c8436e924a68c45b-Abstract.html)]
  Introduced AlexNet, demonstrating the power of deep CNNs with ReLU, dropout, and GPU training on large-scale image classification.

- ⭐ **Very Deep Convolutional Networks for Large-Scale Image Recognition** — ICLR 2015 [`CV`]
  [[Paper](https://arxiv.org/abs/1409.1556)]
  Showed that increasing network depth with small 3x3 convolution filters (VGGNet) significantly improves image recognition performance.

- ⭐ **Deep Residual Learning for Image Recognition** — CVPR 2016 [`CV`]
  [[Paper](https://arxiv.org/abs/1512.03385)] [[Code](https://github.com/KaimingHe/deep-residual-networks)]
  Introduced residual connections (ResNet) enabling training of very deep networks by learning residual mappings.

- ⭐ **Going Deeper with Convolutions** — CVPR 2015 [`CV`]
  [[Paper](https://arxiv.org/abs/1409.4842)]
  Proposed the Inception module (GoogLeNet), using parallel multi-scale convolutions to improve efficiency and accuracy.

- **Densely Connected Convolutional Networks** — CVPR 2017 [`CV`]
  [[Paper](https://arxiv.org/abs/1608.06993)] [[Code](https://github.com/liuzhuang13/DenseNet)]
  Introduced dense connections between layers (DenseNet), strengthening feature propagation and reducing parameters.

- **Convolutional Sequence to Sequence Learning** — ICML 2017 [`NLP`]
  [[Paper](https://arxiv.org/abs/1705.03122)] [[Code](https://github.com/facebookresearch/fairseq)]
  Applied CNN with gated linear units to sequence-to-sequence tasks, achieving competitive results with faster training than RNNs.

- **EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks** — ICML 2019 [`CV`]
  [[Paper](https://arxiv.org/abs/1905.11946)] [[Code](https://github.com/tensorflow/tpu/tree/master/models/official/efficientnet)]
  Proposed compound scaling of depth, width, and resolution to systematically improve CNN efficiency and accuracy.

- **TCN: An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling** — arXiv 2018 [`TSF`]
  [[Paper](https://arxiv.org/abs/1803.01271)] [[Code](https://github.com/locuslab/TCN)]
  Demonstrated that temporal convolutional networks outperform RNNs on a range of sequence modeling benchmarks.
