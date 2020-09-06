# Detail



## Dynamic-Net

In this paper we present a first attempt at alleviating the need for re-training. Rather than fixing the network at training time, we train a “Dynamic-Net” that can be modified at inference time





### relate work

Multi-loss objectives





## HyperNetworks

**Problem**: The author proposed an approach of using a small network (called a “hypernetwork") to generate the weights for a larger network (called a main network). Because of the non-shared weights, the main network may perform better. And the author solved the problem of a big matrix.

**Method**: The author proposed static hypernetworks and dynamic hypernetworks. Here I only introduce the part of static hypernetworks: convolutional networks. The majority of model parameters are in the kernels of convolutional layers. The hypernetwork is a two-layer linear network and the input is an embedding vector that describes the entire weights of a given layer. It is obvious that by using this approach, the whole parameters are reduced.

**Related Knowledge**: HyperNEAT, end to end training,

**Result**: Author's approach is trained end-to-end with gradient descent together with the main network, therefore are more efficient. Testing on CNN and LSTM and get SOTA performance. 

Their main result is that hypernetworks can generate non-shared weights for LSTM and achieve near state-of-the-art results on a variety of sequence modelling tasks including character-level language modelling, handwriting generation and neural machine translation, challenging
the weight-sharing paradigm for recurrent networks



什么是权值共享;

首先什么是权值，一个filter核里面的数就可以看成权值

全连接网络，参数个数太多，于是想个办法降低一下，

权值共享的优缺点;

