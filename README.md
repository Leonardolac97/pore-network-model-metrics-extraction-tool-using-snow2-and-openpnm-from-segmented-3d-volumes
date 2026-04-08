# Pore Network Model Metrics Extraction Tool Using SNOW2 and OpenPNM from Segmented 3D Volumes

## Citation

This software is archived at:
https://doi.org/10.xxxx/xxxxx](https://doi.org/10.35097/wx033rkaeuzp5ynr

## Description

This repository provides a Python-based workflow for extracting pore network model (PNM) metrics from segmented 3D tomographic datasets. The tool is designed for labeled volumetric data (e.g., from X-ray tomography), where the pore space is explicitly segmented.

The workflow integrates:
- PoreSpy (SNOW2 algorithm) for network extraction
- OpenPNM for network analysis and transport simulations

## Features

- Import of 3D labeled TIFF volumes
- Validation of phase labels (0: outside, 1: solid, 2: pore)
- Pore network extraction using SNOW2
- Computation of:
  - Total porosity
  - Throat size distribution
  - Coordination distribution
  - Pore size distribution (PSD)
- Optional 3D visualization

 ## Input Requirements 

- 3D TIFF file (segmented volume)
- Label convention:
  - 0 = outside domain
  - 1 = solid phase
  - 2 = pore phase

## Installation

Install dependencies using:

```bash
pip install -r requirements.txt
