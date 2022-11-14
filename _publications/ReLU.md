---
title: "Numerical influence of ReLU’(0) on backpropagation"
collection: publications
permalink: /publication/relu_prime
#excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2021-12-01
venue: 'Neurips'
paperurl: 'https://proceedings.neurips.cc/paper/2021/hash/043ab21fc5a1607b381ac3896176dac6-Abstract.html'
citation: 'D. Bertoin, J. Bolte, S. Gerchinovitz, E. Pauwels'
---
*(David Bertoin, Jérôme Bolte, Sébastien Gerchinovitz, Edouard Pauwels)*

In theory, the choice of ReLU(0) in [0, 1] for a neural network has a negligible influence both on backpropagation and training. Yet, in the real world, 32 bits default precision combined with the size of deep learning problems makes it a hyperparameter of training methods. We investigate the importance of the value of ReLU'(0) for several precision levels (16, 32, 64 bits), on various networks (fully connected, VGG, ResNet) and datasets (MNIST, CIFAR10, SVHN, ImageNet). We observe considerable variations of backpropagation outputs which occur around half of the time in 32 bits precision. The effect disappears with double precision, while it is systematic at 16 bits. For vanilla SGD training, the choice ReLU'(0) = 0 seems to be the most efficient. For our experiments on ImageNet the gain in test accuracy over ReLU'(0) = 1 was more than 10 points (two runs). We also evidence that reconditioning approaches as batch-norm or ADAM tend to buffer the influence of ReLU'(0)’s value. Overall, the message we convey is that algorithmic differentiation of nonsmooth problems potentially hides parameters that could be tuned advantageously.

[Download paper here](https://proceedings.neurips.cc/paper/2021/hash/043ab21fc5a1607b381ac3896176dac6-Abstract.html)

