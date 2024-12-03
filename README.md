# Face Mask Detection with Hand Tracking

A real-time face mask detection system that also tracks hand positions to improve detection accuracy by ignoring faces that are being covered by hands.

## Features

- Real-time face mask detection using webcam
- Hand tracking to prevent false detections when touching face
- Support for multiple face detection
- Visual indicators for mask/no mask status
- Confidence threshold filtering for reliable detection

## Requirements

- Python 3.x
- OpenCV (cv2)
- TensorFlow
- MediaPipe
- NumPy

## Installation

1. Clone this repository
2. Install required dependencies:
```sh
pip install opencv-python tensorflow mediapipe numpy
```

## Usage

1. Ensure you have the model file 

model_face_mask.keras

 in the root directory
2. Run the Jupyter notebook 

face_mask.ipynb


3. Press 'q' to exit the application

## Project Structure

- 

face_mask.ipynb

 - Main application code with face mask detection and hand tracking
- 

model_face_mask.keras

 - Trained Keras model for mask detection
- 

mask_detect.keras

 - Backup model file
- 

mask_violations

 - Directory for storing violation logs
- 

mask_detection.log

 - Application log file

## Model Information

The face mask detector uses a deep learning model trained to classify faces into two categories:
- with_mask
- without_mask

Confidence threshold is set to 0.9 for high reliability.

## Features Implementation

- Face Detection: Uses MediaPipe's Face Detection solution
- Hand Tracking: Uses MediaPipe's Hands solution
- Image Processing: Resizes faces to 224x224 pixels and normalizes pixel values
- Real-time Processing: Processes webcam feed in real-time with OpenCV

## Error Handling

The system includes robust error handling for:
- Missing model file
- Invalid face detection
- Webcam access issues
- Model loading errors

## License

[Add your license information here]
```

This documentation covers the main aspects of your face mask detection project, including setup, usage, and technical details. You should update the License section and add any additional specific instructions if needed.This documentation covers the main aspects of your face mask detection project, including setup, usage, and technical details. You should update the License section and add any additional specific instructions if needed.