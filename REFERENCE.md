# 🌿 SmartHarvest: A Hybrid Neural Engine for Precision Agriculture

[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-emerald)](https://ab5ef0e396e44cdf31.gradio.live)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-green.svg)](https://www.python.org/)
[![Framework: PyTorch](https://img.shields.io/badge/framework-PyTorch-orange.svg)](https://pytorch.org/)

**SmartHarvest** is a high-performance agricultural intelligence system that synthesizes soil chemistry and climatic dynamics to provide instantaneous, high-confidence crop recommendations. By merging **Nature with Code**, this project demonstrates how deep learning can secure a more resilient and data-driven future for global food systems.

---

## 🚀 The Architecture 
Unlike standard classifiers, SmartHarvest utilizes a **Hybrid Neural Pipeline** inspired by advanced sequence modeling and pattern recognition:

1. **Feature Synthesis (NB15):** An encoder bottleneck that compresses high-dimensional nutrient data into a dense latent space.
2. **Local Correlation (NB11):** 1D-Convolutional layers (1D-CNN) to extract specific patterns between Nitrogen, Phosphorus, and Potassium.
3. **Global Context (NB14):** A Multi-Head Self-Attention layer that dynamically prioritizes critical factors (e.g., Rainfall over pH) based on the specific environmental matrix.
4. **Sequential Memory (NB12):** LSTM units to process the relationship between fluctuating temperature and humidity signatures.

## 📊 Evaluation Rigor
To ensure the engine is production-ready, I implemented a rigorous testing framework:
* **Baseline Benchmark:** Established a Logistic Regression model to quantify the "Neural Lift" provided by the hybrid architecture.
* **Performance Metrics:** Prioritized **Weighted F1-Scores** to manage the **Bias-Variance Trade-off (NB 4A)** across all 22 crop classes.
* **Diagnostic Visualization:** Integrated Training Convergence plots and Confusion Matrix Heatmaps to verify zero "cross-talk" between similar crop signatures.

## 🧪 Field Parameters Analyzed
The model synthesizes seven critical variables to generate a prediction:
- **Nutrients:** Nitrogen (N), Phosphorus (P), Potassium (K)
- **Climate:** Temperature, Humidity, Rainfall
- **Soil Integrity:** pH Balance
