🩹 Wound Image Segmentation using U-Net

📌 Project Overview

This project implements a deep learning-based wound segmentation model using the U-Net architecture. The model performs pixel-wise binary segmentation to identify wound regions from clinical images.

The objective is to demonstrate how convolutional neural networks can assist in automated wound assessment and AI-driven healthcare applications.

⸻

🎯 Objective

To develop and evaluate a U-Net-based segmentation model capable of accurately detecting wound regions in medical images, supporting:
	•	Wound area monitoring
	•	Healing progression analysis
	•	AI-assisted clinical decision support

⸻

🧠 Model Architecture
	•	Architecture: U-Net (Encoder–Decoder CNN with skip connections)
	•	Task: Binary image segmentation (Background vs Wound)
	•	Loss Function: Binary Cross Entropy + Dice Loss
	•	Optimizer: Adam
	•	Learning Rate: 1e-4
	•	Epochs: 20
	•	Framework: PyTorch

The Dice component helps address class imbalance by directly optimizing overlap between predicted and ground truth masks.

⸻

📊 Training Performance
	•	Final Training Dice Score: ~0.72
	•	Final Test Dice Score: ~0.79
	•	Training Loss converged smoothly across epochs

The model demonstrates consistent convergence and reasonable segmentation performance despite limited dataset size and class imbalance.

⸻

🖼 Sample Predictions

The model successfully localizes wound regions across different image samples.
Visual outputs include:
	•	Original Image
	•	Ground Truth Mask
	•	Predicted Mask
	•	Overlay Visualization

(See notebook for full visual results.)

⸻

⚠ Limitations
	•	Limited dataset size
	•	Class imbalance (small wound region vs large background)
	•	No advanced augmentation techniques applied

⸻

🛠 Tech Stack
	•	Python
	•	PyTorch
	•	NumPy
	•	OpenCV
	•	Matplotlib
