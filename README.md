# Dog vs Cat Image Classifier

This project implements an SVM (Support Vector Machine) classifier to distinguish between images of dogs and cats using Histogram of Oriented Gradients (HOG) features.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project uses machine learning techniques to classify images of dogs and cats. We use HOG (Histogram of Oriented Gradients) features to extract information from images and an SVM (Support Vector Machine) classifier to perform the classification. The goal is to achieve a high accuracy in distinguishing between the two classes.

## Dataset

The dataset used for this project is the [Dogs vs. Cats dataset](https://www.microsoft.com/en-us/download/details.aspx?id=54765) provided by Microsoft. Ensure you download and extract the dataset into a directory with the following structure:

```
extracted_images/
    └── PetImages/
        ├── Dog/
        └── Cat/
```

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/yourusername/dog-cat-classifier.git
    cd dog-cat-classifier
    ```

2. Create a virtual environment and activate it:

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install the required packages:

    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Extract the dataset as per the structure mentioned above.

2. Run the Jupyter notebook `svm_classifier.ipynb` to train and evaluate the SVM classifier.

3. The notebook includes steps for loading the dataset, extracting HOG features, training the SVM model, and evaluating its performance.

## Project Structure

```
dog-cat-classifier/
├── extracted_images/
│   └── PetImages/
│       ├── Dog/
│       └── Cat/
├── requirements.txt
├── README.md
└── svm_classifier.ipynb
```

## Results

The classifier should achieve a reasonable accuracy on the test set. Example output:

```
Accuracy: 90.00%
              precision    recall  f1-score   support

         Dog       0.91      0.89      0.90       100
         Cat       0.89      0.91      0.90       100

    accuracy                           0.90       200
   macro avg       0.90      0.90      0.90       200
weighted avg       0.90      0.90      0.90       200
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
