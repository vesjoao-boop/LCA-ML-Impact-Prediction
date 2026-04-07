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
2. **`data`**: Anonymized dataset provided for training and testing the models, ensuring reproducibility without compromising sensitive or proprietary industrial information.

## 📊 Dataset Overview

The provided anonymized dataset is structured to train supervised learning algorithms. It consists of:

* **20 Input Features ($X$):** Representing the process parameters, material inputs, or aggregated LCI flows.
* **3 Target Features ($y$):** Representing the specific environmental impact categories (LCIA results) to be predicted by the model.

## 🚀 Getting Started

### Prerequisites
Make sure you have Python installed. It is highly recommended to use a virtual environment to manage dependencies.

### 1. Clone the repository
```bash
git clone [https://github.com/vesjoao-boop/LCA-ML-Impact-Prediction.git](https://github.com/vesjoao-boop/LCA-ML-Impact-Prediction.git)
cd LCA-ML-Impact-Prediction
