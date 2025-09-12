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

<!-- ChronoChat -->
<div class='title' id='chrono-chat' style='margin-bottom: -10px;'>
  <h1>ChronoChat</h1>
  <div class='widgets'>
    <a href="https://github.com/T0mLam/chrono-chat">
      <i class="fab fa-github button"></i>
    </a>
  </div>
</div>

<div class='badges'>
  <img src='https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54'>
  <img src='https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white'>
  <img src='https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white'>
  <img src='https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white'>
  <img src='https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi'>
</div>  

ChronoChat is a UI for Ollama that enables users to chat with video content using non vision/video-language models (VLMs). It supports both YouTube and local uploads and uses retrieval-augmented generation (RAG) to answer questions using video transcripts, frames, and captions. Powered by local LLMs, ChronoChat streams real-time responses with additional support for images and PDF uploads.

<video src="/images/projects/chrono-chat/demo.mp4" width="100%" controls autoplay muted loop>
  Sorry, your browser doesn’t support embedded videos.
</video>

<br />

---

<!-- bristollink -->
<div class='title' id='bristollink' style='margin-bottom: -10px;'>
  <h1 class="pink-gradient-title">BristolLink</h1>
  <div class='widgets'>
    <a href="https://bristollink.uk">
      <i class="fa-regular fa-globe pink-icon"></i>
    </a>
  </div>
</div>

<div class='badges'>
  <img src='https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB'>
  <img src='https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white'>
  <img src='https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white'>
  <img src='https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white'>
</div>

An anonymous match-making platform for University of Bristol student during Valentine's Day 2025.

<img src='/images/projects/bristollink/pages.png'>

<h2>How does <span><img class="link-logo" src="/images/projects/bristollink/logo.webp"></span> work?</h2>

**1. Enter their Email**

Find their UoB email through Outlook and submit it through Bristol Link. They'll receive an anonymous notification that someone is interested.

**2. Wait for their Response**

If they're interested, they'll log into Bristol Link and enter an email address of their own choice.

**3. Check for a Match**

If the emails match, you both receive confirmation and can start your story. If not, you'll be notified and can try with someone new.

---

<!-- ecosim -->
<div class='title' id='ecosim' style='margin-bottom: -10px;'>
  <h1>EcoSim</h1>
  <div class='widgets'>
    <a href="https://github.com/BRSY1/ecosim">
      <i class="fab fa-github button"></i>
    </a>
  </div>
</div>

<div class='badges'>
  <img src='https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white'>
  <img src='https://img.shields.io/badge/javafx-%23FF0000.svg?style=for-the-badge&logo=javafx&logoColor=white'>
</div>

<p class="event-info">Best ML Project - BrisHack 2025</p>

EcoSim is a Java-based simulation developed during BrisHack 2025. It models the interactions between various animal species and their environment, utilizing procedural terrain generation and intelligent agent behavior.

<img src='/images/projects/ecosim/ecosim.png' width='100%'>

## Contributors

<div class="ecosim-team-container">
    <table>
        <tr>
            <td class="ecosim-team-member">
                <a href="https://github.com/archiekind">
                    <img src="https://avatars.githubusercontent.com/archiekind">
                    <b>Archie Kind</b>
                </a>
            </td>
            <td class="ecosim-team-member">
                <a href="https://github.com/hrsh9486">
                    <img src="https://avatars.githubusercontent.com/hrsh9486">
                    <b>Harish Rajkumar</b>
                </a>
            </td>
            <td class="ecosim-team-member">
                <a href="https://github.com/jwdlb">
                    <img src="https://avatars.githubusercontent.com/jwdlb">
                    <b>Jack Dempsey</b>
                </a>
            </td>
            <td class="ecosim-team-member">
                <a href="https://github.com/joshjkns">
                    <img src="https://avatars.githubusercontent.com/joshjkns">
                    <b>Josh Jenkins</b>
                </a>
            </td>
            <td class="ecosim-team-member">
                <a href="https://github.com/kshubham-108">
                    <img src="https://avatars.githubusercontent.com/kshubham-108">
                    <b>Shubham Kulkarni</b>
                </a>
            </td>
            <td class="ecosim-team-member">
                <a href="https://github.com/T0mLam">
                    <img src="https://avatars.githubusercontent.com/T0mLam">
                    <b>Tom Lam</b>
                </a>
            </td>
        </tr>
    </table>
</div>

## Features

