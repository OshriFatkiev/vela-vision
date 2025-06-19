# VELA Vision

This repository contains deep learning models developed as part of my MSc research to analyze mock galaxy images from the **VELA simulation suite**. The goal is to detect and classify morphological features in high-redshift galaxies using simulated JWST observations.

## Contents

### 1. Object Detection – YOLOv1 and YOLOv3
Located in the `detection/` folder.

- Implementations of YOLOv1 and YOLOv3 in PyTorch
- Trained on mock JWST NIRCam images from VELA simulations
- Designed to identify bright clumpy structures in high-z galaxies
- Notebooks compatible with Google Colab

### 2. Clumpy Galaxy Classification
Located in the `classification/` folder.

- Single-notebook classifier using ViTs to distinguish between clumpy and smooth ('non-clumpy') galaxies
- Uses the same image set as detection, with categorical morphology labels
- Includes training metrics

## Dataset

> **Note:** The full dataset is based on JWST-like mock images generated from the VELA simulation suite. The dataset is not included.

## Setup

```bash
git clone https://github.com/OshriFatkiev/vela-vision.git
cd vela-vision
conda env create -f environment.yml
conda activate vela-vision
jupyter notebook
