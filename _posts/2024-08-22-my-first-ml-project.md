---
title: 'My First ML Project 👨🏻‍💻🤖 (sort of)'
date: 2024-08-22
permalink: /posts/2024/08/my-first-ml-project/
tags:
  - Deep Learning 🤖
---

It is about everything interesting and challenging during the process of building my [LeNet-5 From Scratch](https://t0mlam.github.io/projects/) project. Please lower your expectation before clicking in. 😬🫣

# How I got started in machine learning

My interest in ML emerged during my computer science foundation year. At the time, one of my assignment for the English for Academic Purpose module was to write an essay about an ethical issue in the field of computer science that everyone should know. 

<img src='/images/blogs/my-first-ml-project/eap_essay.png' style='width: 65%; margin: -20px auto; display: block;'>

The topic I wrote about was related to the ethics of recommender systems, which powers the search engines of websites like Youtube and Netflix. Despite the fact that I did not have any technical understanding of how recommender systems work, I was deeply intrigued by the ethical issues I had researched into, e.g. cold-start problem, the diversity problem and etc. I was curious and keen to know the working principles and the ML algorithms behind this 'black-box' seeing how powerful and influential recommender systems were to every internet users.

Fastforward to 14/6/2024, I was relieved as I finished all my IFP examination. I planned to spend my summer on an ML online course on Coursera. During the process, I learned a lot about the foundation of machine learning, from linear algebra to the linear regression model and the gradient descent optimizer for neural networks, as well as machine learning tools like scikit-learn and PyTorch. 

As I have finished the course in late July, I decided to put together my knowledge and challenge myself with a project. The challenge I gave myself was to implement the LeNet-5 model from scratch.

# What is LeNet-5

LeNet-5 is a pioneering Convolutional Neural Network (CNN) architecture in the field of deep learning, particularly known for the handwritten digit classification on the MNIST dataset. It was developed in the late 8-90s by [Yann LeCun](https://en.wikipedia.org/wiki/Yann_LeCun) and proposed in his paper [Gradient-based learning applied to document recognition](https://ieeexplore.ieee.org/document/726791).

Here is a video showcasing his work in handwritten digit recognition.

<iframe src='https://www.youtube.com/embed/FwFduRA_L6Q?si=1TXBDGq9Dr5xnNRH' frameborder="0" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>></iframe>
<br>
The early prototypes of the LeNet-5 model had been used for identifying handwritten zip code numbers provided by the US Postal Service and recognizing digits writtens on cheques.

<img src='/images/blogs/my-first-ml-project/lenet_demo.gif' style='width: 65%; margin: 0px auto; display: block;'>

If you would like to know more about LeNet, I have linked another blog post [here](https://www.educative.io/blog/lenet-5) from `educative.io`.


# So what is my project about

I built a simple handwritten digit recognition app with my implementation of LeNet-5 as the model. 

__What is so special about this project is that I did not use any deep learning libraries or auto-differentiation tools like PyTorch or Tensorflow, instead I created all neural network modules from simple mathematical functions provided by numpy, e.g. matrix multiplication & exponential functions.__

<img src='/images/blogs/my-first-ml-project/app_demo.gif' style='width: 65%; margin: 0px auto; display: block;'>

I have followed the architecture outlined in the original paper with several slight modifications. One of which was that I switched the original RBF output layer in the model to a Softmax layer in combination with the Cross Entropy Loss function which enabled me to display the output confidence / probability for each prediction. 

Here is the original architecture of the LeNet-5

<img src='/images/blogs/my-first-ml-project/architecture.png'>

Here is a high-level (1) overview of my implementation

<img src='/images/blogs/my-first-ml-project/model_code.png'>

# How I coded it up

In summary, the model consists of 4 major components ...

## Layers

```python
"""
Includes ...
1. conventional
2. activation
3. normalization 
4. regularization 
5. pooling
layers
"""
class Layer:
    def forward(self, X: NDArray, **kwargs) -> NDArray:
        pass

    def backward(self, grad: NDArray) -> NDArray:
        pass

    def __call__(self, *args, **kwargs):
        return self.forward(*args, **kwargs)
```

The `Layer` class is the base class of all other building blocks the model. 

__In forward propagation__, the `forward` method takes an input `X` and return a numpy 
array as output after the layer operations.

__In backpropagation__, each layer returns an output gradient, which usually consists of a calculation result of the derivative of the `forward` operations and the input gradients, to its previous layer in the model.

## Sequential Class

```python
class Sequential:
    def __init__(self, blocks: List[Layer]) -> None:
        self.blocks = blocks
        self.is_training = True    

    def forward(self, X: NDArray) -> NDArray:
        for block in self.blocks:
            X = block(X, train=self.is_training)
        return X

    def backward(self, grad: NDArray) -> None:
        for block in reversed(self.blocks):
            grad = block.backward(grad)

    def train(self) -> None:
        self.is_training = True

    def eval(self) -> None:
        self.is_training = False

    def __call__(self, *args, **kwargs):
        return self.forward(*args, **kwargs)
```

You can think of it as a container of the layers. It allows the model to be executed sequentially at once instead of having to execute every layers manually in both forward and backward propagation. It also acts as a switch to control the behaviour of the layers depending on whether it is in training or testing stage.

## Optimizer 

```python
class Optimizer:
    def __init__(self, model: Sequential, lr: float) -> None:
        self.model = model
        self.lr = lr

    def step(self):
        pass
```

This is where the 'learning' of the model happens. The `step` function updates the learnable parameters of each layer by changing it's original value to a calculation result of it's value and the 'delta value' calculated during backpropagation. <br>
e.g. 

$$W_{new} = W_{old} - lr \times W_{change} \\ b_{new} = b_{old} - lr \times b_{change}$$

with $W$ and $b$ being the weight and bias of a linear layer in gradient descent.


## Criterion

```python
class Loss:
    def forward(self, y: NDArray, y_pred: NDArray) -> float:
        pass

    def backward(self) -> NDArray:
        pass

    def __call__(self, *args, **kwargs):
        return self.forward(*args, **kwargs)
```

The structure of the `Loss` is very similar to the `Layer` class. The only difference is that the criterion (loss) function takes `y` (the true label of the sample) and `y_pred` (the prediction made by the model) as input and returns a value representing the difference between the two. The backward function returns the derivative of the forward function and passes the output down layer by layer for backward propagation.

There are also additional components outside the these major ones that I just mentioned. If you would like to know more in-depth how I created the modules, train and test the model, and integrating the model into the app, click the button below to view the source code.

<a href="https://github.com/T0mLam/LeNet-5-from-scratch/">
  <button class="btn btn--inverse">View My Repository</button>
</a>

# Challenges

## Bad at maths 🙈

I must admit I am not a maths genius. 😔

## Unclear instructions 😢🤷‍♂️
