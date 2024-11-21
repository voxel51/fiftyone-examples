<div align="center">
<p align="center">

<!-- prettier-ignore -->
<img src="https://user-images.githubusercontent.com/25985824/106288517-2422e000-6216-11eb-871d-26ad2e7b1e59.png" height="55px"> &nbsp;
<img src="https://user-images.githubusercontent.com/25985824/106288518-24bb7680-6216-11eb-8f10-60052c519586.png" height="50px"> 

<div align="center">
<p align="center">

# **Examples**

</p>
</div>

**This repository contains examples of using [FiftyOne](https://github.com/voxel51/fiftyone) to accomplish various common tasks.**

---

<!-- prettier-ignore -->
<a href="https://voxel51.com/fiftyone">Website</a> •
<a href="https://voxel51.com/docs/fiftyone">Docs</a> •
<a href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/quickstart.ipynb">Try it Now</a> •
<a href="https://voxel51.com/docs/fiftyone/tutorials/index.html">Tutorials</a> •
<a href="https://voxel51.com/blog/">Blog</a> •
<a href="https://slack.voxel51.com">Community</a>

[![PyPI python](https://img.shields.io/pypi/pyversions/fiftyone)](https://pypi.org/project/fiftyone)
[![PyPI version](https://badge.fury.io/py/fiftyone.svg)](https://pypi.org/project/fiftyone)
[![Downloads](https://static.pepy.tech/badge/fiftyone)](https://pepy.tech/project/fiftyone)
[![Docker Pulls](https://badgen.net/docker/pulls/voxel51/fiftyone?icon=docker&label=pulls)](https://hub.docker.com/r/voxel51/fiftyone/)
[![Build](https://github.com/voxel51/fiftyone/workflows/Build/badge.svg?branch=develop&event=push)](https://github.com/voxel51/fiftyone/actions?query=workflow%3ABuild)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Discord](https://img.shields.io/badge/Discord-7289DA?logo=discord&logoColor=white)](https://discord.gg/fiftyone-community)
[![Slack](https://img.shields.io/badge/Slack-4A154B?logo=slack&logoColor=white)](https://slack.voxel51.com)
[![Medium](https://img.shields.io/badge/Medium-12100E?logo=medium&logoColor=white)](https://medium.com/voxel51)
[![Mailing list](http://bit.ly/2Md9rxM)](https://share.hsforms.com/1zpJ60ggaQtOoVeBqIZdaaA2ykyk)
[![Twitter](https://img.shields.io/twitter/follow/Voxel51?style=social)](https://twitter.com/voxel51)


</p>
</div>

# 👋 hey there!

We created an open-source tool that supercharges your computer vision and machine learning workflows by enabling you to visualize datasets, analyze models, and improve data quality more efficiently than ever before. Embark with us in this adventure 🤝. **[FiftyOne](https://fiftyone.ai)**.

![------------------------------------------------------------------](https://github.com/user-attachments/assets/fb0573d0-bb56-40ff-9ae1-a5e8f62f5f42)


<div id='-prerequisites'/>

<details>
<summary>Prerequisites for beginners</summary>

## <img src="https://user-images.githubusercontent.com/25985824/106288517-2422e000-6216-11eb-871d-26ad2e7b1e59.png" height="20px"> prerequisites for beginners 🧸

**Fiftyone** requires Python (3.9 - 3.11), Git and other dependencies. To get started, select the guide for your operating system or environment, if you are an experienced developer you can avoid this section. If you are looking for scaling solution to be installed in Cloud Enterprise Systems, please take a look of **Fiftyone Teams** [here](https://voxel51.com/book-a-demo/)

<details>
<summary>Windows</summary>

<div id='-prerequisites_windows'/>

### 1. Install Python and Git

#### 1.1 Install Python

**Note:** ⚠️ The version of Python that is available in the Microsoft Store is **not recommended**. 

Download a Python installer from [python.org](https://www.python.org/downloads/). Choose Python **3.9**, **3.10**, or **3.11** and make sure to pick a **64-bit** version. For example, this [Python 3.10.11 installer](https://www.python.org/ftp/python/3.10.11/python-3.10.11-amd64.exe).
Double-click on the installer to run it, and follow the steps in the installer.
  - **Check the box to add Python to your PATH**, and to install py.
  - At the end of the installer, there is an option to **disable the PATH length limit**. It is recommended to click this.

#### 1.2 Install Git

Download Git from [this link](https://git-scm.com/download/win).
Double-click on the installer to run it, and follow the steps in the installer.

### 2. Install Microsoft Visual C++ Redistributable and FFMPEG (Optional)

Download [Microsoft Visual C++ Redistributable](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist).
Double-click on the installer to run it, and follow the steps in the installer.

#### Install FFMPEG

Download FFMPEG binary from [here](https://ffmpeg.org/download.html).
Set FFMPEG's path (e.g., C:\ffmpeg\bin) to the PATH environmental variable on Windows.

### 3. Create a Virtual Environment

- Press `Win + R`. type `cmd`, and press `Enter`. Alternatively, search **Command Prompt** in the Start Menu.
- Navigate to your project. ` cd C:\path\to\your\project`
- Create the environment `python -m venv fiftyone_env`
- Activate the environment typing this in the command line window `fiftyone_env\Scripts\activate`
- After activation, your command prompt should change and show the name of the virtual environment `(fiftyon_env) C:\path\to\your\project`
- Now you are ready to install **Fiftyone** and all the requirements/packages/dependencies. Go to [Installation](#-installation) section in this Readme file.
- Once you want to deactivate your environment, just type `deactivate`

</details>

<details>
<summary>Linux</summary>

<div id='-prerequisites_linux'/>

### 1. Install Python and Git

You may need to install some additional libraries on Ubuntu Linux. These steps work on a clean install of Ubuntu Desktop 20.04, and should also work on Ubuntu 22.04 and 20.10, and on Ubuntu Server.

```shell
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install python3-venv build-essential python3-dev git-all libgl1-mesa-dev ffmpeg
```

- On Linux, you will need at least the `openssl` and `libcurl` packages. 
- On Debian-based distributions, you will need to install `libcurl4` or`libcurl3` instead of `libcurl`, depending on the age of your distribution.

  For example:

```shell
# Ubuntu
sudo apt install libcurl4 openssl

# Fedora
sudo dnf install libcurl openssl
```
### 2. Create and activate the Virtual Environment

```shell
python3 -m venv fiftyone_env
source fiftyone_env/bin/activate
```

Now you are ready to install **Fiftyone** and all the requirements/packages/dependencies. Go to [Installation](#-installation) section in this Readme file.

</details>

<details>
<summary>MacOS</summary>

<div id='-prerequisites_macos'/>

### 1. Install Xcode Command Line Tools

```shell
xcode-select --install
```
### 2.  Install Homebrew
```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
After you install it, follow the instructions from the Homebrew installation to set it up.

### 3. Install Python and dependencies

```shell
brew install python@3.9
brew install protobuf

#optional but recommendeded
brew install ffmpeg
```
### 4. Create and activate the Virtual Environment

```shell
python3 -m venv fiftyone_env
source fiftyone_env/bin/activate
```

Now you are ready to install **Fiftyone** and all the requirements/packages/dependencies. Go to [Installation](#-installation) section in this Readme file.


</details>

<details>
<summary>Docker</summary>

<div id='-prerequisites_docker'/>

Refer to
[these instructions](https://voxel51.com/docs/fiftyone/environments/index.html#docker)
to see how to build and run Docker images containing source or release builds
of FiftyOne.


</details>

<div align="center">
<p align="center">

| [Windows](#-prerequisites_windows) | [Linux](#-prerequisites_linux) | [macOS](#-prerequisites_macos) | [Docker](#-prerequisites_docker) | 
| ----------------------------------------------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | 

</p>
</div>

**Important Notes:** Remember, you will need...

-   [Python](https://www.python.org) (3.9 - 3.11)
-   [Node.js](https://nodejs.org) - on Linux, we recommend using
    [nvm](https://github.com/nvm-sh/nvm) to install an up-to-date version.
-   [Yarn](https://yarnpkg.com) - once Node.js is installed, you can
    [enable Yarn](https://yarnpkg.com/getting-started/install) via
    `corepack enable`
    
</details>

![------------------------------------------------------------------](https://github.com/user-attachments/assets/fb0573d0-bb56-40ff-9ae1-a5e8f62f5f42)

## <img src="https://user-images.githubusercontent.com/25985824/106288517-2422e000-6216-11eb-871d-26ad2e7b1e59.png" height="20px"> Usage 🔥

Each example in this repository is provided as a
[Jupyter Notebook](https://jupyter.org). The table of contents below provides
handy links for each example:

<img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">&nbsp;
Click this link to **run** the notebook in
[Google Colab](https://colab.research.google.com) (no setup required!)

<img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">&nbsp;
Click this link to **view** the notebook in
[Jupyter nbviewer](https://nbviewer.jupyter.org)

<img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">&nbsp;
Click this link to **download** the notebook

### Running examples locally

You can always clone this repository:

```shell
git clone https://github.com/voxel51/fiftyone-examples
```

and run any example locally. Make sure you have
[Jupyter installed](https://jupyter.org/install) and then run:

```shell
jupyter notebook examples/an_awesome_example.ipynb
```
![------------------------------------------------------------------](https://github.com/user-attachments/assets/fb0573d0-bb56-40ff-9ae1-a5e8f62f5f42)

## List of Examples

<!-- Autogenerated by `scripts/make_examples.py` -->
<table>
    <tr>
        <th align="center">Shortcuts</th>
        <th align="center">Examples</th>
        <th align="center">Description</th>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/quickstart.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/quickstart.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/quickstart.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/quickstart.ipynb">quickstart</a></td>
        <td>A quickstart example for getting your feet wet with FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/walkthrough.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/walkthrough.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/walkthrough.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/walkthrough.ipynb">walkthrough</a></td>
        <td>A more in-depth alternative to the quickstart that covers the basics of FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/zilliz_advent_of_code.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/zilliz_advent_of_code.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/zilliz_advent_of_code.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/zilliz_advent_of_code.ipynb">zilliz_advent_of_code</a></td>
        <td>Welcome to FiftyOne: Zilliz Advent of Open Source Code 2023</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/ai_telephone.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/ai_telephone.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/ai_telephone.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/ai_telephone.ipynb">ai_telephone</a></td>
        <td>Play multimodal AI telephone with text-to-image models, image-to-text models, and Fiftyone</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/clean_conceptual_captions.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/clean_conceptual_captions.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/clean_conceptual_captions.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/clean_conceptual_captions.ipynb">clean_conceptual_captions</a></td>
        <td>Clean Google's Conceptual Captions Dataset with Fiftyone to train your own ControlNet</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/segment_anything_openvino.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/segment_anything_openvino.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/segment_anything_openvino.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/segment_anything_openvino.ipynb">segment_anything_openvino</a></td>
        <td>Add object masks to a FiftyOne dataset with OpenVINO-optimized Segment Anything Model</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/comparing_YOLO_and_EfficientDet.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/comparing_YOLO_and_EfficientDet.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/comparing_YOLO_and_EfficientDet.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/comparing_YOLO_and_EfficientDet.ipynb">comparing_YOLO_and_EfficientDet</a></td>
        <td>Compares the YOLOv4 and EfficientDet object detection models on the COCO dataset</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/digging_into_coco.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/digging_into_coco.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/digging_into_coco.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/digging_into_coco.ipynb">digging_into_coco</a></td>
        <td>A simple example of how to find mistakes in your detection datasets</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/deepfakes_in_politics.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/deepfakes_in_politics.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/deepfakes_in_politics.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/deepfakes_in_politics.ipynb">deepfakes_in_politics</a></td>
        <td>Evaluating deepfakes using a deepfake detection algorithm and visualizing the results in FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/emotion_recognition_presidential_debate.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/emotion_recognition_presidential_debate.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/emotion_recognition_presidential_debate.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/emotion_recognition_presidential_debate.ipynb">emotion_recognition_presidential_debate</a></td>
        <td>Analyzing the 2020 US Presidential Debates using an emotion recognition model</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/image_uniqueness.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/image_uniqueness.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/image_uniqueness.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/image_uniqueness.ipynb">image_uniqueness</a></td>
        <td>Using FiftyOne's image uniqueness method to analyze and extract insights from unlabeled datasets</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/structured_noise_injection.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/structured_noise_injection.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/structured_noise_injection.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/structured_noise_injection.ipynb">structured_noise_injection</a></td>
        <td>Visually exploring a method for structured noise injection in GANs from CVPR 2020</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/visym_pip_175k.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/visym_pip_175k.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/visym_pip_175k.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/visym_pip_175k.ipynb">visym_pip_175k</a></td>
        <td>Exploring the People in Public 175K Dataset from Visym Labs with FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/wrangling_datasets.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/wrangling_datasets.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/wrangling_datasets.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/wrangling_datasets.ipynb">wrangling_datasets</a></td>
        <td>Using FiftyOne to load, manipulate, and export datasets in common formats</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/open_images_evaluation/open_images_evaluation.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/open_images_evaluation/open_images_evaluation.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/open_images_evaluation/open_images_evaluation.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/open_images_evaluation/open_images_evaluation.ipynb">open_images_evaluation</a></td>
        <td>Evaluating the quality of the ground truth annotations of the Open Images Dataset with FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/working_with_feature_points.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/working_with_feature_points.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/working_with_feature_points.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/working_with_feature_points.ipynb">working_with_feature_points</a></td>
        <td>A simple example of computing feature points for images and visualizing them in FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/image_deduplication.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/image_deduplication.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/image_deduplication.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/image_deduplication.ipynb">image_deduplication</a></td>
        <td>Find and remove duplicate images in your image datasets with FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/exploring_classification_hardness.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/exploring_classification_hardness.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/exploring_classification_hardness.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/exploring_classification_hardness.ipynb">hardness_for_image_classification</a></td>
        <td>Use the FiftyOne Brain to mine the hardest images in your classification dataset</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/pytorch_detection_training.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/pytorch_detection_training.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/pytorch_detection_training.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/pytorch_detection_training.ipynb">pytorch_detection_training</a></td>
        <td>Using FiftyOne datasets to train a PyTorch object detection model</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/pytorchvideo_tutorial.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/pytorchvideo_tutorial.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/pytorchvideo_tutorial.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/pytorchvideo_tutorial.ipynb">pytorchvideo_model_evaluation</a></td>
        <td>Evaluate and visualize PyTorchVideo models with FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/training_clearml_detector.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/training_clearml_detector.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/training_clearml_detector.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/training_clearml_detector.ipynb">training_clearml_detector</a></td>
        <td>Train a model with ClearML and FiftyOne to detect DRAGONS!</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/convert_tags_to_classifications.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/convert_tags_to_classifications.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/convert_tags_to_classifications.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/convert_tags_to_classifications.ipynb">converting_tags_to_classifications</a></td>
        <td>Convert classifications to tags and back to annotate them right in the FiftyOne App</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/Qdrant_FiftyOne_Recipe.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/Qdrant_FiftyOne_Recipe.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/Qdrant_FiftyOne_Recipe.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/Qdrant_FiftyOne_Recipe.ipynb">Qdrant_FiftyOne_Recipe</a></td>
        <td>Nearest neighbor classification of embeddings with Qdrant</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/armbench_defect_detection.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/armbench_defect_detection.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/armbench_defect_detection.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/armbench_defect_detection.ipynb">armbench_defect_detection</a></td>
        <td>Visualizing Defects in Amazon’s ARMBench Dataset Using Embeddings and OpenAI’s CLIP Model</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/openvino_detection_with_fiftyone.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/openvino_detection_with_fiftyone.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/openvino_detection_with_fiftyone.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/openvino_detection_with_fiftyone.ipynb">openvino_model_horizontal_text_detection</a></td>
        <td>Horizontal text detection on Total-Text Dataset using OpenVino Model</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/chest_xray14.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/chest_xray14.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/chest_xray14.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/chest_xray14.ipynb">chest_xray14</a></td>
        <td>Load and explore the NIH's ChestX-ray14 dataset in FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/football_player_segmentation.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/football_player_segmentation.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/football_player_segmentation.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/football_player_segmentation.ipynb">football_player_segmentation</a></td>
        <td>Detection and Segmentation on Football Player Segmentation Dataset using SAM</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/wildme_conservation_datasets.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/wildme_conservation_datasets.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/wildme_conservation_datasets.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/wildme_conservation_datasets.ipynb">wildme_conservation_datasets</a></td>
        <td>Create a 'meta' dataset out of three WildMe conservation datasets in FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/Tips_and_Tricks_CLI.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/Tips_and_Tricks_CLI.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/Tips_and_Tricks_CLI.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/Tips_and_Tricks_CLI.ipynb">CLI Tips & Tricks</a></td>
        <td>Use FiftyOne's Command Line Interface to expedite your workflows</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/Grouped Datasets.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/Grouped Datasets.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/Grouped Datasets.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/Grouped Datasets.ipynb">Grouped Dataset Tips & Tricks</a></td>
        <td>Learn how to work with grouped datasets in FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/Keypoints.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/Keypoints.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/Keypoints.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/Keypoints.ipynb">Keypoint Tips & Tricks</a></td>
        <td>Learn how to work with keypoint skeletons in FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/3D Detections.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/3D Detections.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/3D Detections.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/3D Detections.ipynb">3D Detections Tips & Tricks</a></td>
        <td>Make your first 3D detection in point clouds using FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/heatmaps.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/heatmaps.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/heatmaps.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/heatmaps.ipynb">Heatmaps Tips & Tricks</a></td>
        <td>Learn how to use heatmaps with a body pose estimation example</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/examples/Video Labels.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/examples/Video Labels.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/examples/Video Labels.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="examples/Video Labels.ipynb">Video Labels Tips & Tricks</a></td>
        <td>Learn different label types in video datasets with ASL videos</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/Tracking_Datasets.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/Tracking_Datasets.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/Tracking_Datasets.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="Tracking_Datasets.ipynb">Tracking Datasets with FiftyOne</a></td>
        <td>Learn how to load and work with tracking datasets with the help of FiftyOne</td>
    </tr>
    <tr>
        <td>
            <a target="_blank" href="https://colab.research.google.com/github/voxel51/fiftyone-examples/blob/master/GradCam + More Tutorial.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791629-6e618700-5769-11eb-857f-d176b37d2496.png" height="22" width="22">
            </a>
            <a target="_blank" href="https://nbviewer.jupyter.org/github/voxel51/fiftyone-examples/blob/master/GradCam + More Tutorial.ipynb">
                <img src="https://user-images.githubusercontent.com/25985824/104791634-6efa1d80-5769-11eb-8a4c-71d6cb53ccf0.png" height="22" width="22">
            </a>
            <a id="raw-url" href="https://raw.githubusercontent.com/voxel51/fiftyone-examples/master/GradCam + More Tutorial.ipynb" download>
                <img src="https://user-images.githubusercontent.com/25985824/104792428-60f9cc00-576c-11eb-95a4-5709d803023a.png" height="22" width="22">
            </a>
        </td>
        <td><a href="GradCam + More Tutorial.ipynb">GradCam and More with FiftyOne</a></td>
        <td>Apply Model Explainability techniques to your workflows with FiftyOne and GradCam!</td>
    </tr>
</table>

![------------------------------------------------------------------](https://github.com/user-attachments/assets/fb0573d0-bb56-40ff-9ae1-a5e8f62f5f42)
<div id='-contributing'/>

## <img src="https://user-images.githubusercontent.com/25985824/106288517-2422e000-6216-11eb-871d-26ad2e7b1e59.png" height="20px"> contributing to FiftyOne Examples 🧡


This repository is open source and community contributions are welcome!

Check out the [contribution guide](CONTRIBUTING.md) to learn how to get
involved.

<div align="center">
<p align="center">

### 🤝 **Join Our Community** 🤝

Connect with us through your preferred channels:
    
[![Discord](https://img.shields.io/badge/Discord-7289DA?logo=discord&logoColor=white)](https://discord.gg/fiftyone-community)
[![Slack](https://img.shields.io/badge/Slack-4A154B?logo=slack&logoColor=white)](https://slack.voxel51.com)
[![Medium](https://img.shields.io/badge/Medium-12100E?logo=medium&logoColor=white)](https://medium.com/voxel51)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?logo=twitter&logoColor=white)](https://twitter.com/voxel51)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/company/voxel51)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?logo=facebook&logoColor=white)](https://www.facebook.com/voxel51)

**Share your workflow improvements on social media and tag us @Voxel51 and #FiftyOne!**. 

🎊 You will be in our rewarded list. 🎊

</p>
</div>


![------------------------------------------------------------------](https://github.com/user-attachments/assets/fb0573d0-bb56-40ff-9ae1-a5e8f62f5f42)

<div id='-contributors'/>

## <img src="https://user-images.githubusercontent.com/25985824/106288517-2422e000-6216-11eb-871d-26ad2e7b1e59.png" height="20px"> contributors 🤓

Special thanks to these amazing people for contributing to FiftyOne Examples! 🙌

<a href="https://github.com/voxel51/fiftyone/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=voxel51/fiftyone-examples" />
</a>

![------------------------------------------------------------------](https://github.com/user-attachments/assets/fb0573d0-bb56-40ff-9ae1-a5e8f62f5f42)
<div id='-citation'/>

## <img src="https://user-images.githubusercontent.com/25985824/106288517-2422e000-6216-11eb-871d-26ad2e7b1e59.png" height="20px"> citation 📖

If you use a specific contributed example in this repository, feel free to cite the project (but only if you love it 😊):

```bibtex
@article{moore2020fiftyone,
  title={FiftyOne},
  author={Moore, B. E. and Corso, J. J.},
  journal={GitHub. Note: https://github.com/voxel51/fiftyone},
  year={2020}
}
```




