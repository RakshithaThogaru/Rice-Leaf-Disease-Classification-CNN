# Rice Leaf Disease Classification Using CNN

## Project Overview

This project focuses on classifying rice leaf diseases using image processing and Convolutional Neural Networks (CNNs). The objective is to analyze leaf images and classify them into three disease categories: **Bacterial Leaf Blight, Brown Spot, and Leaf Smut**.

The project includes Exploratory Data Analysis (EDA), image preprocessing, CNN model development, data augmentation, model evaluation, and performance comparison.

## Objectives

- Analyze rice leaf image data using Exploratory Data Analysis.
- Preprocess images for deep learning model training.
- Develop a CNN model for rice leaf disease classification.
- Apply data augmentation to improve model generalization.
- Evaluate and compare baseline and augmented CNN models.
- Identify model limitations and potential improvements.

## Dataset

The dataset consists of 119 images belonging to three classes.

| Disease Class | Number of Images |
|---|---:|
| Bacterial Leaf Blight | 40 |
| Brown Spot | 40 |
| Leaf Smut | 39 |
| **Total** | **119** |

The dataset was explored to understand image dimensions, class distribution, RGB characteristics, and image variations.

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Google Colab

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

- Analyzed class-wise image distribution.
- Examined image dimensions and aspect ratios.
- Visualized sample images from each disease category.
- Explored RGB color distributions and image characteristics.

### 2. Image Preprocessing

- Resized images to 224 × 224 pixels.
- Normalized pixel values.
- Prepared training, validation, and testing datasets.
- Applied appropriate preprocessing for CNN training.

### 3. Baseline CNN Model

Developed a baseline Convolutional Neural Network to classify rice leaf diseases.

The model was trained and evaluated using training, validation, and test datasets.

### 4. Data Augmentation

Applied augmentation techniques to training images to introduce additional variations:

- Horizontal flipping
- Random rotation
- Random zoom
- Random translation
- Random contrast adjustment

### 5. Augmented CNN Model

Developed and trained an augmented CNN model to investigate whether data augmentation could improve classification performance and generalization.

### 6. Model Evaluation

Both models were evaluated using:

- Training Accuracy
- Validation Accuracy
- Test Accuracy
- Test Loss
- Precision
- Recall
- F1-Score
- Confusion Matrix

## Model Performance Comparison

| Metric | Baseline CNN | Augmented CNN |
|---|---:|---:|
| Training Accuracy | 59.04% | 42.17% |
| Validation Accuracy | 77.78% | 55.56% |
| Test Accuracy | 50.00% | 50.00% |
| Test Loss | 0.9437 | 1.0115 |
| Macro F1-Score | 0.4776 | 0.4434 |

## Results and Conclusion

Both models achieved a test accuracy of 50.00%.

The Baseline CNN achieved a higher validation accuracy and Macro F1-Score than the Augmented CNN. Data augmentation did not improve overall test performance in this experiment.

Based on the evaluation results, the Baseline CNN was selected as the better-performing model among the two configurations.

The experiment highlighted the challenges of training deep learning models with limited image data and the importance of evaluating class-wise performance rather than relying only on accuracy.

## Challenges

- Limited dataset size.
- Variations in image dimensions, lighting, and background.
- Difficulty generalizing to unseen images.
- Inconsistent class-wise classification performance.
- Data augmentation did not improve overall test performance.
- Limited computational resources during model training.

## Future Improvements

- Collect a larger and more diverse dataset.
- Experiment with transfer learning architectures such as MobileNetV2, ResNet, or EfficientNet.
- Perform hyperparameter tuning.
- Explore additional augmentation strategies.
- Evaluate the model on a larger independent test dataset.
- Improve classification performance across all disease categories.

## Project Structure

```text
Rice-Leaf-Disease-Classification-CNN/
│
├── Rice_Leaf_Disease_Classification.ipynb
├── README.md
├── requirements.txt
│
└── results/
    ├── dataset_distribution.png
    ├── model_accuracy.png
    ├── model_loss.png
    ├── confusion_matrix.png
    └── model_comparison.png
```

*Note: The results directory will contain selected project visualizations. The original dataset is not included in this repository.*

## Project Notebook

The Jupyter Notebook contains the complete workflow, including:

- Data analysis and visualizations
- Image preprocessing
- Baseline CNN training
- Data augmentation
- Augmented CNN training
- Model evaluation
- Confusion matrices
- Classification reports
- Performance comparison
- Final conclusions

## Author

**Rakshitha Thogaru**

B.Tech Graduate | Computer Science

Interested in Data Science, Machine Learning, Artificial Intelligence, and Data Analytics.

GitHub: [RakshithaThogaru](https://github.com/RakshithaThogaru)
