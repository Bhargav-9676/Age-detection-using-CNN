# Age Prediction Model

## Description

This project is designed to predict the age of individuals from images using a **Convolutional Neural Network (CNN)**. The model uses a deep learning approach to analyze facial features and estimate the age of a person based on their image.

### Features:

* **Image Preprocessing**: Resizes and normalizes input images for model compatibility.
* **CNN Architecture**: Trains and predicts the age of individuals from facial images.
* **Real-time Prediction**: Allows real-time age prediction from a provided image.
* **Custom Dataset**: Supports testing with custom images and labels.

---

## Requirements

To run the project, make sure you have the following Python libraries installed. You can install them using the command:

```bash
pip install -r requirements.txt
```

### Libraries:

* `requests` – For downloading images from the web.
* `Pillow` – For image manipulation and processing.
* `matplotlib` – For visualizing images and results.
* `torch` and `torchvision` – For building and using deep learning models.

---

## Installation

1. Clone this repository to your local machine:

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install the dependencies from the `requirements.txt` file:

   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. **Download Test Images**: The project includes a set of test images that are downloaded automatically when the script runs. These images are saved in the `test_images/` directory.

2. **Run the Script**:
   To test the model, simply run the Python script which will:

   * Download a test image.
   * Display the image along with the true age.
   * If a trained model is available, it will predict the age and show the predicted age alongside the actual age.

   Example:

   ```bash
   python predict_age.py
   ```

3. **Prediction Output**:
   The script will display the test image with the predicted and true ages. You can modify the script to add additional images and test the model's performance on them.

---

## Model Training

The model is built using **PyTorch** and trained on a custom dataset of images with corresponding age labels. The model utilizes a **CNN architecture** to extract features from facial images and predict the corresponding age.

---

## File Structure

```
Age-Prediction-Model/
│
├── test_images/             # Folder containing test images
├── model/                   # Folder for saving trained model weights
├── requirements.txt         # List of Python dependencies
├── predict_age.py           # Main script for prediction
└── README.md                # Project documentation
```

---


### Customization:

* **Add More Test Images**: You can modify the `test_images` section to add more URLs or paths to your images.
* **Model Performance**: Implement evaluation metrics like **Mean Absolute Error (MAE)** or **Root Mean Squared Error (RMSE)** for assessing the model's prediction performance.

