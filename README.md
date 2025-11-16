<p align="center">
  <img src="https://github.com/I-Sumit-kumar/Automated-Tooth-Instance-Analysis/assets/your-image-url-or-logo.png" width="100" alt="Tooth Logo">
</p>

<h1 align="center">🦷 Automated Tooth Instance Analysis using U-Net</h1>
<p align="center">
  <b>Segmentation and boundary detection for teeth in panoramic dental X-ray images</b>
  <br>
  <i>Deep learning applied to dental diagnostics, using U-Net.</i>
</p>

---

## 📌 Overview

Automated Tooth Instance Analysis leverages the power of <b>U-Net</b> for precise segmentation of teeth from panoramic dental X-ray images. It streamlines tooth boundary detection, generating accurate segmentation masks to assist dental professionals in diagnostics.

<p align="center">
  <img src="https://github.com/I-Sumit-kumar/Automated-Tooth-Instance-Analysis/assets/sample_xray_pred.png" width="600" alt="X-ray Sample Prediction">
  <br>
  <i>Example: Predicted mask (blue) overlayed on an X-ray image</i>
</p>

---

## 💡 Features

- ✅ **U-Net Architecture**: End-to-end training pipeline for medical image segmentation.
- ✅ **Panoramic X-ray Support**: Handles grayscale dental X-rays.
- ✅ **Automatic Mask Generation**: Accurately segment individual teeth.
- ✅ **Visualization**: Prediction overlays and training curves.
- ✅ **Customizable & Extendable**: Supports instance/semantic segmentation, post-processing, and more.

---

## 📂 Project Structure

```
Tooth_Instance_Analysis/
├── Tooth_Instance_Analysis.ipynb   # Jupyter notebook: training + inference
├── data/
│   ├── images/                     # Input X-ray images
│   └── masks/                      # Ground-truth segmentation masks
├── README.md
```

---

## 🧠 Model Architecture

U-Net is especially powerful for biomedical segmentation tasks:
- Works effectively with small datasets
- Preserves spatial info via skip connections
- Produces pixel-level segmentation masks

**Main Components:**
- **Encoder**: Feature extraction through convolutions
- **Decoder**: Upsampling and spatial reconstruction
- **Skip Connections**: Retain fine details at each scale

---

## 🛠 Technology Stack

| Component            | Technology              |
| -------------------- | ---------------------- |
| Language             | Python                 |
| Deep Learning        | TensorFlow / Keras     |
| Image Processing     | NumPy, OpenCV          |
| Visualization        | Matplotlib             |
| Training Environment | Google Colab/Jupyter   |

---

## 📥 Installation

**Clone the repository**
```bash
git clone https://github.com/I-Sumit-kumar/Automated-Tooth-Instance-Analysis.git
cd Automated-Tooth-Instance-Analysis
```

**Install dependencies**
```bash
pip install tensorflow numpy opencv-python matplotlib scikit-learn
```
---

## ▶️ How to Run

1. Open `Tooth_Instance_Analysis.ipynb` in Jupyter Notebook or Google Colab
2. Mount/load your dataset (`data/images/` & `data/masks/`)
3. Set dataset paths in notebook as required
4. Run all cells sequentially:
    - Preprocess images
    - Train the U-Net model
    - Evaluate segmentation performance
    - Visualize predictions & metrics

---

## 📊 Results

- **Predicted Masks**: For each X-ray image
- **Overlay Visualizations**: Input X-ray + predicted mask
- **Training Curves**: Loss & Accuracy
- *Tip:* Adjust thresholding to fine-tune boundaries.

---

## 🔧 Customization Ideas

- Multi-class segmentation (e.g., types of teeth)
- Tooth numbering/labeling
- Instance segmentation (e.g., upgrade to Mask R-CNN)
- Post-processing: contour extraction, polygon mapping

---

## 🤝 Contributions

Pull requests and feature suggestions are welcome!
- Improved data preprocessing
- Enhanced U-Net variants (attention, residual, etc.)
- Better post-processing
- New evaluation methods

---

## 📜 License

`MIT License`.

---

<p align="center">
  <em>Empowering dental AI research with open-source tools.</em><br>
  <a href="https://github.com/I-Sumit-kumar/Automated-Tooth-Instance-Analysis">🌐 Repository</a>
</p>
