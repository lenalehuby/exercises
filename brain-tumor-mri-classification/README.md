# brain-tumor-mri-classification
End-to-end pipeline for brain tumor MRI classification using Vision Transformers. Includes image preprocessing, simulation, model training, and evaluation with Hugging Face, PyTorch, and Colab GPU support.

## Project Overview
This project tackles a real-world medical imaging challenge: classifying human-brain MRI scans for tumor detection using cutting-edge vision transformer (ViT) models. Developed in collaboration with Brain-AI, the goal was to turn raw MRI images into actionable results for experts working in clinics and research labs. The end game? Fast, reliable, and accurate diagnosis with no second guessing.

### What’s Actually Inside
Functions to preprocess, visualize, and reconstruct MRI image data.

MRI simulation routines to generate realistic data variants for research and reconstruction testing.

An AI module built from Hugging Face’s Transformers and PyTorch, to tell apart healthy brains from those showing tumor signs.

Full training/evaluation pipelines, with step-by-step accuracy tracking and sample predictions.

Project targets at least 95% classification accuracy, but realistically you’ll want to run a few more tests.

### Key Technologies
Python—Colab notebook friendly for GPU speed

Hugging Face Transformers, PyTorch (core modeling)

OpenCV, Plotly, scikit-learn, Matplotlib, pandas (for visualization, exploration, and wrangling data)

### Milestones
Processing, Visualizing, and Reconstructing MRI Data — milestone-1.ipynb

Training a Vision Transformer for Brain Tumor Classification — milestone-2.ipynb

### Why Use This?
If you need to build or prototype state-of-the-art medical image classifiers, this project gives you the full workflow: from noisy MRI images to automated tumor detection using deep learning, transformer architectures, and practical visualization. Whether you’re a data scientist, ML engineer, or a biomedical tinkerer, these notebooks are a launching pad for your own experiments.

#### License

This is mainly meant for learning and tinkering, not commercial use.
