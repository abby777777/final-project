**Self-Supervised Tree Classification from Aerial Imagery**

Project Overview
This project explores the use of self-supervised learning techniques—MOCO-V3 (contrastive learning), MAE (Masked Autoencoders), and DINO (student/teacher modeling)—to classify tree species from aerial imagery at scale. The goal is to determine which method performs best and is most robust to distribution shifts when models are trained in one city (e.g., Los Angeles) and tested in another (e.g., New York).

Tree patterns are influenced by urban planning and human activity, creating unique signals in each city. By fine-tuning global models to local contexts, we aim to improve classification performance and assist urban ecologists in targeting replanting efforts to improve climate adaptation.

Problem Statement
Environmental monitoring and Earth observation from aerial imagery have the potential to enable policymakers to make data-informed decisions to facilitate societal adaptation to a changing climate. However, aerial and street-level data repositories are currently at the petabyte scale and growing, making manual extraction of useful information intractable without automation.

Automated tree genus classification from GPS-registered aerial imagery is increasingly of interest, with applications in humanitarian aid, disaster relief, agriculture, and urban mapping. Datasets like Auto Arborist enable the computer vision community to investigate automated methods for tree genus classification from aerial imagery at scale.

Research Questions
Primary Question: Which self-supervised learning method (MOCO-V3, MAE, DINO) performs best for tree classification from aerial imagery?
Secondary Questions:
How robust are these methods to distribution shifts between different cities?
What performance gains are achieved by fine-tuning models for specific cities?
How does teacher/student finetuning impact performance on statistical distribution shifts?
Objectives
Compare MOCO-V3, MAE, and DINO models to identify which handles city-to-city distribution shifts best.
Fine-tune a global model for specific cities and evaluate the performance boost from local adaptation.
Use statistical techniques like Maximum Mean Discrepancy (MMD) to analyze distribution shifts.
Investigate the impact of teacher/student finetuning on model performance.
Data Sources
Auto Arborist Dataset: Over 1 million images with genus labels for individual trees.
iNaturalist (iNat) Dataset: Over 1 million images retrieved via API.
iWildCam Dataset: Wildlife camera trap images for ecological studies.
Functional Map of the World (FMoW) Dataset: Satellite imagery for land use classification.

README.md
LICENSE
requirements.txt

Binder/

environment.yml
postBuild
Notebooks/

data_exploration.ipynb
moco_training.ipynb
mae_training.ipynb
dino_training.ipynb
finetuning.ipynb
evaluation.ipynb
Data/

auto_arborist/
inat/
iwildcam/
fmow/
Images/

samples/
visualizations/
Outputs/

models/
logs/
results/
Pre-Analysis Plan/

pre_analysis_plan.md


Acknowledgments
Datasets: Thanks to the creators of Auto Arborist, iNaturalist, iWildCam, and FMoW for providing the datasets.
Community: Appreciation to the open-source community for providing tools and resources that make this project possible.
References
Auto Arborist: Large-Scale Tree Classification Using Aerial Imagery
MOCO: Momentum Contrast for Unsupervised Visual Representation Learning
MAE: Masked Autoencoders Are Scalable Vision Learners
DINO: Emerging Properties in Self-Supervised Vision Transformers
Maximum Mean Discrepancy (MMD) for Distribution Shift Analysis

