# An Explainable Graph-Based Approach to Agriculture Crop Disease Identification

## Overview
This project presents **G-AgriNet**, an advanced automated system for classifying crop diseases using **Graph Neural Networks (GNNs)**. Our approach integrates **Active Learning (AL), Feature Extraction, and Graph Classification** to enhance classification accuracy and interpretability. By leveraging GraphXAI visualization tools, this system provides transparency and insights into disease classification in agriculture.

## Features
- **Active Learning (AL):** Selects informative nodes to label, improving classification performance.
- **Feature Extraction:** Utilizes **GLCM, LBP**, and other handcrafted features from crop images.
- **Graph Construction:** Constructs a graph based on extracted features for better representation.
- **Graph Classification:** Uses **Graph Neural Networks (GNNs), Graph Attention Networks (GATs)** for node classification.
- **Explainability & Interpretability:** Employs **Grad-CAM, GNNExplainer, GraphLIME, SHAP**, and **SubgraphX** for decision analysis.
- **High Accuracy:** Achieved **99.25% accuracy** using the **CCMT Crop Pest and Disease Detection dataset** with **102,976 images** across **22 classes**.
- **Sustainable Agriculture Impact:** Supports **Integrated Pest Management (IPM)** by reducing excessive pesticide use.

## System Architecture
1. **Active Learning (AL):** Selects informative data samples for annotation (Section III-A).
2. **Feature Extraction:** Extracts handcrafted features from images (Section III-B).
3. **Graph Construction & Classification:** Constructs a feature-based graph and classifies nodes (Section III-C).
4. **Interpretability & Visualization:** Uses **GraphXAI** tools for explainability.

## Dataset
- **Dataset Name:** CCMT Crop Pest and Disease Detection Dataset
- **Total Images:** 102,976
- **Classes:** 22 (Cashew, Cassava, Maize, Tomato, etc.)
- **Graph Data Structure:**
  - **Train Node Features:** (77,092, 15)
  - **Test Node Features:** (19,274, 15)
  - **Edges:** (210, 2)

## Technologies Used
- **Deep Learning:** TensorFlow, PyTorch Geometric
- **Graph Analysis:** NetworkX, PyG
- **Image Processing:** OpenCV, NumPy, Pandas
- **XAI (Explainable AI):** GraphXAI, SHAP, Grad-CAM
- **Visualization:** Matplotlib, Seaborn

## Installation
```bash
# Clone the repository
git clone https://github.com/your-username/G-AgriNet.git
cd G-AgriNet

# Install dependencies
pip install -r requirements.txt
```

## Usage
```python
from model import GAgriNet
model = GAgriNet()
model.train()
model.evaluate()
```

## Results
- **Accuracy:** 99.25%
- **Precision, Recall, F1-score:** Available in `results/metrics.json`
- **ROC Curve & AUC Values:** Plots available in `results/` folder

## Contributors
- **Injamul** - [GitHub Profile](https://github.com/your-username)

## License
MIT License - See [LICENSE](LICENSE) for details.

## Acknowledgments
- **Daffodil International University - Department of Computer Science and Engineering**
- **Google Colab Pro** for model training
- **GraphXAI Toolkit** for interpretability
