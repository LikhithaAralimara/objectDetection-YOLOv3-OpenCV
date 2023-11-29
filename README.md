# ObjectDetection-YOLOv3-OpenCV
This Python script uses OpenCV to implement object detection with the YOLOv3 model, capable of accurately identifying multiple objects in images or video frames. It captures video from the default camera or loads an image, applies real-time detection with user-defined thresholds, and displays results in a window named 'win'.

# YOLOv3 Object Detection with OpenCV

This Python script demonstrates real-time object detection using the YOLOv3 model with the OpenCV library.

## Prerequisites

- Python 3.x
- OpenCV
- NumPy

## Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/yolov3-object-detection.git
cd yolov3-object-detection
```
## Usage

1. Make sure you have the required dependencies installed.
2. Download the YOLOv3 configuration file (`yolov3.cfg`) and weights file (`yolov3.weights`) from the official YOLO website: [YOLOv3](https://pjreddie.com/darknet/yolo/)
3. Save the downloaded files in the project directory.
4. Create a file named `coco.names` and add the class names from the COCO dataset (available [here](https://github.com/pjreddie/darknet/blob/master/data/coco.names)).
5. Run the script:

   ```bash
   python yolo_object_detection.py

## Customization and Configuration

By default, the script captures video from the default camera. To load an image instead, set `showCap=False` and specify the image file.

```python
showCap = False  # Set to True for webcam feed, False for loading an image
image_file_path = 'path/to/your/image.jpg'  # Specify the path to your image file
```
### Configuration Variables

Tailor the script's behavior by adjusting the following variables:

- **`showCap`**: Set to `True` to use the webcam feed for real-time detection. Set to `False` to load a sample image.

  ```python
  showCap = True  # or False

- **`confThr`**: Confidence threshold for object detection.

  ```python
  confThr = 0.5  # Set your desired confidence threshold

- **`nmsThr`**: Non-maximum suppression threshold.

  ```python
  nmsThr = 0.4  # Set your desired non-maximum suppression threshold

Feel free to explore various configurations and seamlessly integrate the script into your projects! Customize the parameters to achieve optimal results for your specific use case.

