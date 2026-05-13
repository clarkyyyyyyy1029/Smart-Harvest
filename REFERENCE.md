# 🌿 SmartHarvest: A Hybrid Neural Engine for Precision Agriculture

[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-emerald)](https://bb09dec369c6716e77.gradio.live)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-green.svg)](https://www.python.org/)
[![Framework: PyTorch](https://img.shields.io/badge/framework-PyTorch-orange.svg)](https://pytorch.org/)

📖 SmartHarvest: Technical Reference & Blueprint
This document provides the architectural mapping and scientific justification for the SmartHarvest Hybrid Neural Engine.
________________________________________
🏛️ 1. Neural Architecture (The Hybrid Pipeline)
The engine utilizes a custom CNN-LSTM-Attention hybrid architecture. This is not a simple classifier; it is a multi-stage synthesizer designed to map environmental signatures to biological requirements.
Layer Type	Purpose	Notebook Mapping
1D-CNN	Captures Spatial Correlations between Nitrogen, Phosphorus, and Potassium.	NB11
LSTM	Processes Sequential Dependencies in climatic variables (Temp/Humidity).	NB12
Self-Attention	Dynamically Weights critical factors (e.g., Rainfall vs. pH).	NB14
Encoder Bottleneck	Performs Feature Synthesis by compressing data into latent space.	NB15
________________________________________
🔍 2. Failure Analysis & Diagnostic Boundaries
No intelligent system is without limitations. To ensure academic rigor, the following “Confusion Zones” were identified during the validation phase:
A. Signature Overlap (Rice vs. Jute)
The model occasionally experiences high entropy when distinguishing between Rice and Jute.
•	Cause: Both crops share a 90% overlap in high-rainfall (>200mm) and high-humidity signatures.
•	Resolution: Future iterations will require soil texture data (Clay vs. Silt) to further resolve these boundaries.
B. Boundary Sensitivity
Predictions at the extreme edges of the pH scale (Highly Acidic < 4.5 or Highly Alkaline > 8.5) show a slight drop in precision.
•	Cause: These represent “Data Boundaries” where biological signatures begin to converge for multiple hardy crops.
________________________________________
📊 3. Dataset & Data Sources
The SmartHarvest engine is trained on high-fidelity agricultural data.
Primary Training Data
•	File Name: Crop_recommendation.csv
•	Source: Kaggle - Crop Recommendation Dataset
•	Description: Contains 2,200 instances with 8 attributes including N, P, K, Temperature, Humidity, pH, and Rainfall.
•	Role: This file serves as the ground truth for all supervised learning cycles in this project.
________________________________________
🧪 4. Evaluation Metrics
The project prioritizes the Weighted F1-Score over raw Accuracy. This ensures that the model is penalized for misclassifying “rare” crops, preventing the model from becoming biased toward the most common samples.
________________________________________
📜 5. References & Citations
1.	Hargreaves, G. H., & Samani, Z. A. (1985). Reference Crop Evapotranspiration from Temperature. Applied Engineering in Agriculture. (Used for climate weighting logic).
2.	Vaswani, et al. (2017). “Attention is All You Need.” (The mathematical basis for the Self-Attention mechanism in NB14).
3.	Kaggle Data Contributors. “Crop Recommendation Dataset.” [Online]. Available: https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset
________________________________________


