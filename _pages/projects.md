---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
gallery:
  - url: projects/lenet-5-from-scratch/app_demo.gif
    image_path: projects/lenet-5-from-scratch/app_demo.gif
    alt: "My digit recognization app with LeNet-5 as the model"
    title: "My digit recognization app with LeNet-5 as the model"
  - url: projects/lenet-5-from-scratch/architecture.png
    image_path: projects/lenet-5-from-scratch/architecture.png
    alt: "The LeNet-5 CNN Architecture"
    title: "The LeNet-5 CNN Architecture"
---


As I am interested in data science and deep learning, much of my time is spent on creating side projects or re-implementing papers. Below you will find my recent projects that I did during my free time outside classes or on vacations which I am very proud of. 😆


<!-- Landcover Segmentation with UNets -->


<div class='title' style='margin-bottom: -10px;'>
  <h1>Landcover Segmentation with UNets</h1>
  <div class='widgets'>
    <a href="https://github.com/T0mLam/Landcover-Segmentation-with-UNets">
      <i class="fab fa-github button"></i>
    </a>
    <a href="https://t0mlam.github.io/posts/2024/08/practicing-pytorch-and-image-segmentation/">
      <i class="fa-solid fa-blog button"></i>
    </a>
  </div>
</div>

<div class='badges'>
  <img src='https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white'>
  <img src='https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black'>
</div>

Semantic segmentation of satellite images with [UNet](https://doi.org/10.1007/978-3-319-24574-4_28) and [ResUNet-a](https://arxiv.org/abs/1904.00592) in PyTorch.


<!-- LeNet-5 From Scratch -->


<div class='title' style='margin-bottom: -10px;'>
  <h1>LeNet-5 From Scratch</h1>
  <div class='widgets'>
    <a href="https://github.com/T0mLam/LeNet-5-from-scratch">
      <i class="fab fa-github button"></i>
    </a>
    <a href="https://t0mlam.github.io/posts/2024/08/my-first-ml-project/">
      <i class="fa-solid fa-blog button"></i>
    </a>
  </div>
</div>

<div class='badges'>
  <img src='https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white'>
</div>

During the summer vacation after my foundation year, I took an [online course](https://tinyurl.com/bdr6href) on machine learning which really sparked my interest in deep neural networks. 🤩 Having nothing else to do as I was living in Bristol, I decided to spend my summer building a handwritten digit recognition app, marking the start of my journey in deep learning. 🥳

<div class="images">
    <img src='/images/projects/lenet-5-from-scratch/architecture.png' width='75%'>
    <img src='/images/projects/lenet-5-from-scratch/app_demo.gif' width='25%'>
</div>


<style>
  .title {
    display: flex;
    
    h1 {
      margin-right: 10px;
    }
  }

  .badges {
    margin-top: 5px;
  }

  .widgets {
    transform: translateY(-5px);
    display: flex;
    gap: 10px;
    align-items: center;
  }

  .images {
    display: flex; 
    justify-content: space-between;
  }

  .button {
    display: inline-block;
    font-size: 20px;
    color: #449DD1;
    transition: transform 0.3s ease, color 0.3s ease;
  }

  .button:hover {
    transform: scale(1.2);
    color: #192BC2;
  }
</style>
