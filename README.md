# Leaf Disease Detection

Leaf Disease Detection is a machine learning project aimed at detecting plant diseases from images of leaves. By using deep learning techniques, this project helps identify diseases based on leaf patterns, color, and texture. This project can assist in early identification and prevention of plant diseases, potentially improving agricultural productivity.


## Overview

This project uses image classification techniques to detect and classify plant leaf diseases. It leverages convolutional neural networks (CNNs) to extract features from images of leaves and then classify them into healthy or diseased categories.

The primary diseases targeted in this project include:

- Bacterial Spot
- Late Blight
- Early Blight
- Powdery Mildew
- Healthy (no disease)
- And many more diseases...

The project pipeline includes data preprocessing, model training, evaluation, and prediction.

## Dataset

The dataset used for this project contains labeled images of plant leaves, including both healthy and diseased samples. It is publicly available from the following sources:

- [PlantVillage Dataset](https://www.kaggle.com/emmarex/plantdisease)
  
Each image is labeled with a specific disease type or marked as healthy.

## Prerequisites

To run this project, you'll need the following software and libraries installed:

- Python 3.x
- TensorFlow / Keras
- NumPy
- OpenCV
- Scikit-learn
- Matplotlib

You can install the required libraries using:

```bash
pip install -r requirements.txt
```

## Installation

1. Clone the repository:

```bash
git clone https://github.com/username/leaf-disease-detection.git
cd leaf-disease-detection
```

2. Install the dependencies:

```bash
pip install -r requirements.txt
```

3. Download the dataset and place it in the `data/` directory:

```bash
mkdir data
# Place dataset in the data folder
```

## Model Training

To train the model on the dataset, run the following command:

```bash
python train.py
```

This will start the training process and save the trained model to the `models/` directory.

## Prediction

To predict disease from an image of a leaf, run the following command:

```bash
python predict.py --image /path/to/leaf/image.jpg
```

This will output the predicted disease class for the given image.

## Evaluation

To evaluate the model's performance on a test dataset, run:

```bash
python evaluate.py
```

This will provide metrics such as accuracy, precision, recall, and F1-score.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
