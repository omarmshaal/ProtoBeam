# ProtoBeam

## Overview

**ProtoBeam** is an implementation of Prototypical Networks aimed at improving beam classification across different antenna configurations in mmWave communication systems. It addresses the challenge of domain shifts, where models trained on one set of antenna hardware may not generalize well to another. By leveraging Prototypical Networks, ProtoBeam enhances the ability of deep learning models to generalize across different domains without requiring retraining, making it an effective solution for real-world beam management in wireless networks.

## Features

- **Domain Adaptation:** Uses Prototypical Networks to handle domain shifts in mmWave beam management, allowing models trained on one antenna setup to generalize to others.
- **Data Augmentation and Normalization:** Incorporates data normalization and augmentation techniques to improve model robustness and accuracy.
- **Flexible and Scalable:** Designed to work with varying antenna configurations, providing a scalable solution for real-world deployments.
- **Open-Source Implementation:** All code is available in this repository, allowing for further research and development.

## Installation

To run the ProtoBeam code, ensure that you have the following dependencies installed:

- **Python 3.10.12**
- **PyTorch 2.2.2+cu118**
- **NumPy 1.26.3**

## Usage

The core implementation is contained in the ProtoBeam.ipynb Jupyter notebook. To use the code:

**1-** Clone this repository:
```bash
git clone https://github.com/yourusername/ProtoBeam.git
cd ProtoBeam
```

**2-** Launch the Jupyter notebook.

**3-** Follow the steps in the notebook to load the dataset, train the Prototypical Network, and evaluate its performance across different antenna configurations.


## Dataset

The dataset used in this implementation is the DeepBeam dataset, which includes experimental data from 24 horizontal beam codebooks using different SiBeam 60 GHz frontends. This dataset can be customized or extended depending on your specific needs.

## Validation and Evaluation

To ensure accurate and unbiased performance metrics, validation data is shuffled before evaluation. This shuffling helps to avoid any sequence-related issues that might affect the prototypes built during testing, ensuring a fair assessment of the model's generalization capabilities.

## Project Basis

This project is based on the tutorial notebook available at: [Meta-Learning Tutorial.](https://github.com/phlippe/uvadlc_notebooks/blob/master/docs/tutorial_notebooks/tutorial16/Meta_Learning.ipynb)


## Contact

For any questions or suggestions, feel free to reach out to the repository owner or open an issue on GitHub.
