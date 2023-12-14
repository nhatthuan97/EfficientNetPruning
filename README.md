# EfficientNetPruning

## Overview

The goal of this project is to explore the behavior of EfficientNetB0 when subjected to l1 pruning at the Conv2D layer. Pruning is performed at three different ratios: 0%, 15%, and 50%.

## Repository Contents

This repository contains two types of files:

### Notebook Files

1. **Demo1000.ipynb**: This notebook is designed for live class demonstrations. Its primary objective is to run 10 samples from each class in the CIFAR-100 dataset and analyze the highest and lowest accuracy achieved.

2. **Demo10000.ipynb**: This notebook is not suitable for live demos but is meant for more comprehensive analysis. It is similar to Demo1000, but each class in the CIFAR-100 dataset is represented by 100 samples, providing more detailed insights.

3. **IndividualRun.ipynb**: This notebook serves as an explanatory guide to the project's code structure. It includes detailed Markdown explanations for each section and allows users to select their pretrained model to load.

### Pretrained Model Files (pth files)

The pretrained model files are stored in the following formats:

- **prune0_train.pth**: This is the smallest file and represents the base EfficientNetB0 model with no pruning.

- **prune15_train.pth** and **prune50_train.pth**: These files are larger than prune0_train.pth because Torch NN introduces new masking parameters during pruning. Due to their size, they are compressed as zip files (prune15_train.zip and prune50_train.zip). To use these pretrained models, unzip the corresponding file to the project directory.

## Getting Started

To begin exploring this project, follow these steps:

1. Clone this repository to your local machine.

2. Explore the different notebook files to understand the project's objectives and analyses.

3. If you wish to use the pretrained models with pruning ratios of 15% and 50%, unzip the corresponding zip files in the project directory.

4. Run the notebooks to conduct experiments and analyze the results.

