# Lumbar Spinal Stenosis Detection using YOLOv8

## Overview
This project focuses on the detection and classification of lumbar spinal stenosis from sagittal MRI images using the YOLOv8 deep learning model.

The work is derived from our group research project published at the ICOFE-2024 conference. This repository presents the implementation of the proposed approach, covering data preprocessing, object detection, and evaluation workflows for medical image analysis.

## Research Reference

**Paper:** Lumbar Spinal Stenosis Degenerative Detection and Classification on MRI Images  
🔗 Link: <https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5088833>

## Research Background
**Paper Title:** Lumbar Spinal Stenosis Degenerative Detection and Classification on MRI Images  
**Conference:** ICOFE 2024  
**Authors:** Ishita Savale et al.

The proposed approach utilizes the YOLOv8s model to detect lumbar spinal levels (L1–S1) and classify the severity of spinal stenosis into three categories:
Normal/Mild, Moderate, and Severe.

## Dataset
- Source: RSNA 2024 Lumbar Spine Degenerative Classification dataset
- Modality: Sagittal T2-weighted MRI images
- Format: DICOM (.dcm)
- Total Images: 3031

Due to dataset size and privacy constraints, the full dataset is not included in this repository.

## Methodology
1. DICOM to JPG conversion with normalization
2. Annotation generation using spinal level coordinates
3. YOLOv8s model training and fine-tuning
4. Model evaluation using precision, recall, and mAP metrics

## Model & Tools
- Python
- YOLOv8 (Ultralytics)
- OpenCV
- NumPy, Pandas
- PyTorch

## Results (from published research)
- Precision: 0.85
- Recall: 0.91
- mAP@50: 0.91

## Disclaimer
This repository contains the implementation of a research project published at the ICOFE-2024 conference on lumbar spinal stenosis detection using YOLOv8.

## Future Work
- Reduce model complexity
- Improve inference speed
- Extend to multi-condition spinal diagnosis
