# ML-for-microplastics
This repository contains experimental evaluations of deep learning models for automated microplastic image segmentation. Image segmentation plays a crucial role in automating microplastic analysis, as it allows not only detection but also pixel-level delineation of particle boundaries, shapes, and sizes. We experimentally evaluated two approaches: the task-specific MP-Net architecture and the more general Segment Anything Model (SAM).
1. MP-Net Experiment
Dataset: MP-Set (publicly available on Kaggle)

Fluorescence microscopy images of Nile Red stained microplastics
Nile Red is a lipophilic fluorescent dye that preferentially binds to plastics
Images divided into 256x256 patches (73 total patches)
Training: 60 patches | Testing: 13 patches

Model Architecture:

U-Net architecture with ResNet encoder
Pre-trained ImageNet weights for transfer learning
Fine-tuned on MP-Set training data

2. Segment Anything Model (SAM) Experiment
Model Characteristics:

Foundation model for image segmentation
Promptable model (masks, points, boxes, or text prompts)
Zero-shot generalizability
Combines interactive and automatic segmentation capabilities

Datasets Tested:

Stereomicroscopic microplastic images
SEAMaP images (without available segmentation masks)
