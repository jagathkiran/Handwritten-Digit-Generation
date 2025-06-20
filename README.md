# Handwritten Digit Generation with Naive Bayes

This repository contains a Jupyter notebook demonstrating the generation of handwritten digits using the Naive Bayes algorithm, specifically leveraging the MNIST dataset and the Bernoulli Naive Bayes model. The notebook includes code for loading the dataset, preprocessing, model training, and generating new digit samples using different methods.

## Project Overview

The project showcases how a Naive Bayes algorithm can be used as a generative model to create new samples resembling handwritten digits from the MNIST dataset. It includes:
- Loading and preprocessing the MNIST dataset.
- Training a Bernoulli Naive Bayes model.
- Generating new digit images using template, threshold, and probabilistic methods.
- Visualizing generated digits interactively.

## Prerequisites

To run this project, ensure you have the following installed:
- Python 3.8 or later
- pip (Python package manager)
- Virtualenv (optional, for creating a virtual environment)

## Installation

Follow these steps to set up and run the project:

### 1. Clone the Repository
```bash
git clone https://github.com/jagathkiran/Handwritten-Digit-Generation.git
cd Handwritten-Digit-Generation
```

### 2. Create a Virtual Environment
To isolate dependencies, create a virtual environment:
```bash
python -m venv venv
```

Activate the virtual environment:
- On Windows:
  ```bash
  venv\Scripts\activate
  ```
- On macOS/Linux:
  ```bash
  source venv/bin/activate
  ```

### 3. Install Dependencies
The required Python packages are listed in `requirements.txt`. Install them using:
```bash
pip install -r requirements.txt
```

### 4. Run the Jupyter Notebook
Start Jupyter Notebook:
```bash
jupyter notebook
```

Open the `Handwritten digit generation using Naive Bayes algorithm.ipynb` file in the Jupyter interface and run the cells to execute the code.

## Dependencies
The project uses the following key Python packages (see `requirements.txt` for the full list):
- `numpy`: For numerical computations.
- `matplotlib`: For visualizing generated digits.
- `scikit-learn`: For the Bernoulli Naive Bayes model.
- `tensorflow`: For loading the MNIST dataset.
- `scipy`: For image processing utilities.

## Usage
1. Open the Jupyter notebook in your browser.
2. Run the cells sequentially to:
   - Load and preprocess the MNIST dataset.
   - Train the Naive Bayes model.
   - Generate and visualize handwritten digits using different methods.
3. The `interactive_generation` function will display generated digits for each class (0–9) using template, threshold, and probabilistic methods.

## Notes
- The notebook assumes the MNIST dataset is accessible via `tensorflow.keras.datasets.mnist`.
- The generated digits are binary (black and white) due to the use of Bernoulli Naive Bayes.
- Adjust the `temperature` parameter in the probabilistic method to control the randomness of generated samples.
