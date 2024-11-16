
# Mask Detection Web App using Streamlit

This is a simple **real-time mask detection web application** built using **Streamlit**, **OpenCV**, and **TensorFlow**. The app detects whether a person in front of the webcam is wearing a mask or not. The application uses a pre-trained deep learning model (`mask_detector.h5`) to make predictions in real-time.

## Project Overview

- The app captures video from the webcam using OpenCV.
- Each frame is passed through a trained model for mask detection.
- The app displays the prediction (whether a mask is detected or not) on the live webcam feed.
- The model is a binary classification model that outputs either "Mask Detected" (1) or "No Mask Detected" (0).
  
## Features

- Real-time webcam mask detection.
- Shows a label on the webcam feed indicating whether a mask is detected or not.
- Built using Streamlit for a simple web-based interface.

## Prerequisites

Before running the app, you need to install the necessary dependencies and have the required model file.

### Requirements

- Python 3.x
- TensorFlow (for the pre-trained model)
- OpenCV (for webcam video capture and frame processing)
- Streamlit (for building the web app)

### Install Dependencies

You can install the required dependencies using `pip`. You can either install them manually or use the provided `requirements.txt` file (if you prefer).

To install the dependencies manually, run:

```bash
pip install streamlit opencv-python tensorflow
```

Alternatively, create a `requirements.txt` file with the following content:

```
streamlit
opencv-python
tensorflow
```

Then, install the dependencies using:

```bash
pip install -r requirements.txt
```

### Model File

- The app uses a pre-trained model `mask_detector.h5` to detect whether a person is wearing a mask.
- Ensure that you have the model file in the same directory as the app, or provide the correct path to the model in the code.

## Usage

1. **Clone this repository** (or download the `app.py` and `mask_detector.h5` files).

   ```bash
   git clone <repository-url>
   ```

2. **Navigate to the project directory**.

   ```bash
   cd path/to/project
   ```

3. **Run the Streamlit app**.

   Run the following command to start the app:

   ```bash
   streamlit run app.py
   ```

4. **Open the app in your browser**.

   The app will automatically open in your default web browser, and you should see the webcam feed along with the mask detection results in real-time.

### Example Output

- **Mask Detected**: The app will display a green label "Mask Detected" when the person in front of the webcam is wearing a mask.
- **No Mask Detected**: The app will display a red label "No Mask Detected" when the person is not wearing a mask.

## Code Structure

- **`app.py`**: Main Streamlit app file. It handles the webcam feed, mask detection, and the display of results.
- **`mask_detector.h5`**: Pre-trained model file for mask detection (make sure to have this in your project directory).

## Model Details

The app uses a pre-trained mask detection model. If you don't have a pre-trained model yet, you can use models such as MobileNetV2 trained on a mask detection dataset or create your own mask detection model.

- You can train a model on a mask detection dataset, which consists of images of people with and without masks.
- For more information on creating or training a mask detection model, check out [this tutorial](https://realpython.com/keras-deep-learning/).

## Troubleshooting

- **Camera Access**: If the app is not showing the webcam feed, ensure that your camera is accessible and not being used by other applications.
- **Model Not Found**: Ensure that the `mask_detector.h5` model is in the correct path relative to the `app.py` script.
- **Slow Performance**: If you experience slow performance, consider reducing the video frame size or using a smaller, more optimized model like MobileNetV2.


## Project by 

Name: Rohan chatse (Data scientist)
Email: rohancrchatse@gmail.com 





