# LCA-ML Impact Prediction 🍃🤖

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![License](https://img.shields.io/badge/license-MIT-green)

> **Integration of Life Cycle Assessment (LCA) and Machine Learning for environmental impact prediction.**

## 📖 About the Project

This repository contains the methodology and source code to predict environmental impact categories by combining Life Cycle Inventory (LCI) data with Machine Learning algorithms. The primary goal is to overcome computational bottlenecks and the scarcity of primary data in LCA studies by leveraging data-driven predictions based on historical datasets.

## 📂 Repository Contents

Currently, the repository is streamlined into two main components:

1. **`github_pipeline_lca+ml_integration`**: The core script/notebook that contains the end-to-end Machine Learning pipeline. It handles everything from data loading and preprocessing to model training, evaluation, and prediction.
2. **`data`**: generic dataset provided for training and testing the models, ensuring reproducibility without compromising sensitive or proprietary industrial information.

## 🚀 Getting Started

### Prerequisites
Make sure you have Python installed. It is highly recommended to use a virtual environment to manage dependencies.

### 1. Clone the repository
```bash
git clone https://github.com/vesjoao-boop/LCA-ML-Impact-Prediction.git
cd LCA-ML-Impact-Prediction
```

### 2. Install required packages
To ensure the code runs correctly, you need to install the same libraries used during development. We highly recommend creating a virtual environment first.

```bash
# Create a virtual environment (optional but recommended)
python -m venv venv

# Activate the environment (Windows)
venv\Scripts\activate

# Activate the environment (Linux/Mac)
source venv/bin/activate

# Install the dependencies
pip install -r requirements.txt
```

### 3. Run the Prediction Pipeline
Due to confidentiality reasons, the real industrial LCA dataset is not publicly available. However, to ensure full reproducibility, we provide a script that generates a synthetic dataset containing 200 samples, 20 LCA-related input features (materials, energy, transport), and 3 target impact categories.

#### 📊 Dataset Overview

The provided generic dataset is structured to train supervised learning algorithms. It consists of:

* **20 Input Features (X):** Representing the process parameters, material inputs, or aggregated LCI flows.
* **3 Target Features (y):** Representing the specific environmental impact categories (LCIA results) to be predicted by the model.
  
```bash
# If using a standard Python script:
python github_pipeline_lca+ml_integration.py

# If using a Jupyter Notebook:
jupyter notebook github_pipeline_lca+ml_integration.ipynb
```

## 📈 Results and Visualizations

*(Drag and drop an image of your graphs here. For example, a Feature Importance chart or a parity plot showing Actual Impacts vs. Predicted Impacts).*

## 🎓 4. Citation

If this code or dataset is useful for your research, please cite our paper:

```bibtex
@article{Salla2026lca,
  title={Accelerating Life Cycle Assessment: A Machine Learning-Based Decision-Support Pipeline for Environmental Impact Prediction},
  author={João Victor Encide Salla, Tiago Agostinho de Almeida and Diogo Aparecido Lopes Silva},
  journal={Journal of Cleaner Prodyction (target)},
  research group= {EngS and LaSID, UFSCar - Brazil}
  year={2026}
}
```

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.
