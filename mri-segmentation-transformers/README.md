# mri-segmentation-transformers
End-to-end pipelines for brain MRI tumor segmentation using transformer models (SegFormer and MaskFormer). Includes dataset exploration, custom accuracy metrics, model training, and performance benchmarking on real medical data.

## Project Overview
Welcome to the world of biomedical imaging with transformers! This project is all about automating brain MRI segmentation: taking stacks of scan slices and letting deep learning models find tumors faster, more consistently, and without anyone squinting at pixels for hours. Manual segmentation has its place, but with modern AI (especially transformer models), we’re aiming for something far more scalable.

### What’s Happening Inside
A real neuroscience lab MRI dataset—prepping images and ground-truth masks for model training.

The pipeline explores, preprocesses, and benchmarks two transformer-based segmentation models: SegFormer and MaskFormer.
Custom segmentation metrics will let us compare their accuracy and efficiency, side by side.

Visualization notebooks show what the models see, how they segment, and where they might get confused.

### Key Technologies
Python (Google Colab for GPU-powered doodling)

Hugging Face Transformers (for SegFormer, MaskFormer)

PyTorch, OpenCV, Plotly, scikit-learn, Matplotlib, pandas (for loading, augmentation, and analysis)

### Milestones
Dataset Exploration & Segmentation Metric — Segmentation_metric.ipynb

Brain MRI Segmentation with SegFormer — Segmentation_SegFormer.ipynb

Brain MRI Segmentation with MaskFormer — Segmentation_Maskformer.ipynb

### Why Use This?
If you want to build, evaluate, or deploy state-of-the-art segmentation for medical imaging—with the ability to adapt metrics, visualize results, and compete models—this project is your launchpad. 
