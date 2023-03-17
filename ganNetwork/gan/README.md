# GANs

> GANs (Generative Adversarial Nets) (2014) [[paper]](https://arxiv.org/pdf/1406.2661.pdf) [[Github]](https://github.com/goodfeli/adversarial)

## Introduction

GANs model is developed by Ian Goodfellow and his colleagues in 2014. It consists two main components: a **generator** and a **discriminator**, they engage in a continuous game of competition, hence the term "adversarial."
- **Generative** model $G$ that captures the data distribution and creates realistic synthetic data samples. The object is mimic the distribution of the real data.
- **Discriminative** model $D$ that estimates the probability that if a sample came from the training data or $G$. It acts as a classifier, taking input from both the generator's output and real data samples, and learns to classify them as either real or fake.

**Adversarial Nets**
In the framework, both models are multilayer perceptrons. 
Input data is $x$. Generator's distribution is $p_g$. Input noise variables $p_z(z)$. Mapping to data space is $G(z;\theta_g)$, where $G$ is a [differentiable function](https://en.wikipedia.org/wiki/Differentiable_function) represented by neural network with parameters $\theta_g$. Second neural network $D(x;\theta_d)$ outputs a single scalar, $D(x)$ represents the probability that $x$ came from the input data rather than $p_g$.
The **training purpose** is to train $D$ to maximize the probability of assigning the correct label to the input data, train $G$ to minimize $\log(1-D(G(z)))$.
The value function is $V(G,D)$:
$$
\min_G\max_D V(D,G)=\mathop{\mathbb{E}}_{x\sim p_{data}(x)}[\log{D(x)}]+\mathop{\mathbb{E}}_{z\sim p_{z}(z)}[\log{1-D(G(z))}]
$$




