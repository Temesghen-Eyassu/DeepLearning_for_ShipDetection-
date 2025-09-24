# DeepLearning_for_ShipDetection

This repository contains datasets, Colab notebooks, and scripts for ship detection using Sentinel-1 SAR imagery with UNet + VGG16 deep learning models. It is designed to help researchers and practitioners experiment with ship detection, train models, and evaluate results.

## Contents

- `LabelFinal.tif` – Ground truth labels for ship locations.  
- `S1_VV_VH_fullSeaShips.tif` – Sentinel-1 SAR imagery covering full sea regions.  
- `Patches/` – Preprocessed image patches, organized into:  
  - `images/` – Input SAR image patches.  
  - `masks/` – Corresponding mask patches for training and evaluation.  
- `UNet_and_VGG16.ipynb` – Colab notebook for interactive exploration, training, and evaluation.  
- `Scripts/` – Helper Python scripts for data preprocessing, patch generation, and model inference.  

## How to Use

### Colab Notebook

1. Open `UNet_and_VGG16.ipynb` in Google Colab.  
2. Mount your Google Drive or point paths to local data files.  
3. Run the cells to preprocess data, train the model, or visualize predictions.  

### Scripts

Run preprocessing or inference scripts locally if you prefer not to use Colab.  
Scripts allow batch processing and integration into larger pipelines.  

## Notes

Large data files and trained models are tracked using Git LFS, so they are included in the repository without exceeding GitHub file limits.  

Ensure Git LFS is installed when cloning the repository:

```bash
git clone https://github.com/Temesghen-Eyassu/DeepLearning_for_ShipDetection-.git
git lfs pull
