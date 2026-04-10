# sEEG Analysis

Multi-class CSP (Common Spatial Pattern) pipeline for stereo-electroencephalography (sEEG) signal classification.

## Features

- 4-class classification pipeline
- Bad channel detection
- Notch and bandpass filtering
- Local Mean Peak (LMP) feature extraction
- One-vs-Rest FBCSP features (HFB + LMP)
- CSP spatial pattern visualization
- Deep learning model support

## Dataset

Data should be organized in the `dataset/` folder with class-named subdirectories:
```
dataset/
  class_1_关一下灯/
  class_2_我冷了/
  ...
```

Each trial contains `.wav` and `.npz` files.

## Requirements

See `requirements.txt` for dependencies.

## Usage

Open and run the Jupyter notebooks:
- `seeg_full_pipeline.ipynb` - Main CSP pipeline
- `seeg_full_pipeline DL.ipynb` - Deep learning approach
- `seeg_full_pipeline Riemann.ipynb` - Riemannian geometry approach

## Model

Pre-trained model: `best_model.pth`