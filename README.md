# SAM
Segment Anything Model (SAM)
# Deep Neural Network Project README

## Semantic Segmentation using Meta's Model Fine-Tuning

This project focuses on fine-tuning Meta's newly released model for the semantic segmentation problem. The goal is to accurately label each pixel in satellite images depicting water bodies.

### Data Set Preparation

We selected the dataset for this project from [Kaggle](https://www.kaggle.com/datasets/franciscoescobar/satellite-images-of-water-bodies), specifically the *Satellite Images of Water Bodies* dataset, which includes both images and masks for image segmentation. We divided the data into two parts: training and evaluation, in a 1:9 ratio.

### Model Selection

To load the model, we utilized the Model Card for Segment Anything Model (SAM) - ViT Base (ViT-B) version, as described in the article *Segment Anything* by Alexander Kirillov, Eric Mintun, and Nikhila Ravi.

### Data Augmentation

Given the nature of satellite data, we employed data augmentation techniques to enhance the model's ability to generalize and accurately segment images under various conditions. We utilized the Albumentations library, a powerful tool for data augmentation in machine vision and image processing problems.

### Metric and Cost Function Evaluation

For evaluating the performance of our model during training, we implemented two metrics: the Dice coefficient and the Intersection over Union (IoU) score. These metrics provide insights into the accuracy and consistency of the model's segmentation outputs.

---

This README provides an overview of our deep neural network project for semantic segmentation. For more detailed instructions on running the code and reproducing the results, please refer to the documentation provided in the repository. Contributions and feedback are welcome!
