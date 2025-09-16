# Skin Lesion Classification System

This project presents a deep learning solution for classifying 7 types of skin lesions from the HAM10000 dermatoscopic image dataset. The primary challenge was the dataset's severe class imbalance. The final model utilizes a pre-trained **ResNet50** architecture in **PyTorch**, combined with a **class weighting** strategy, to achieve high accuracy and robust performance.



---
## Key Features
* **Model:** Transfer learning with a state-of-the-art **ResNet50** model, pre-trained on ImageNet.
* **Performance:** Achieved **85% accuracy** on the unseen test set.
* **Imbalance Handling:** Implemented **class weights** in PyTorch to effectively train on the imbalanced data, forcing the model to pay attention to rare classes.
* **Explainability:** Includes **Grad-CAM** visualizations to interpret model predictions and understand which parts of an image influenced the diagnosis.

---
## Model Performance
The final model achieved a test accuracy of **84.76%**. The classification report shows strong performance, particularly a "safety-first" bias with high recall rates for critical cancerous classes like Melanoma (**71%**) and Basal Cell Carcinoma (**84%**).

---
## Tech Stack
* **Frameworks:** Python, PyTorch, Scikit-learn
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Pillow, TQDM

---
## Usage
The entire workflow, from data loading and preprocessing to model training and evaluation, is contained within the main Jupyter Notebook file. To run this project, open the notebook in an environment like Google Colab, ensure a GPU is enabled, and execute the cells in order.

---
## Dataset
This project uses the publicly available [HAM10000 "Skin Cancer MNIST" dataset on Kaggle](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000).
