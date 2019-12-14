# For-papers

Including ideas and processes



|                          会议/期刊                           | Abstract Deadline |  Paper deadline   |
| :----------------------------------------------------------: | :---------------: | :---------------: |
|             [WCCI](https://wcci2020.org/calls/)              |         -         | January 15, 2020  |
| [IJCAI-PRICAI](https://www.ijcai20.org/call-for-papers.html) | January 15, 2020  | January 21, 2020  |
| [GECCO](https://gecco-2020.sigevo.org/index.html/Call+for+Papers) | January 30, 2020  | February 6, 2020  |
|                   [ICML](https://icml.cc/)                   | January 31, 2020  | February 7, 2020  |
|          [TOG](http://transactions.games/#special)           |         -         | February 29, 2020 |
|             [CoG](http://ieee-cog.org/2020/cfp)              |         -         |  March 23, 2020   |
|        [PPSN](https://ppsn2020.liacs.leidenuniv.nl/)         |   April 1, 2020   |   April 8, 2020   |

[AI Conference Deadlines](https://aideadlin.es/?sub=,ML,RO,CV,SP,NLP,DM)

[Openreview](https://openreview.net/)



## Game

Based on [《Evolving Mario Levels in the Latent Space of a Deep Convolutional Generative Adversarial Network》](https://arxiv.org/abs/1805.00728)

Key points: GAN, CMA-ES, Latent variable evolution

### Problems

* 1、Certain broken structures in the output

### Solutions

* text (symbol sequence) generation models such as LSTMs

### Ideas

* 1、用进化算法寻找潜在向量的方法不好，因为是不连续的函数，相关性很低
* 2、衡量难度不应该用跳跃次数，应该用noisy下的成功几率，抗干扰能力，不找最好的AI
* 3、检测故障的块在GAN中
* 4、多目标的组合情况，现在是线性组合，如何组合，多目标算法，取舍

### Code

[Evolving Mario Levels whole project](https://github.com/TheHedgeify/DagstuhlGAN)



### Related Links

[About Generative Adversarial Network (GAN)](https://github.com/yzy1996/Artificial-Intelligence/tree/master/Machine-Learning/GAN)



### Related Papers

[Searching the Latent Space of a Generative Adversarial Network to Generate DOOM Levels](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8848011) 同样运用CMA-ES+GAN，只是迁移到了ZOOM这一个游戏



### Daily summary

Dec 12 2019: update the part of ideas, figure out the concept of CMA-ES and Latent vector

Dec 13 2019: solve the problem of java

Dec 14 2019: try the GAN, and WGAN