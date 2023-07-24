# Image Classification with TensorFlow.js

This project is a simple web-based image classification application that uses the [TensorFlow.js](https://www.tensorflow.org/js) library. It uses a pre-trained [MobileNet](https://arxiv.org/abs/1704.04861) model to classify images.

## Features

- **Image Upload:** Users can upload an image file for classification. The image file should be in a format that can be displayed in a web browser (e.g., JPG, PNG, GIF).

- **Image Classification:** Once an image is uploaded, it is passed to the MobileNet model for classification. The model outputs a list of probabilities, one for each class that the model can recognize.

- **Display of Results:** The application displays the class with the highest probability as the predicted class for the image. The name of this class and the associated probability are displayed on the web page.

## Usage

To use the application, simply open the HTML file in a web browser. Click the file input field to select an image file from your device. Once an image is selected, it will be displayed on the page and the model will automatically classify the image. The prediction result will be displayed below the image.

## Implementation Details

The application is implemented in HTML, CSS, and JavaScript. It uses the TensorFlow.js library to load the MobileNet model and perform the classification. The model is loaded from a JSON file hosted on the TensorFlow.js model repository.

The JavaScript code handles file uploads, image display, and prediction display. It also manages the lifecycle of the image URL to ensure that the URL of the previously uploaded image is released when a new image is uploaded.

The CSS code sets the font of the page to Roboto and hides the image element until an image is uploaded.

## Note

The code includes a list of class names (IMAGENET_CLASSES) that correspond to the classes that the MobileNet model can recognize. This list is incomplete and should be filled with the actual class names if the application is to be used for real image classification tasks.
