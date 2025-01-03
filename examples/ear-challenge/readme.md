# Elderly Action Recognition Challenge - Dataset Preparation

This repository contains a Jupyter Notebook that demonstrates how to prepare a dataset for the **Elderly Action Recognition Challenge**, hosted as part of the **Computer Vision for Smalls Workshop (CV4Smalls)** at **WACV 2025**.

The notebook leverages [FiftyOne](https://voxel51.com/) to streamline dataset preparation, including importing, parsing actions, assigning categories, splitting videos into clips, and exporting datasets.

---

## Challenge Overview

The **Elderly Action Recognition Challenge** focuses on identifying Activities of Daily Living (ADLs) and fall detection for the elderly. Participants are encouraged to contribute models that address real-world healthcare challenges and assistive living scenarios.

- **Challenge Page**: [Details & Instructions](https://voxel51.com/computer-vision-events/elderly-action-recognition-challenge-wacv-2025/)
- **Submission Platform**: [Submit Here](https://eval.ai/web/challenges/challenge-page/2427/overview)
- **Discord Channel**: [Join the Discussion](https://discord.com/channels/1266527359511564372/1319053378843836448)

---

## Repository Contents

### 1. **Notebook: `elderly_action_recognition.ipynb`**
This notebook walks you through:
- Setting up the GMDCSA24 Dataset.
- Parsing and categorizing actions.
- Splitting videos into clips based on individual actions.
- Exporting the dataset in different formats (e.g., Classification Directory Tree, FiftyOne format).

### 2. **Example Dataset**
We use the [GMDCSA24 Dataset](https://doi.org/10.5281/zenodo.12921216) in this notebook, which is designed for human fall detection and ADL recognition.

### 3. **Resources**
- [FiftyOne Documentation](https://docs.voxel51.com/)
- [GMDCSA24 GitHub Project Page](https://github.com/ekramalam/GMDCSA24-A-Dataset-for-Human-Fall-Detection-in-Videos)
- [Scientific Paper on GMDCSA24](https://www.sciencedirect.com/science/article/pii/S2352340924008552)

---

## Prerequisites

### 1. Install Dependencies
Make sure you have Python 3.8 or higher installed, and als have a Python Environment in yout system. For beginners, take a look of these [instructions](https://github.com/voxel51/fiftyone-examples?tab=readme-ov-file#-prerequisites-for-beginners-)

Then, install the jupyter lab or run this notebook using VS Code
```bash
pip install jupyterlab
```
---

## Dataset Download

Download the GMDCSA24 dataset from Zenodo: https://doi.org/10.5281/zenodo.12921216

## Usage

1. Open the notebook:
```bash
jupyter lab elderly_action_recognition.ipynb
```

2. Follow the steps in the notebook:

- Define the dataset path and initialize a FiftyOne dataset.
- Parse and categorize actions.
- Split videos into clips.
- Export the processed dataset for model training.

3. Launch the FiftyOne App to interact with and visualize your dataset:
```bash
session = fo.launch_app(dataset)
```

## Output Formats

- Video Classification Directory Tree: Organized for action classification tasks.
- FiftyOne Dataset Format: Exported to leverage FiftyOne's advanced features.

## Contributing
We welcome contributions to improve the notebook or add new features! Including Model Training, Model Evaluation. Please submit a pull request or open an issue with your suggestions.