- **Procedural Terrain Generation**: Uses **Perlin noise** to create realistic and dynamic terrain landscapes.
- **Animal AI with Monte Carlo Tree Search (MCTS)**: Animals use **MCTS-based decision-making** to move intelligently, avoiding predators, seeking food, and reproducing.
- **Predator-Prey Dynamics**: Implements a food chain where animals interact based on hierarchical levels, engaging in hunting, fleeing, and breeding behaviors.
- **Environmental Factors**: Includes terrain types that influence movement and survival.
- **Graphical Interface**: Built using **JavaFX**, allowing users to visualize the ecosystem in real time.
- **Event Logging and Statistics**: Displays ecosystem events and population statistics in real-time.

## Running the app

### Install Java Runtime Environment (JRE)

You can download Java from the [official Oracle website](https://www.oracle.com/java/technologies/downloads/).

### Install the EcoSim JAR file

Download the pre-built JAR file from the [releases section](https://github.com/BRSY1/ecosim/releases)

### Navigate to the directory with the JAR File

Then run

```bash
java -jar ecosim-1.0.0.jar
```

---

<!-- claude-haskell -->

<div class='title' id='claude-haskell' style='margin-bottom: -10px;'>
  <h1>Claude-haskell</h1>
  <div class='widgets'>
    <a href="https://github.com/T0mLam/claude-haskell">
      <i class="fab fa-github button"></i>
    </a>
  </div>
</div>

<div class='badges'>
  <img src='https://img.shields.io/badge/Haskell-5D4F85?style=for-the-badge&logo=haskell&logoColor=white'>
</div>

**claude-haskell is an unofficial binding for Anthropic's Claude API. This project has not been reviewed or published as an official package.**

This library provides Haskell functions to interact with the Claude API, including sending text messages, images, pdf documents, listing and retrieving model information, and create message batches. It includes utilities and types for building API requests and handling responses.

<div class="widgets">
  <a href="https://github.com/T0mLam/claude-haskell#readme">
    <button class="btn btn--inverse">Read installation and usage guide</button>
  </a> 
  <a href="https://docs.anthropic.com/en/api/getting-started">
  <button class="btn btn--inverse">Read Anthropic's API docs</button>
  </a>
</div>

---

<!-- Candycombs -->

<div class='title' id='candycombs' style='margin-bottom: -10px;'>
  <h1 class='halloween-launch'>🍬Candycombs</h1>
  <div class='widgets'>
    <a href="https://github.com/BRSY1/candycombs">
      <i class="fab fa-github halloween-button"></i>
    </a>
  </div>
</div>

<div class='badges'>
  <!--<img src='https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54'>-->
  <img src='/images/projects/candycombs/pygame_logo.png' width='80px' style='margin-top: -10px;'>
</div>

<p class="event-info">Bristol CSS 24-Hour GameJam 2024</p>

A 2D Halloween-themed game featuring various mini-games. Players collect candies by exploring rooms, answering trivia questions, trying their luck at the roulette table, and opening chests to gain power-ups.

<video width="100%" controls autoplay muted loop>
  <source src="/images/projects/candycombs/candycombs_gameplay.mp4" type="video/mp4">
</video>

## Contributors

<div class="team-table-responsive">
  <table class="team-table">
    <tr align="center" valign="top">
      <td><a href="https://github.com/archiekind"><img src="https://avatars.githubusercontent.com/archiekind" width="80" height="80"><br><b>Archie Kind 🎃</b></a></td>
      <td><a href="https://github.com/hrsh9486"><img src="https://avatars.githubusercontent.com/hrsh9486" width="80" height="80"><br><b>Harish Rajkumar 👻</b></a></td>
      <td><a href="https://github.com/rsh-e"><img src="https://avatars.githubusercontent.com/rsh-e" width="80" height="80"><br><b>Hrushikesh Emkay 🧛</b></a></td>
      <td><a href="https://github.com/jwdlb"><img src="https://avatars.githubusercontent.com/jwdlb" width="80" height="80"><br><b>Jack Dempsey 🦇</b></a></td>
      <td><a href="https://github.com/joshjkns"><img src="https://avatars.githubusercontent.com/joshjkns" width="80" height="80"><br><b>Josh Jenkins 🕸️</b></a></td>
      <td><a href="https://github.com/kshubham-108"><img src="https://avatars.githubusercontent.com/kshubham-108" width="80" height="80"><br><b>Shubham Kulkarni 🧙</b></a></td>
      <td><a href="https://github.com/T0mLam"><img src="https://avatars.githubusercontent.com/T0mLam" width="80" height="80"><br><b>Tom Lam 🎃</b></a></td>
    </tr>
  </table>
</div>

## Installation

### Clone the Repository

```bash
git clone https://github.com/BRSY1/candycombs.git
cd candycombs
```

### Install dependencies

```bash
pip install -r requirements.txt
```

## Launch the game

```bash
python3 test.py
```

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
    margin-top: 10px;
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    align-items: center;
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

  .team-table-responsive {
    display: block;
    overflow: auto;
    width: 100%;
  }

  .team-table {
    background-color: #ffffff; /* light background */
    color: #f1c40f; /* Halloween yellow text color */
    border: 2px solid #ff7518; /* Orange border */
    border-radius: 10px;
    padding: 15px;
  }

  .team-table td {
    padding: 10px;
  }

  .team-table a {
    color: #f1c40f;
    text-decoration: none;
  }

  .team-table img {
    border-radius: 50%;
    box-shadow: 0px 4px 10px rgba(255, 117, 24, 0.5); /* Orange glow */
  }

  .team-table b {
    font-size: 1em;
    display: block;
    margin-top: 8px;
    color: #f39c12; /* Pumpkin orange color */
  }

  /* Add a subtle hover effect for spooky touch */
  .team-table td:hover {
    background-color: #3e3b41;
    transition: background-color 0.3s ease;
  }

  /* Emoji bounce for extra Halloween vibe */
  .team-table b::after {
    content: ' 🎃';
    display: inline-block;
    animation: bounce 1.5s infinite;
  }

  @keyframes bounce {
    0%, 20%, 50%, 80%, 100% {
      transform: translateY(0);
    }
    40% {
      transform: translateY(-8px);
    }
    60% {
      transform: translateY(-4px);
    }
  }

  .halloween-launch {
    color: #ff7518;
    text-shadow: 0 0px 2px #ff7518, 0 0px 4px #ff7518, 0 0 6px #ff7518;
    animation: flicker 1.2s infinite alternate;
  }

  @keyframes flicker {
    0% {
      opacity: 1;
    }
    50% {
      opacity: 0.8;
    }
    100% {
      opacity: 1;
    }
  }

  .halloween-button {
    display: inline-block;
    font-size: 20px;
    color: #FD7F20;
    transition: transform 0.3s ease, color 0.3s ease;
  }

  .halloween-button:hover {
    transform: scale(1.2);
    color: #944F00;
  }

  .event-info {
    color: #6e6e6e;
    font-style: italic;
    font-weight: bold;
  }

  .pink-gradient-title {
    background: linear-gradient(to right,rgb(255, 117, 129), #ff7eb3); -webkit-background-clip: text; color: transparent;
  }

  .pink-icon {
    color: #ff7eb3;
    transition: transform 0.3s ease, color 0.3s ease;
  }

  .pink-icon:hover {
    transform: scale(1.2);
    color:rgb(209, 58, 111);
  }

  .link-logo {
    width: 65px;
    transform: translateY(-3px);
    opacity: 75%;
  }

  .ecosim-team-container {
    padding: 20px;
    background-color: #f4f4ec;
    border-radius: 15px;
    box-shadow: 3px 3px 15px rgba(0, 0, 0, 0.1);
    overflow: auto;
  }

  .ecosim-team-container table {
    border-collapse: collapse;
    width: 100%;
    text-align: center;
  }

  .ecosim-team-container td {
    padding: 10px;
    white-space: nowrap;
  }

  .ecosim-team-member {
    padding: 20px;
    transition: background-color 0.3s ease-in-out, transform 0.2s;
    border-radius: 10px;
  }

  .ecosim-team-member:hover {
    background-color: #d9e6cc;
    transform: scale(1.05);
  }

  .ecosim-team-member a {
    text-decoration: none;
    color: #2f613f;
    display: inline-block;
  }

  .ecosim-team-member img {
    width: 80px;
    height: 80px;
    max-width: 100%;
    border-radius: 50%;
    border: 3px solid #a3c09a;
    transition: transform 0.3s;
    object-fit: cover;
  }

  .ecosim-team-member:hover img {
    transform: rotate(5deg);
  }

  .ecosim-team-member b {
    display: block;
    margin-top: 10px;
    font-size: 16px;
  }
</style>
