# Dental White Lesion Detection

Semantic segmentation of dental white lesions in clinical images using a U-Net architecture trained on Google Colab with GPU acceleration.

## What this project does

Detects and segments white lesions in dental photographs — a computer vision approach to assist clinical image analysis. The model takes a grayscale dental image as input and outputs a pixel-level mask highlighting lesion regions.

## Approach

- **Architecture:** U-Net (encoder-decoder with skip connections)
- **Input:** Grayscale dental images, resized and normalized
- **Training:** 150 epochs, GPU (T4), Google Colab
- **Augmentation:** Horizontal flip, brightness variation
- **Inference:** Test-Time Augmentation (TTA) for improved robustness

## Results

| Metric | This model (TTA) | Literature (InceptionResNetV2) |
|--------|-----------------|-------------------------------|
| Dice | 0.61 | N/A |
| Precision | 0.61 | 0.28 |
| Recall | 0.74 | 0.81 |
| F1 | 0.61 | 0.42 |

## Status

Work in progress — additional data will be added in future iterations.

## Tech stack

Python · TensorFlow/Keras · PIL · Matplotlib · Google Colab
