Capsule Networks: Dynamic Routing, Pose Encoding, and Robust Representation Learning

This repository contains all code, results, and the final tutorial report for the assignment on Capsule Networks (CapsNets).
The project investigates how dynamic routing, pose-aware representations, and reconstruction-based regularisation contribute to capsule behaviour on MNIST.

Repository Structure
├── notebooks/
│   └── raju_kumar_code_ml.ipynb      # Full implementation & experiments
│
├── figures_capsnet/
│   ├── capsnet_training_losses.png
│   ├── capsnet_reconstructions.png
│   ├── capsnet_rotation_robustness.png
│   └── capsnet_routing_vs_accuracy.png
│
├── tutorial.pdf                       # Final assignment report
├── LICENSE                             # MIT License
└── README.md                           # This file

Project Overview

Capsule Networks, introduced by Sabour, Frosst & Hinton (2017), were designed to overcome limitations of CNNs by modelling both entity presence and pose via vector outputs.
This repository explores:

Dynamic routing-by-agreement

Capsule-based pose encoding

Reconstruction as regularisation

Robustness to rotations

Effect of routing iterations on accuracy

The experiments follow the methodology described in the tutorial and reproduce all figures automatically.

How to Run the Notebook
1. Clone the repository:
git clone https://github.com/Rajusareddy1203/machinelearning.git
cd raju_kumar_code_ml.ipynb

2. Install dependencies:
pip install torch torchvision matplotlib numpy

3. Run the Jupyter Notebook:
jupyter notebook notebooks/capsnet_experiments.ipynb


Executing all cells will generate every figure stored in the figures_capsnet/ folder.

Dataset Description

The notebook uses the MNIST handwritten digits dataset:

60,000 training samples

10,000 testing samples

Grayscale, 28×28 images, ten classes

A subset of 10,000 training and 2,000 test images is used for faster experimentation.
No further preprocessing is necessary beyond normalisation.

Figures Generated

The notebook automatically saves:

Training losses (margin + reconstruction)

Reconstruction grid comparing original vs reconstructed digits

Rotation robustness curve

Routing iterations vs accuracy plot

All images include alt text descriptions in the report for accessibility.

Accessibility Notes

Colour-blind-friendly palettes

High-contrast plots

Clear headings for screen readers

Alt text provided for every figure

No colour-only cues used in tables or diagrams

License

This project is released under the MIT License.
