PathGAN
======================
A Pytorch implementation of **Generative Adversarial Network for Heuristics of Sampling-based Path Planning**

[Original arXiv paper](https://arxiv.org/pdf/2012.03490.pdf)

## Table of content

- [Structure](#structure)
  - [Searching algorithm](#searching-algorithm)
  - [GAN architecture](#gan-architecture)
- [Dataset](#dataset)
- [Training](#training)
- [Results](#results)
- [License](#license)
- [Links](#links)


## Structure

The overall structure of the PathGAN consists of two things:
1) RRT* searching algorithm and
2) Generative Aversarial Network for promising region generation 

### Searching algorithm

**`RRT*` algorithm:**

<a><img src="assets/gan_rrt.png" align="center" height="150px" width="350px"/></a>

**Comparing `RRT*` and `Heuristic RRT*`:**

<a><img src="assets/rrt_vs_hrrt.png" align="center" height="350px" width="340px"/></a>

### GAN architecture

**Overall `GAN` architecture:**

<a><img src="assets/gan.jpg" align="center" height="400px" width="600px"/></a>

**`GAN` architecture in details:**

<a><img src="assets/detailed_gan.jpg" align="center" height="400px" width="800px"/></a>

## Dataset

**[Dataset](https://disk.yandex.ru/d/mgf5wtQrld0ygQ) of 10,000 samples (`Map`, `Point`, `ROI`):**
- train set (8,000 samples)
- test set (2,000 samples)

## Training

## Results

**[Results](https://disk.yandex.ru/d/jObhWjtA2KbR6w) on `test set` of [dataset](https://disk.yandex.ru/d/mgf5wtQrld0ygQ) above:**

<a><img src="assets/result.png" align="center" height="600px" width="750px"/></a>

**RRT `-->` True ROI `-->` Pred ROI `-->` IoU**

**mIoU = 0.957 (`average` IoU for all 2,000 samples in `test set`)**

## License

This project is licensed under MIT.

## Links

* **[Generative Adversarial Network based Heuristics for Sampling-based Path Planning (arXiv article)](https://arxiv.org/pdf/2012.03490.pdf)**

* **[Dataset](https://disk.yandex.ru/d/mgf5wtQrld0ygQ)**

* **[Results](https://disk.yandex.ru/d/jObhWjtA2KbR6w)**
