# Group 5 — Deep Learning: CIFAR-10 Image Classification with CNN

A convolutional neural network (CNN) trained on the CIFAR-10 dataset, built with TensorFlow/Keras as part of a deep learning course project.

## Members

| Name | 
|------|
| Tatjana Kiseļova |
| Dante Wensby |
| Thanadol Sutantiwanichkul |
| Sofia Larsson |
| Miren Urrutia Iturritza |
| Panagiotis Kalogeropoulos |

## Project Overview

This project explores image classification on the [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) dataset — 60,000 colour images (32×32) across 10 classes:

`airplane` · `automobile` · `bird` · `cat` · `deer` · `dog` · `frog` · `horse` · `ship` · `truck`

### Model Architecture

A sequential CNN with the following structure:

```
Conv2D(8)  → Conv2D(16) → MaxPool
Conv2D(32) → MaxPool
Conv2D(64) → MaxPool
Flatten → Dense(128) → Dense(32) → Dense(10)
```

- **Optimizer:** Adam  
- **Loss:** Sparse Categorical Cross-Entropy  
- **Epochs:** 15

## Results

| Metric | Value |
|--------|-------|
| Test Loss | 0.903 |
| Test Cross-Entropy | 1.965 |

## Repository Structure

```
.
├── Gr5_model.ipynb        # Main model notebook
├── CNN_CIFAR_Demo_3.ipynb # Demo / exploration notebook
├── environment.yml        # Conda environment
└── README.md
```

## Getting Started

**1. Create the conda environment:**

```bash
conda env create -f environment.yml
conda activate dl
```

**2. Launch JupyterLab:**

```bash
jupyter lab
```

**3. Open `Gr5_model.ipynb` and run all cells.**
