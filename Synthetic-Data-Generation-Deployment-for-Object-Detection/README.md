# Synthetic-Data-Generation-Deployment-for-Object-Detection-
Project from NVIDIA training - NVIDIA DLI Hands-On Pipeline

## Project Overview
This repository contains my hands-on solutions and workflows from an NVIDIA Deep Learning Institute (DLI) training focused on synthetic data generation for object detection. Guided by the course creators, this fictional case study dives into the how and why of generating artificial datasets for computer vision pipelines, especially when real-world data is expensive, laborious to label, or just not diverse enough.

Throughout this mini-project, the focus is on a simple but surprisingly sticky example: fruit detection on a food production line. The process aims to answer questions like, “What if you could quickly train an object detection model using totally artificial but perfectly labeled data, and then actually know your model will generalize to real-world challenges?” While the pipeline is demo-friendly, the concepts closely mirror real industry pains.

The work here covers the complete synthetic data journey:

Synthetic Data Generation: Using Omniverse Replicator (inside a GUI and via scripts) to build 3D scenes, randomize elements, and export large, annotated, physically accurate datasets that would be tough to collect by hand.

Model Training: Taking the generated data and fine-tuning a PyTorch object detection model. The hope is to quickly see the value of synthetic data in boosting model performance and coverage, even on edge cases.

Deployment: Serving the trained model on NVIDIA Triton to show the “last mile” of a computer vision pipeline, from training all the way to actual inference in production.

Visualization & Export: Visualizing and exporting results to track both model learning and the diversity of the generated synthetic sets.

Realistically, in industry, you might not always get to control the whole pipeline (data, training, and deployment), but this training makes it easy to experiment with every stage. Like the examples shown in the course, every notebook and script is meant for rapid prototyping, flexible re-use, and plenty of tinkering.

### What’s Inside?

0_generate_data_headless.ipynb – Jupyter notebook for generating synthetic data (headlessly, no GUI required)

generate_data_headless.py – Python script for running generation straight from the terminal

1_visualize.ipynb – Notebook for visualizing generated scenes and annotations

2_train.ipynb – Fine-tune or train an object detection model (using PyTorch) on the synthetic dataset

3_export.ipynb – Export generated assets, model weights, or visualizations for reuse

4_deploy.ipynb – Deploy and run the trained model using NVIDIA Triton Inference Server

### Why Synthetic Data?

Sometimes you just don’t have enough real data. Maybe collecting tomatoes on a conveyor belt sounds simple, until you try to cover every lighting condition, fruit type, or batch error you might see in production. Synthetic data lets you build big, diverse, and well-labeled datasets cheaply and repeatably. It also gives you annotation types (like depth or object speed) you can’t even capture with a normal camera.

### Getting Started

All code is in Python (notebooks and scripts). If you want to run it locally or extend for your own experiments, start with the data generation notebooks and .py scripts, then move through training, visualization, and deployment.

Requirements: Jupyter notebook, NVIDIA Omniverse Replicator setup, PyTorch, Triton Inference Server

Steps: Generate → Visualize → Train → Export → Deploy

### A Note on Scope

While the core example is a fruit detection pipeline for a food factory, the workflow and code are relevant to any domain where annotated image data is a bottleneck. If you’re interested in industrial, robotics, or perception model training, consider this a template for building it yourself.

### License
This is mainly meant for learning and tinkering, not commercial use.
