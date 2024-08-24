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

<img src='/images/blogs/my-first-ml-project/app_demo.gif' style='width: 65%; margin: 0px auto; display: block;'>

I have followed the architecture outlined in the original paper with several slight modifications. One of which was that I switched the original RBF output layer in the model to a Softmax layer in combination of the Cross Entropy Loss function which enabled me to display the output confidence / probability for each prediction. 

Here is the original architecture of the LeNet-5

<img src='/images/blogs/my-first-ml-project/architecture.png'>


# Challenges


