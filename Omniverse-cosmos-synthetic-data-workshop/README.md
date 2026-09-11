# Omniverse-cosmos-synthetic-data-workshop
Notebook workflow for generating synthetic training data via NVIDIA Omniverse, Cosmos—build digital twins, simulate sensors, engineer prompts, and automate realistic data creation for factory Physical AI.

## Project Overview
This notebook is part of an intensive NVIDIA workshop on synthetic data generation and digital twins for Physical AI. The workflow brings together cutting-edge simulation (Omniverse) and the Cosmos family of AI models to solve one of the biggest challenges in AI for robotics and automation: getting enough safe, diverse, and photorealistic training data without the time and cost of capturing it in the real world.

### What Actually Happens
Create detailed digital twin 3D scenes using Omniverse, with all the physics and visual realism required for industrial AI tasks.

Generate structured ground-truth data (segmentation, depth, and motion) mimicking data from sensors like cameras, RGB-D, and lidar.

Use Cosmos Transfer to convert this structured simulation data into photorealistic video sequences customized by natural language prompts for precise scene control.

Add even more visual variety and data by using Cosmos Predict, a model that generates new videos from simple text prompts or extends sequences for “future scenarios.”

Automate synthetic data generation further with AI agents that assemble scenes, control simulations, run inference, and filter outputs for realism using Cosmos Reason.

The final datasets are used for robust, cost-effective training of perception, policy, and VLM (vision-language model) systems, tailored for industrial settings and real-world deployment.

### Why Is This Useful?
Physical AI, think robots, autonomous vehicles, and industrial automation, needs enormous and varied datasets for training, validation, and benchmarking. Real-world data takes ages and costs a fortune; simulation and synthetic data change the game. With this workflow, you can:

Rapidly generate massive, scalable, controllable datasets for nearly any vision or robotics task.

Fine-tune models for factory, warehouse, or autonomous systems without risk to equipment or personnel.

Experiment with prompts, parameters, and scenario variations to fit the exact needs of your research or deployment.

### Technologies
NVIDIA Omniverse for photorealistic digital twins

Cosmos Transfer & Predict for multimodal, prompt-driven data generation

Cosmos Reason for filtering samples by physical realism/common sense

Python Jupyter notebooks, GPU cloud environment (Colab or on-prem H100/A100)

### From Workshop to Real-World AI
The only thing included in this repo is the hands-on notebook for synthetic data workflows, enabling fast experimentation or extension for your own projects. Use it to learn, prototype, or kick off full-scale data pipelines for real-world automation or industrial Physical AI.
