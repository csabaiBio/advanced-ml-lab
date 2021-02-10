# Advanced Machine learning seminar

This is the official repository of the advanced machine learning seminar. Please see all the topics below. If you have a topic suggestion please email [us](mailto:olaralex666@gmail.com) and we might consider it to be included here.

## Topics

### 1. [Hamiltonian neural networks](https://arxiv.org/abs/1906.01563)

*Abstract:* Even though neural networks enjoy widespread use, they still struggle to learn the basic laws of physics. How might we endow them with better inductive biases? In this paper, we draw inspiration from Hamiltonian mechanics to train models that learn and respect exact conservation laws in an unsupervised manner. We evaluate our models on problems where conservation of energy is important, including the two-body problem and pixel observations of a pendulum. Our model trains faster and generalizes better than a regular neural network. An interesting side effect is that our model is perfectly reversible in time.

* Read the above article and understand the basics of it.
* Take a simple Hamiltonian and run a number of simulations with it in order to generate training data [code required]
* Set up the training pipeline for the Hamiltonian neural net manually and run it on your data.
* Evaluate the predictions compared to the simple Euler method.

### 2. [Neural style transfer](https://arxiv.org/abs/1508.06576)

*Abstract:* In fine art, especially painting, humans have mastered the skill to create unique visual experiences through composing a complex interplay between the content and style of an image. Thus far the algorithmic basis of this process is unknown and there exists no artificial system with similar capabilities. However, in other key areas of visual perception such as object and face recognition near-human performance was recently demonstrated by a class of biologically inspired vision models called Deep Neural Networks. Here we introduce an artificial system based on a Deep Neural Network that creates artistic images of high perceptual quality. The system uses neural representations to separate and recombine content and style of arbitrary images, providing a neural algorithm for the creation of artistic images. Moreover, in light of the striking similarities between performance-optimised artificial neural networks and biological vision, our work offers a path forward to an algorithmic understanding of how humans create and perceive artistic imagery.

* sequel: [Fast neural style transfer](https://cs.stanford.edu/people/jcjohns/papers/eccv16/JohnsonECCV16.pdf), [Fast stylization](https://arxiv.org/abs/1607.08022)

* Read the above articles and discuss what the differences are between them
* Select one you wish to implement (PyTorch recommended)
  * model
  * training script
  * evaluation script
* Create a small movie and convert it into your style(s)

### 3. [Generative models: an alternative to GANs](https://arxiv.org/abs/1907.05600)

*Abstract:* We introduce a new generative model where samples are produced via Langevin dynamics using gradients of the data distribution estimated with score matching. Because gradients can be ill-defined and hard to estimate when the data resides on low-dimensional manifolds, we perturb the data with different levels of Gaussian noise, and jointly estimate the corresponding scores, i.e., the vector fields of gradients of the perturbed data distribution for all noise levels. For sampling, we propose an annealed Langevin dynamics where we use gradients corresponding to gradually decreasing noise levels as the sampling process gets closer to the data manifold. Our framework allows flexible model architectures, requires no sampling during training or the use of adversarial methods, and provides a learning objective that can be used for principled model comparisons. Our models produce samples comparable to GANs on MNIST, CelebA and CIFAR-10 datasets, achieving a new state-of-the-art inception score of 8.87 on CIFAR-10. Additionally, we demonstrate that our models learn effective representations via image inpainting experiments.

* read and understand the basics of the article
  * NOTE: this should take the longest, the math here is not trivial and would be nice to know more about
* investigate how it is different from generative adversarial networks
* do a basic implementation of
  * model
  * training
  * Langevin sampling
* evaluate your generated images with the basic generative scores (FID, Inception score)

-----------------------

Requirements:
* your own code - do not copy from the web, the goal is that you understand what you do
* read the paper carefully and understand the math
* every 2-3 weeks do a small presentation about what you did so far [create a public GitHub repository and share it with us in the issues]
