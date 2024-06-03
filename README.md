# Machine Learning Project: ECG Health Classification

## Overview

This project focuses on using Machine Learning techniques to classify Electrocardiogram (ECG) data as either healthy or unhealthy. We employed a Transformer model to analyze the ECG signals and make predictions regarding their health status. The model was trained using Python and TensorFlow, with variations including Transformer architectures with both 32 and 16 attention heads.

## Dataset

The dataset used in this project consists of a collection of ECG signals in the ecg5000 folder. Here we inverted the test and train set due to huge data in the test set compared to the train set.

## Model Architecture

We experimented with different variations of the Transformer model architecture to find the most effective approach for ECG signal classification. Two main configurations were explored:

1. Transformer Model with 32 Attention Heads
2. Transformer Model with 16 Attention Heads
We used both a single and a double-layer encoder.

The models are trained using the labeled ECG data to learn patterns indicative of healthy and unhealthy signals.

## Implementation

The project is implemented in Python using Pytorch, a popular machine learning framework. The codebase consists of a single ipynb file with following sections:

- **data_processing**: Here we used a wavelet filter to filter out the noise and separate the healthy from unhealthy samples.
- **transformer model**: Defines the Transformer model architectures with different attention head configurations.
- **train**: Handles the training procedure, including model training, validation, and evaluation.
- **Threshold calculation**: Calculation of threshold based on which we can say whether a sample is healthy or not.
- **test**: Contains utility functions used across different modules.

## Usage

To run the project, follow these steps:

1. Install the required dependencies.
2. Prepare your ECG dataset or use a provided dataset.
3. Preprocess the data using `data_processing`.
4. Train the model using `train`, specifying the desired model architecture and hyperparameters.
5. Evaluate the trained model using `test` on test data.

## Results

The performance of the trained models is evaluated using standard metrics such as accuracy, precision, recall, and F1-score. Results are presented in tabular format and can be found in the [results directory](https://github.com/Asif-droid/CSE-472-project-anomally-detection-in-ecg-/blob/main/Project/result.md).


## Conclusion

In conclusion, this project demonstrates the feasibility of using Transformer models for ECG signal classification. By experimenting with different attention head configurations, we explored the impact of model architecture on classification performance. Further optimizations and fine-tuning may improve the model's accuracy and robustness.

## Contributors

- [K M Asifur Rahman](https://github.com/Asif-droid)
