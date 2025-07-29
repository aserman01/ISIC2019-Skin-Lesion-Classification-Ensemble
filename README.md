# Skin Lesion Classification with Ensemble Methods

This repository contains the implementation and results described in our paper:

**"Comparison of Different Deep Learning Architectures on Skin Lesion Classification with the ISIC 2019 Dataset"**

Authors: Anil Tan Aktan, Alaa Almouradi, Erchan Aptoula, Berrin Yanikoglu
Sabanci University, Istanbul, Türkiye


[![Download Models](https://img.shields.io/badge/Download-Trained%20Models-blue?style=for-the-badge&logo=github)](https://github.com/aserman01/ISIC2019-Skin-Lesion-Classification-Ensemble/releases/)

## Paper Overview

This paper addresses the challenge of accurately classifying dermoscopic skin lesion images into multiple diagnostic categories, including various cancer types. It evaluates state-of-the-art deep learning architectures, tackles class imbalance and robustness issues, and proposes a heterogeneous ensemble model achieving high performance.



## Contributions

* Evaluation of deep learning methods addressing class imbalance and robustness in skin lesion classification.
* Development of a heterogeneous ensemble model for enhanced multi-class classification.
* Implementation of effective test-time augmentation for clinical robustness.



## Dataset

The models are trained and evaluated on the publicly available [ISIC 2019 Dataset](https://challenge.isic-archive.com/data/).

* Training set: 25,331 images
* Test set: 8,238 images
* Classes: NV, MEL, BCC, BKL, AK, SCC, VASC, DF



## Methods and Technologies

* **Architectures:**

  * EfficientNet-B5
  * Vision Transformer (ViT)
  * MambaVision (Hybrid ViT-State Space Model)
* **Training Strategies:**

  * Data augmentation
  * Test-time augmentation (TTA)
  * Loss functions (Cross-Entropy, Weighted Cross-Entropy, Focal Loss)
  * Bayesian hyperparameter optimization (Optuna)



## Results

| Model                 | F1-score  | Accuracy  | Balanced Accuracy | Macro AUC |
| --------------------- | --------- | --------- | ----------------- | --------- |
| EfficientNet-B5       | 0.736     | 0.738     | 0.598             | 0.925     |
| ViT                   | 0.722     | 0.724     | 0.587             | 0.912     |
| MambaVision           | 0.723     | 0.735     | 0.591             | 0.918     |
| **Proposed Ensemble** | **0.743** | **0.748** | **0.607**         | **0.942** |


## Contact

For any inquiries, please contact:

* Anil Tan Aktan ([tan.aktan@sabanciuniv.edu](mailto:tan.aktan@sabanciuniv.edu))
* Alaa Almouradi ([alaaalmouradi@sabanciuniv.edu](mailto:alaaalmouradi@sabanciuniv.edu))
* Erchan Aptoula ([erchan.aptoula@sabanciuniv.edu](mailto:erchan.aptoula@sabanciuniv.edu))
* Berrin Yanikoglu ([berrin@sabanciuniv.edu](mailto:berrin@sabanciuniv.edu))
