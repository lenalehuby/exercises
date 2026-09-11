# construction-site-object-detection-transformers
Object detection pipeline for construction site surveillance using transformer models and Roboflow datasets. Covers vehicle tracking and building defect identification with DETR-family models, dataset creation, augmentation, and benchmarking.

## Project Overview
How do you keep an eye on a construction site that sprawls over a square kilometer? In this project, AI picks up the slack: transformer-powered computer vision models automatically spot vehicles, detect building cracks, and identify structural faults using powerful object detection workflows. Designed for AI-aided surveillance, these notebooks turn tricky human inspection jobs into streamlined, data-driven dashboards.

# What's inside
Prepping and augmenting datasets for construction vehicles and building defects (cracks, fissures, more) using both Hugging Face and Roboflow platforms.

Explore the ins and outs of multi-class dataset creation—combining disparate Roboflow collections into one format for transformer training.

Train and benchmark three state-of-the-art object detection models: DETR, conditional DETR, and Deformable DETR.

Evaluate model performance on real and varied images, tuning to find the best fit for clients who want fewer false alarms and more reliable safety checks.

### Technologies
Python (notebooks, data processing, augmentation)

Hugging Face Transformers (DETR, conditional DETR, Deformable DETR)

Roboflow (dataset aggregation, augmentation, annotation tools)

PyTorch, scikit-learn, Matplotlib, pandas for training and evaluation

### Milestones
Construction vehicle detection with Transformers — milestone-2.ipynb

Building crack detection with Transformers — milestone-3.ipynb (part 1: single-class, part 2: multi-class, using Roboflow datasets)

### What Stands Out
End-to-end pipeline: from downloading raw images/annotations to performance visualizations and models.

Multi-client support: tailor models for both vehicle tracking and defect detection, with options for fine-tuning expanded datasets.

Practical lessons: master Hugging Face object detection, Roboflow data wrangling, and real-world model evaluation.
