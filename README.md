# CellTrackAI

Cell tracking and trajectory prediction framework built using OpenCV, LSTM, and Transformer models.



## Overview

This project performs:

- Cell Detection
- Cell Tracking
- Trajectory Extraction
- Heatmap Generation
- Behavior Classification
- Future Trajectory Prediction

using microscopy image sequences from the Cell Tracking Challenge dataset.


## Pipeline


Microscopy Images
        ↓
Preprocessing
        ↓
Cell Detection
        ↓
Cell Tracking
        ↓
Trajectory Extraction
        ↓
Behavior Analysis
        ↓
LSTM / Transformer
        ↓
Future Position Prediction


## Results

| Model       | RMSE   | ADE    | FDE    |
| ----------- | ------ | ------ | ------ |
| LSTM        | 0.0233 | 0.0255 | 0.0255 |
| Transformer | 0.0353 | 0.0473 | 0.0473 |

## Technologies

- Python
- OpenCV
- NumPy
- Pandas
- Matplotlib
- PyTorch
- Scikit-Learn


## Dataset


Dataset:
Fluo-N2DH-SIM+

Source:
Cell Tracking Challenge



## Key Findings

- Successfully tracked cell movements across image sequences.
- Generated trajectory maps and activity heatmaps.
- Classified cell behavior based on movement speed.
- LSTM outperformed Transformer on small trajectory datasets.