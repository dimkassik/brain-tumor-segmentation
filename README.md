# Brain Tumor Segmentation with U-Net

## Dataset
- Source: Kaggle (LGG MRI Segmentation Dataset)
- Images: MRI brain scans (128×128, grayscale)
- Masks: Binary tumor segmentation masks

## Project Structure
- `01_baseline_cnn_unet.py` – baseline comparison (CNN vs U-Net)
- `02_unet_bs16_lr001.py` – extended training (BS=16)
- `03_unet_bs32_lr001.py` – batch size comparison
- `04_unet_final_augmentation.py` – final model with augmentation

## Best Model
- Architecture: U-Net
- Learning rate: 0.001
- Batch size: 16
- Dice (validation): ~0.76
- IoU (validation): ~0.73

## How to Run
```bash
pip install -r requirements.txt
python src/04_unet_final_augmentation.py
