# Diabetic Foot Ulcer Segmentation using PyramidNet

A deep learning implementation of a **PyramidNet-based semantic segmentation architecture** tailored for medical image segmentation, specifically targeting diabetic foot ulcer localization and boundary delineation.

---

## Overview

Diabetic foot ulcers (DFUs) require precise, non-invasive boundary assessment to monitor healing trajectories and support clinical interventions. This project implements a lightweight PyramidNet segmentation network developed in TensorFlow/Keras to perform automated ulcer boundary segmentation on standard RGB wound imagery.

- **Total Trainable Parameters**: 2,006,114 (~2.01M)
- **Framework**: TensorFlow 2.x (Keras)
- **Application**: Medical image analysis / Diabetic Foot Ulcer Segmentation Challenge

---

## Repository Structure

```text
ulcer-segmentation-using-pyramidnet/
├── ulcer-segmentation-using-pyramidnet.ipynb  # Full training, preprocessing & evaluation pipeline
├── Pyramid_Net-epoch-49.weights.h5            # Pretrained model checkpoint (epoch 49)
├── Weights/                                   # Checkpoint storage directory
├── LICENSE                                    # Open source license
└── README.md                                  # Repository documentation
```

---

## Setup & Requirements

### Dependencies
- Python `>= 3.8`
- TensorFlow `>= 2.12.0` (tested on 2.17.0)
- OpenCV (`opencv-python`)
- NumPy
- Matplotlib
- tqdm

### Quick Installation
```bash
pip install tensorflow opencv-python numpy matplotlib tqdm
```

---

## Usage

1. Open and run [`ulcer-segmentation-using-pyramidnet.ipynb`](ulcer-segmentation-using-pyramidnet.ipynb) in Google Colab or a local Jupyter Notebook environment with GPU acceleration.
2. Load the trained checkpoint directly:
```python
from tensorflow.keras.models import load_model

# Load model architecture and weights
model.load_weights("Pyramid_Net-epoch-49.weights.h5")
```

---

## Author & Citation

**Pritam Chakraborty**  
School of Computer Engineering, KIIT Deemed to be University, Bhubaneswar, India  
Email: pritam23@ieee.org
