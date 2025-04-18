# PseudoLabeling-CNN-DominAdaptation
This tutorial on pseudo-labeling for domain adaptation using the DomainNet dataset!


This tutorial on pseudo-labeling for domain adaptation using the DomainNet dataset! You'll learn how to leverage pseudo-labeling techniques to improve model performance across different domains within the diverse DomainNet dataset, enhancing your model's ability to generalize and adapt.

Domain Adapation: Domain adaptation refers to the process of transferring knowledge from one domain (source) to another (target) where the data distributions are different. It's often used in machine learning and AI to improve the performance of models when applied to new, unseen environments.

CCN: Convolutional Neural Networks (CNNs), a type of deep learning model especially effective for tasks involving spatial data, like images.

Pseduo-labeling: Pseudo-labeling is a powerful semi-supervised learning technique where a model trained on labeled data generates labels for unlabeled data. This approach can iteratively improve the model's performance by incorporating the newly labeled data. Here’s a high-level overview of a pseudo-labeling cycle

DomainNet Dataset is a collection of common objects across six different domains: Clipart, Infograph, Real, Painting, Quickdraw, and Sketch. Each domain includes 345 categories (classes) of objects such as bracelets, planes, birds, and cellos. This dataset is often used for tasks like domain adaptation and domain generalization

Prerequisites

Basic understanding of Pytorch, Machine learning and neural networks
Python, CNN, Pytorch libraries


## Training Metrics

Below are the training metrics for 10 epochs:

| Epoch | Loss                  | Notes            |
|-------|-----------------------|------------------|
| 1     | 4.8640               | Epoch 1 completed |
| 2     | 3.1892               | Epoch 2 completed |
| 3     | 2.1195               | Epoch 3 completed |
| 4     | 1.3928               | Epoch 4 completed |
| 5     | 0.8942               | Epoch 5 completed |
| 6     | 0.5775               | Epoch 6 completed |
| 7     | 0.3912               | Epoch 7 completed |
| 8     | 0.3272               | Epoch 8 completed |
| 9     | 0.2285               | Epoch 9 completed |
| 10    | 0.1873               | Epoch 10 completed |


Conclusion

The initial loss when using source domain only is significantly higher.
Adding pseudo labels starts with a much lower initial loss, indicating the additional data helps the model start off in a better position.
This lower initial loss would reflect the fact that the model has already
learned from the source data before incorporating pseudo-labeled data.
Pseudo-labeled data introduces some uncertainty, as the pseudo-labels might not be as accurate as true labels. This can introduce noise, leading to a slightly higher loss during training. Possibly explaing why the 10th epoch for the inital source domain training was lower
