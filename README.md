# Thesis

### Exploring Novel Targets for Mycobacterium tuberculosis through Machine Learning Methods

This project accompanies the Master’s dissertation “Exploring Novel Targets for Mycobacterium tuberculosis through Machine Learning Methods” (University of Minho, 2025).
It presents a computational framework for drug–target interaction (DTI) prediction in Mycobacterium tuberculosis, combining both self-supervised and supervised learning models, namely the Barlow Twins architecture and the BCM-DTI model, to explore the potential of artificial intelligence in accelerating tuberculosis drug discovery.

The overall objective of this work is to integrate chemical and biological data to identify promising compound–protein interactions that may serve as candidates for new anti-tuberculosis therapies. To this end, the project constructs a unified pipeline that connects data preprocessing, model training, evaluation, and interpretation within a reproducible structure.

The data preprocessing stage merges and standardizes molecular and protein data from multiple bioactivity sources, including Papyrus and TBb specific datasets. Molecules are represented by SMILES strings and proteins by UniProt sequences. Continuous activity values such as pChEMBL are transformed into binary labels according to a threshold of 6.5, distinguishing active from inactive compounds.
This unified dataset is then used to train and test both deep learning models.

The Barlow Twins model is implemented as a self-supervised contrastive learning approach, capable of learning latent molecular representations without explicit labels. This representation learning step improves the model’s ability to generalize across unseen targets and molecular scaffolds.
In parallel, the BCM-DTI (Bilinear Convolutional Model for Drug–Target Interaction) is trained in a supervised setting, leveraging labeled data to perform direct DTI prediction. The two architectures are compared in terms of performance, interpretability, and suitability for small or imbalanced datasets.


