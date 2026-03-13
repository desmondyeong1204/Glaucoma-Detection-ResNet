# 👁️ Project TomatoFriedEgg: Explainable Glaucoma Detection
**Developed for the IDSC 2026 Data Science Hackathon** *Theme: Mathematics for Hope in Healthcare*

## 🌟 Overview
Project TomatoFriedEgg is an AI-driven screening tool designed to detect **Glaucomatous Optic Neuropathy (GON)** from retinal fundus images. Using a Transfer Learning approach with a ResNet-34 architecture, the model achieves a high diagnostic accuracy of **95.3%**. 

To align with the "Hope in Healthcare" theme, we integrated **Grad-CAM Interpretability**, ensuring that the model's decisions are transparent and clinically verifiable by medical professionals.

## 📥 Model Download
Due to GitHub's file size restrictions, the trained model weights are hosted externally.
* **[Download Trained Model (.pkl) Here]((https://drive.google.com/drive/folders/1H0_AJZ5ybZIpcK4ViaSC4HsJ-w-i9J0t?usp=sharing))**

## 📊 Technical Specifications
- **Architecture:** ResNet-34 (Pre-trained on ImageNet)
- **Framework:** FastAI & PyTorch
- **Dataset:** Hillel Yaffe Glaucoma Dataset (HYGD) - A "Gold-Standard" annotated dataset.
- **Hardware:** Trained on a Google Colab T4 GPU instance.
- **Accuracy:** 95.3%
- **Interpretability:** Gradient-weighted Class Activation Mapping (Grad-CAM).

## 🩺 Clinical Interpretability (The "Why")
In healthcare, a "Black Box" AI is not enough. Our model uses Grad-CAM to highlight exactly where the neural network is "looking." As seen in the results within the notebook, the model consistently focuses on the **optic disc** and **neuroretinal rim**, which are the key physiological areas used by ophthalmologists for diagnosis.

## 📂 Repository Structure
- `TomatoFriedEgg.ipynb`: The complete training, evaluation, and interpretability pipeline.
- `Labels.csv`: Reference for dataset ground-truth labels.
- `Images/`: (Referenced from the HYGD dataset).

## 🚀 How to Run
1. Open the `.ipynb` file in Google Colab.
2. Ensure your Runtime Type is set to **T4 GPU**.
3. Run the cells sequentially to reproduce the results and Grad-CAM heatmaps.

---
**Team:** TomatoFriedEgg (Solo)  
**Competition:** IDSC 2026 (UPM x UNAIR)
