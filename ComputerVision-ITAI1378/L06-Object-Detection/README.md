# L06 - Object Detection and Image Segmentation

## Course Information

- Student: Ali Abed
- Course: ITAI 1378 - Computer Vision
- Institution: Houston Community College

## Problem Statement

This project explores modern computer vision techniques
for detecting objects and identifying their precise
outlines within digital images.

## Approach

The project uses pretrained YOLO11 and SAM 2 models
to perform object detection and instance segmentation.

The main steps include:

- Loading pretrained YOLO11 models
- Detecting objects in sample images
- Extracting bounding boxes and confidence scores
- Comparing different confidence thresholds
- Performing instance segmentation
- Generating segmentation masks using SAM 2
- Comparing specialist and foundation models
- Exploring computer vision evaluation metrics

## Results

| Metric | Result |
|---|---|
| Sample image dimensions | 810 x 1080 |
| Supported YOLO11 classes | 80 |
| Detected objects | 5 |
| Bus detection confidence | 94.02% |
| YOLO11 detection inference | 12.3 ms |
| YOLO11 segmentation inference | 10.3 ms |
| YOLO11 segmentation masks | 6 |
| SAM 2 inference | 465.5 ms |

The object detection model identified four people
and one bus in the sample image.

The YOLO11 segmentation model generated six masks,
including four people, one bus, and one stop sign.

A second sample image produced detections for two
people and one tie.

These results demonstrate successful detection and
segmentation using pretrained models. Confidence
scores do not represent overall model accuracy.
Inference times depend on the runtime hardware.

## Key Findings

- Object detection identifies and locates objects.
- Segmentation provides pixel-level object outlines.
- Confidence thresholds affect detection results.
- Non-Maximum Suppression reduces duplicate detections.
- SAM 2 can generate masks using bounding box prompts.
- Precision, recall, IoU, and mAP are important
  metrics for evaluating computer vision systems.

## Technologies Used

- Python
- Ultralytics
- YOLO11
- YOLO11-Seg
- SAM 2.1
- PyTorch
- NumPy
- Matplotlib
- Pillow
- Google Colab
- Jupyter Notebook

## Dataset and Image Sources

The pretrained YOLO11 models use COCO object categories.

This project uses publicly available Ultralytics
sample images:

- https://ultralytics.com/images/bus.jpg
- https://ultralytics.com/images/zidane.jpg

No external dataset upload is required.

## How to Run

1. Open the Jupyter notebook in Google Colab.
2. Enable a GPU runtime if available.
3. Install the Ultralytics library.
4. Run all notebook cells in order.
5. Allow the pretrained model weights to download.
6. Review the detection and segmentation results.

## Real-World Applications

- Traffic monitoring
- Workplace safety
- Autonomous vehicles
- Manufacturing quality control
- Medical image analysis
- Robotics and automation

## References and Acknowledgments

- Ultralytics: https://docs.ultralytics.com/
- COCO Dataset: https://cocodataset.org/
- SAM 2: https://github.com/facebookresearch/sam2

This project was completed as part of the ITAI 1378
Computer Vision coursework.

Original lab author: Patricia McManus.
Original lab collaborator: Claude (Anthropic).
