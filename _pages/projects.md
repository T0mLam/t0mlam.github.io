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
sidebar: 
  nav: "projects"
---

As I am interested in computer vision and deep learning, much of my time is spent on creating side projects or re-implementing papers. Below you will find my recent projects that I did during my free time outside classes or on vacations which I am very proud of. 😆

---

<!-- Land Cover Segmentation with UNets -->

<div class='title' id='land' style='margin-bottom: -10px;'>
  <h1>Land Cover Segmentation with UNets</h1>
  <div class='widgets'>
    <a href="https://github.com/T0mLam/Landcover-Segmentation-with-UNets">
      <i class="fab fa-github button"></i>
    </a>
    <!--
    <a href="https://t0mlam.github.io/posts/2024/08/practicing-pytorch-and-image-segmentation/">
      <i class="fa-solid fa-blog button"></i>
    </a>
    -->
  </div>
</div>

<div class='badges'>
  <img src='https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white'>
  <img src='https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white'>
  <img src='https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black'>
</div>

Semantic segmentation of the [Multi-Source Satellite Imagery for Segmentation Dataset](https://www.kaggle.com/datasets/hammadjavaid/multi-source-satellite-imagery-for-segmentation/data) with [UNet](https://link.springer.com/chapter/10.1007/978-3-319-24574-4_28) and [ResUNet-a](https://arxiv.org/abs/1904.00592) (a variant of ResUNet) in PyTorch.
<!--
 This repository holds the first PyTorch implementation of the ResUNet-a d6 model on Github.[^1]
-->

<div class="images">
    <img src='/images/projects/landcover-segmentation-with-unets/unet_segmentation_results.png' width='50%'>
    <img src='/images/projects/landcover-segmentation-with-unets/res_unet_a_segmentation_results.png' width='50%'>
</div>

I incorporated the trained models into a graphical interface using Streamlit. It allows users to randomly generate a image segmentation mask from the test dataset and upload images to the models.

<img src='/images/projects/landcover-segmentation-with-unets/app.gif'>

Unfortunitely, the models are not able to generalize well to real-world images due to the limited number of data samples in the dataset. <br>

---

<!-- LeNet-5 From Scratch -->

<div class='title' id='lenet' style='margin-bottom: -10px;'>
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

During the summer vacation after my foundation year, I took an [online course](https://tinyurl.com/bdr6href) on machine learning which really sparked my interest in deep neural networks. 🤩 Having no internships and nothing else to do, I decided to spend my summer building a handwritten digit recognition app, marking the start of my journey in deep learning. 🥳

<div class="images">
    <img src='/images/projects/lenet-5-from-scratch/architecture.png' width='75%'>
    <img src='/images/projects/lenet-5-from-scratch/app_demo.gif' width='25%'>
</div>

## Installation

### Clone the Repository

```bash
git clone https://github.com/T0mLam/LeNet-5-from-scratch.git
cd LeNet-5-from-scratch
```

### Install dependencies

```bash
pip install -r requirements.txt
```

## Usage

### Launch the app

```bash
python -m app
```

### Import and use the modules

Create a new file `experiment.py` in the root directory

```python
# Use the format 'from modules.{filename} import {module}'

# e.g. import the Adam optimizer
from modules.optimizer import Adam
...
optimizer = Adam(model, lr=0.001)

```

Run the script

```bash
python -m experiment
```

---

<!--
[^1]: Sorry for boasting too much. The model I implementated was the ResUNet-a d6 model instead of the more complex d7 multi-tasking model. I also replaced the Tanimoto Loss purposed in the paper to a conventional Dice Loss.
-->

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
