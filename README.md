# Pore Network Model Metrics Extraction Tool Using SNOW2 and OpenPNM from Segmented 3D Volumes

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
  - Percolating porosity
  - Pore size distribution (PSD)
  - Permeability
  - Tortuosity
  - Dead-end pore fraction
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