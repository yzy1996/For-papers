# For-papers

Including ideas and processes



## Game

Based on [《Evolving Mario Levels in the Latent Space of a Deep Convolutional Generative Adversarial Network》](https://arxiv.org/abs/1805.00728)

Key points: GAN, CMA-ES, Latent variable evolution

### Problems

* 1、Certain broken structures in the output

### Solutions

* text (symbol sequence) generation models such as LSTMs

### Ideas

* 1、用进化算法寻找潜在向量的方法不好，因为是不连续的函数，相关性很低
* 2、衡量难度不应该用跳跃次数，应该用noisy下的成功几率
* 3、检测故障的块在GAN中
* 4、多目标的组合情况，现在是线性组合，如何组合，多目标算法，取舍

### Daily summary

Dec 12 2019