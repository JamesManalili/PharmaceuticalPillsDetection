# Pharmaceutical Pill Detection with YOLOv8 and EasyOCR

This pharmaceutical pill detection system utilizes a YOLOv8s model trained on a dataset of 9,603 images, preprocessed with auto-orientation correction and stretch resizing to 640×640 pixels. The model achieves exceptional performance with 97.2% mAP, 95.7% precision, and 99.1% recall, demonstrating highly reliable pill localization even under varying lighting and orientation conditions. Trained for 50 epochs with mosaic augmentation and AdamW optimization, the system combines these detections with EasyOCR text recognition to verify pill identities through text pattern matching (threshold: 0.6 similarity). 

## 📊 Performance Metrics
| Metric        | Score   |
|---------------|---------|
| mAP@0.5       | 97.2%   |
| Precision     | 95.7%   |
| Recall        | 99.1%   |

- __Confusion Matrix__

![confusion_matrix](https://github.com/user-attachments/assets/b8f70581-7fa1-4240-b504-6ca08d4e4531)

- __Precision Confidence Curve__

![P_curve](https://github.com/user-attachments/assets/bf96b547-739d-4fd1-a44b-930586e4eed6)

- __Recall Confidence Curve__

![R_curve](https://github.com/user-attachments/assets/e97a9660-2f39-4b9a-9781-f8c776414e44)

## Dataset Specifications
| Attribute          | Value       |
|--------------------|-------------|
| Total Images       | 9,603       |
| Preprocessing      | Auto-orient + Resize (Stretch to 640×640) |
| Train/Val/Test Split | 70%/20%/10% |


## 🚀 Features
- High-accuracy pill detection (YOLOv8)
- Text recognition (EasyOCR)
- Text-to-class verification system
- Visual output with detection boxes
- Configurable similarity threshold

