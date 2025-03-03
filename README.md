# Facial Emotion Recognition Preprocessing

This project preprocesses facial emotion images for machine learning tasks. It includes image resizing, normalization, and data augmentation to improve model training.

## Dataset

The dataset can be downloaded from:
[Facial Emotion Dataset](https://drive.google.com/drive/folders/1TnAcsAoBxsXP2NP3SXI6OEV_wHe_b-PA?usp=drive_link)

After downloading, place the dataset in the project directory at:
```
D:\Mini ML\archive (3)
```

## Features

- Image resizing to 224x224 pixels
- RGB color space conversion
- Pixel normalization (0-1 range)
- Data augmentation using Albumentations:
  - Horizontal flipping (30% probability)
  - Random rotation (±15 degrees)
  - Random brightness and contrast adjustments

## Requirements

The project requires Python 3.13+ and the following packages:
```
numpy>=2.0.0
opencv-python>=4.8.0
albumentations>=1.3.1
scikit-learn>=1.4.0
tqdm>=4.66.1
```

To install the requirements:
```bash
pip install -r requirements.txt
```

## Project Structure

```
Mini ML/
├── archive (3)/          # Original dataset directory
│   ├── train/           # Training images
│   └── test/            # Testing images
├── processed_data/       # Output directory for preprocessed images
├── preprocessing.py      # Main preprocessing script
├── requirements.txt      # Package dependencies
└── README.md            # This file
```

## Usage

1. Download the dataset from the provided Google Drive link
2. Install the requirements using pip
3. Run the preprocessing script:
```bash
python preprocessing.py
```

The preprocessed images will be saved in the `processed_data` directory, maintaining the same folder structure as the original dataset. 