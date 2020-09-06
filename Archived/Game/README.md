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
* 2、how to evaluate the game map generation

### Ideas

* 1、用进化算法寻找潜在向量的方法不好，因为是不连续的函数，相关性很低
* 2、衡量难度不应该用跳跃次数，应该用noisy下的成功几率，抗干扰能力，不找最好的AI
* 3、检测故障的块在GAN中
* 4、多目标的组合情况，现在是线性组合，如何组合，多目标算法，取舍，加入偏好性

### Solutions

#### evaluation

* 1、(数值) 比较loss
* 2、(数值) Agent玩的分数，用A,B两个play算法去玩，用performance的差值作为指标，相对值比绝对值更有说服力 iipp，差值大体现区别性，体现游戏的难度
* 3、(非数值) 人来评判，问卷调查

* 4、(数值) 评价难度，给agent加噪声，再看成功率

#### EA

* 1+1ES 
* CMA-ES



### Algorithm

#### play 

random play(不动)、MCTS、A*、EA

### Code

[Evolving Mario Levels whole project](https://github.com/TheHedgeify/DagstuhlGAN)



### Related Links

[About Generative Adversarial Network (GAN)](https://github.com/yzy1996/Artificial-Intelligence/tree/master/Machine-Learning/GAN)

[The Video Game Level Corpus](https://github.com/TheVGLC/TheVGLC)

[Mario-AI-Framework](https://github.com/amidos2006/Mario-AI-Framework)



### Related Papers

[Searching the Latent Space of a Generative Adversarial Network to Generate DOOM Levels](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8848011) 同样运用CMA-ES+GAN，只是迁移到了DOOM这一个游戏

[Intentional Computational Level Design](https://arxiv.org/pdf/1904.08972.pdf) 2019 用的Feasible-Infeasible 2-Population (FI2Pop) and Constrained Map-Elites



https://aibirds.org/call-for-papers.html