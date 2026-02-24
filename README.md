# Multi-label Emotion Classification for the DLGenAI Project competition

This repository contains the implementation of a Deep Learning and Generative AI project, covering the full pipeline from data preprocessing and model training to inference. This project is documented in the associated report `23F3001910_DG_T32025.pdf`.

## Project Overview
This project focuses on predicting five emotions, **anger, fear, joy, sadness, and surprise**, from short English text snippets. Since texts can express multiple emotions simultaneously, the task is treated as a multi-label classification problem. The dataset was found to be highly imbalanced. The final solution employs an ensemble of transformer models to maximize predictive performance.

## Repository Structure

The project is organized into modular directories to separate the different stages of the machine learning lifecycle:

*   **`Preprocessing/`**: Contains notebooks and scripts for data cleaning, augmentation, and preparation.
*   **`Training/`**: Includes the core model architecture and training loops.
*   **`Data/`**: Directory for storing datasets used during the project.
*   **`Milestones/`**: Documentation and code related to specific project progress milestones given by instructors.
*   **`inference.ipynb`**: A standalone Jupyter Notebook to run the trained model on test data.
*   **`23F3001910_DG_T32025.pdf`**: The final project report containing methodology, architecture details, and results.


## Results
Performance is measured by the **Macro F1-score**.

| Model | Leaderboard Score |
| :--- | :--- |
| DeBERTa Baseline | 0.87 |
| RoBERTa Baseline | 0.865 |
| DeBERTa Advanced (Ensemble+Focal) | 0.877 |
| RoBERTa Advanced (Ensemble+Focal) |0.87  |
| **Ensemble (DeBERTa + RoBERTa)** | **0.883** |

## Tech Stack
* **Frameworks:** PyTorch, Hugging Face Transformers
* **Tracking:** Weights & Biases (wandb)
* **Environment:** Python 3.10, Google Colab / GPU

---
**Author:** [Shi-pra-19](https://github.com/Shi-pra-19)
**Roll Number:** 23F3001910





