🦷 Tooth Instance Analysis using U-Net

A deep learning project for segmenting teeth in panoramic dental X-ray images using the U-Net architecture.
This project automates tooth boundary detection and supports dental diagnostics by generating accurate segmentation masks.

📌 Project Overview

This project implements a U-Net-based image segmentation pipeline to automatically identify and segment individual teeth from X-ray images. It is designed to support dental practitioners by enabling faster and more accurate assessment of dental structures.

  The notebook includes:
  
  Dataset preprocessing
  
  Model architecture (U-Net)
  
  Training and validation
  
  Visualization of predictions
  
  Evaluation metrics

🚀 Features

  ✔ Fully implemented U-Net architecture for medical image segmentation
  
  ✔ Supports grayscale panoramic dental X-rays
  
  ✔ Automatic mask generation
  
  ✔ Training pipeline with callbacks
  
  ✔ Visualization of model predictions
  
  ✔ Easily extendable to instance or semantic segmentation

📂 Project Structure
Tooth_Instance_Analysis/
│── Tooth_Instance_Analysis.ipynb   # Complete training + inference pipeline
│── data/
│     ├── images/                   # Input X-ray images
│     └── masks/                    # Ground-truth segmentation masks
│── README.md

🧠 Model Architecture

This project uses the U-Net architecture, specifically designed for biomedical image segmentation.
U-Net is chosen because:

  It works well on small datasets
  
  It preserves spatial information via skip connections
  
  It generates pixel-accurate segmentation masks

Key components:

  Encoder: feature extraction
  
  Decoder: upsampling and spatial reconstruction
  
  Skip connections: retain fine-grained details

🛠 Tech Stack
| Component            | Technology         |
| -------------------- | ------------------ |
| Language             | Python             |
| Deep Learning        | TensorFlow / Keras |
| Processing           | NumPy, OpenCV      |
| Visualization        | Matplotlib         |
| Training Environment | Google Colab       |


📥 Installation

Clone the repository:

    git clone https://github.com/yourusername/Tooth_Instance_Analysis.git
    cd Tooth_Instance_Analysis



Install dependencies:

    pip install tensorflow numpy opencv-python matplotlib scikit-learn


▶️ How to Run

1. Open Tooth_Instance_Analysis.ipynb in Jupyter or Google Colab

2. Mount your dataset

3. Set the correct dataset paths

4. Run all cells to:

    preprocess images
    
    train the U-Net model
    
    evaluate results
    
    generate segmentation masks

📊 Results

The model outputs:

  Predicted masks
  
  Overlay visualizations: X-ray + predicted mask
  
  Training curves (loss & accuracy)

You can modify thresholding to refine segmentation boundaries.

🔧 Customization

You can extend this project to:

  Multi-class segmentation
  
  Tooth numbering / labeling
  
  Instance segmentation using Mask R-CNN
  
  Post-processing (contour extraction, polygon mapping)

🤝 Contributions

Pull requests and improvements are welcome — especially enhancements related to:

  Better preprocessing
  
  Improved U-Net variants
  
  Post-processing and evaluation methods

📜 License

This project is released under the MIT License.
