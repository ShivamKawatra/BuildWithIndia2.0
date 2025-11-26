# Build With India Hackathon - Object Detection Submission

## Project Overview
This submission contains a complete YOLO object detection model trained using synthetic data from Duality AI's Falcon platform.

## Quick Reproduction Guide

### Prerequisites
- Google account with access to Google Colab
- Duality AI Falcon account (free registration)

### Step-by-Step Reproduction

1. **Access Training Environment**
   - Go to https://falcon.duality.ai/
   - Navigate to Exercise 3 → Google Colab path
   - Open the provided Colab notebook

2. **Setup and Training**
   - Connect to GPU runtime (Runtime → Change runtime type → GPU)
   - Run all cells sequentially
   - Training takes 1-2 hours with GPU

3. **Expected Results**
   - Final mAP@0.5: 67.3%
   - Model weights saved as best.pt
   - Results in runs/ folder

## File Structure

```
SUBMISSION/
├── README.md                    # This file
├── HACKATHON_REPORT.pdf        # Complete 8-page report
├── model/
│   └── best.pt                 # Trained model weights
├── results/
│   ├── confusion_matrix.png    # Performance visualization
│   ├── training_curves.png     # Loss/accuracy graphs
│   └── results.csv            # Training metrics
├── code/
│   └── syntheticDataWorks_multiclass.ipynb
└── documentation/
    ├── methodology.md
    ├── performance_analysis.md
    └── challenges_solutions.md
```

## Performance Metrics
- **mAP@0.5**: 67.3%
- **Training Time**: 67.3 hours
- **Model Architecture**: YOLOv8
- **Dataset**: Falcon synthetic data (5GB)

## Usage Instructions

### Loading the Model
```python
from ultralytics import YOLO
model = YOLO('model/best.pt')
results = model('path/to/image.jpg')
```

## Team Information
- **Team Name**: [Rakshak]
- **Members**: [Shivam Kawatra, Anjali Verma, Arpit Sharma, Abhishek Kumar Gupta, Kshitij Varshney, Dev Gaur]
- **Contact**: [shivamkawatra261205@gmail.com]
- **Submission Date**: [26/11/2025]

---
**Final Performance: mAP@0.5 = 67.3%**