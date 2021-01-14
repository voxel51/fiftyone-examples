# FiftyOne Examples

<img alt="FiftyOne" src="https://user-images.githubusercontent.com/25985824/94951983-346abe80-04b3-11eb-9717-9fb47fc8e5b2.png">

[FiftyOne](http://www.voxel51.com/docs/fiftyone) is an open source machine
learning tool created by [Voxel51](https://voxel51.com) that helps you rapidly
experiment with your data and ML models. Check out the main github repository
for the project at https://github.com/voxel51/fiftyone.

This repository contains various examples of using FiftyOne to accomplish
common tasks.

## Usage

This repository assumes that you have `fiftyone` installed on your machine. See
[this page](https://voxel51.com/docs/fiftyone/getting_started/install.html) for
installation instructions, or refer to
[this page](https://github.com/voxel51/fiftyone#installing-from-source) for
instructions on installing FiftyOne from source.

Examples are typically provided as [Jupyter Notebooks](https://jupyter.org) to
make it easy for users to download and run them. You can install Jupyter via
[these instructions](https://jupyter.org/install).

You can run a notebook as follows:

```
jupyter notebook examples/an_awesome_example.ipynb
```

## Table of Contents

| Example                                                                                           | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| [quickstart](examples/quickstart.ipynb)                                                           | A quickstart example for getting your feet wet with FiftyOne                                      |
| [walkthrough](examples/walkthrough.ipynb)                                                         | A more in-depth alternative to the quickstart that covers the basics of FiftyOne                  |
| [comparing_YOLO_and_EfficientDet](examples/comparing_YOLO_and_EfficientDet.ipynb)                 | Compares the YOLOv4 and EfficientDet object detection models on the COCO dataset                  |
| [deepfakes_in_politics](examples/deepfakes_in_politics.ipynb)                                     | Evaluating deepfakes using a deepfake detection algorithm and visualizing the results in FiftyOne |
| [emotion_recognition_presidential_debate](examples/emotion_recognition_presidential_debate.ipynb) | Analyzing the 2020 US Presidential Debates using an emotion recognition model                     |
| [evaluate_detections](examples/evaluate_detections.ipynb)                                         | Using FiftyOne to quantitatively and qualitatively evaluate object detections                     |
| [image_uniqueness](examples/image_uniqueness.ipynb)                                               | Using FiftyOne's image uniqueness method to analyze and extract insights from unlabeled datasets  |
| [structured_noise_injection](examples/structured_noise_injection.ipynb)                           | Visually exploring a method for structured noise injection in GANs from CVPR 2020                 |
| [visym_pip_175k](examples/visym_pip_175k.ipynb)                                                   | Exploring the People in Public 175K Dataset from Visym Labs with FiftyOne                         |
| [wrangling_datasets](examples/wrangling_datasets.ipynb)                                           | Using FiftyOne to load, manipulate, and export datasets in common formats                         |
| [open_images_evaluation](examples/open_images_evaluation/open_images_evaluation.ipynb)            | Evaluating the quality of the ground truth annotations of the Open Images Dataset with FiftyOne   |

## Contributing

This repository is open source and community contributions are welcome!

Check out the [contribution guide](CONTRIBUTING.md) to learn how to get
involved.

If you are contributing new material to this repository, please install the
pre-commit hooks so that your changes will be passed through our linting tools:

```
pre-commit install
```

Check out the notebook templates in `templates/` to get started writing a new
example.
