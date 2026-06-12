# CellTrackAI: Cell Tracking and Trajectory Prediction using Deep Learning

## Overview

CellTrackAI is an end-to-end computer vision and deep learning framework designed to track cell movements and predict future trajectories from microscopy image sequences.

The project combines traditional image processing techniques with sequence learning models to analyze cell dynamics, generate movement trajectories, classify behavioral patterns, and forecast future positions.

The framework was evaluated using microscopy datasets from the Cell Tracking Challenge and includes a comparative study between LSTM and Transformer-based trajectory prediction models.

---

## Key Features

- Cell detection using image preprocessing and contour-based segmentation
- Multi-object tracking across image sequences
- Trajectory extraction and visualization
- Cell activity heatmap generation
- Behavior classification based on movement patterns
- Future trajectory prediction using LSTM
- Transformer-based trajectory forecasting
- Model comparison using RMSE, ADE, and FDE metrics

---

## Project Pipeline

```text
Microscopy Images
        │
        ▼
Image Preprocessing
        │
        ▼
Cell Detection
        │
        ▼
Cell Tracking
        │
        ▼
Trajectory Extraction
        │
        ├────────► Heatmap Generation
        │
        ├────────► Behavior Classification
        │
        ▼
Trajectory Dataset Creation
        │
        ▼
LSTM / Transformer Models
        │
        ▼
Future Position Prediction
        │
        ▼
Performance Evaluation
```

---

## Dataset

**Dataset:** Fluo-N2DH-SIM+

**Source:** Cell Tracking Challenge

The dataset consists of fluorescence microscopy image sequences used for benchmarking cell detection and tracking algorithms.

---

## Technologies Used

| Category | Tools |
|-----------|---------|
| Programming | Python |
| Computer Vision | OpenCV |
| Deep Learning | PyTorch |
| Data Processing | NumPy, Pandas |
| Visualization | Matplotlib |
| Machine Learning | Scikit-Learn |
| Tracking | Hungarian Matching |
| Sequence Models | LSTM, Transformer |

---

## Model Performance

### LSTM

| Metric | Value |
|----------|----------|
| MSE | 0.00054 |
| RMSE | 0.02325 |
| ADE | 0.02552 |
| FDE | 0.02552 |

### Transformer

| Metric | Value |
|----------|----------|
| MSE | 0.00125 |
| RMSE | 0.03533 |
| ADE | 0.04729 |
| FDE | 0.04729 |

### Comparison

| Model | RMSE | ADE | FDE |
|---------|---------|---------|---------|
| LSTM | 0.02325 | 0.02552 | 0.02552 |
| Transformer | 0.03533 | 0.04729 | 0.04729 |

**Best Performing Model:** LSTM

The LSTM achieved lower prediction error across all evaluation metrics and demonstrated better performance on short trajectory sequences.

---

## Results

### Cell Detection

Add screenshot here

```
outputs/detection.png
```

### Trajectory Visualization

Add screenshot here

```
outputs/trajectory_map.png
```

### Activity Heatmap

Add screenshot here

```
outputs/heatmap.png
```

### Trajectory Prediction

Add screenshot here

```
outputs/lstm_prediction.png
```

---

## Repository Structure

```text
CellTrackAI/
│
├── CellTrack_model.ipynb
├── README.md
├── requirements.txt
│
├── outputs/
│   ├── trajectory_map.png
│   ├── heatmap.png
│   ├── lstm_prediction.png
│   ├── comparison_plot.png
│   └── tracking_demo.mp4
│
└── results/
    └── model_comparison.csv
```

---

## Future Improvements

- Multi-step trajectory forecasting
- Cross-dataset evaluation
- DeepSORT-based tracking
- Real-time trajectory prediction
- Graph Neural Network-based cell interaction modeling

---

## Author

Dhruv Shukla

---

## License

This project is released for educational and research purposes.
