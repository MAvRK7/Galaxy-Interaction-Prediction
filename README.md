# Explainable Galaxy Interaction Prediction with Novel Hybrid Attention Mechanisms

This repository implements a novel attentive neural ensemble model for predicting galaxy interactions using the Galaxy Zoo DESI dataset from the DESI Legacy Imaging Surveys. The model integrates three advanced architectures—Attention-Guided Explainable Capsules (AG-XCaps), Hybrid Self-Attention Neural Network (H-SNN), and ResNet with GRU layers—to provide highly accurate and interpretable predictions.

Key Features:

Attention Mechanisms: Used to capture complex morphological features of galaxies.

Explainability: Utilizes Local Interpretable Model-agnostic Explanations (LIME) to ensure transparency in predictions.

High Accuracy: Achieved 96% accuracy, 0.95 precision, 1.00 recall, and 0.97 F1-score in binary classification of galaxy interactions.

Performance: Outperforms a Random Forest baseline, significantly reducing false positives while maintaining robust detection of interacting galaxies.

Lightweight: Model size of only 0.45 MB, making it efficient for large-scale surveys.

Scalable Inference: Suitable for future large-scale surveys like Euclid and LSST.

Installation:

Prerequisites are
Python 3.x,
PyTorch,
TensorFlow 

Required libraries:

numpy,
pandas,
scikit-learn,
LIME,
matplotlib (for visualization)

Dataset:

The model is trained on the Galaxy Zoo DESI dataset, which is publicly available through the DESI Legacy Imaging Surveys. You can download the dataset from the official Galaxy Zoo website. (https://www.zooniverse.org/projects/zookeeper/galaxy-zoo/)

Code is available in Galaxy_Morphology_main.ipynb.zip

Results:

Precision: 0.95

Recall: 1.00

F1-Score: 0.97

Accuracy: 96%

False Positives: Reduced from 70 (Random Forest) to 23.


Model Architecture

The ensemble model combines the following architectures:

Attention-Guided Explainable Capsules (AG-XCaps),
Hybrid Self-Attention Neural Network (H-SNN),
ResNet with GRU layers.

These architectures work together to capture complex galaxy morphology and enhance prediction accuracy.

Contributing

Feel free to open issues or submit pull requests to contribute to the project.

Acknowledgments

Galaxy Zoo
DESI Legacy Imaging Surveys
LIME for explainable AI
