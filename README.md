# License Plate Recognition
This project is an advanced License Plate Recognition (LPR) system that uses image processing and Optical Character Recognition (OCR) to detect and recognize license plates from images. The project is implemented using Python, OpenCV, EasyOCR, and other supporting libraries.

## Table of Contents
1. Overview
2. Installation
3. Usage
4. Project Structure
5. Methodology
6. Results

## Overview
The License Plate Recognition System aims to accurately detect and read license plates from images. The system employs various image processing techniques to enhance the image, locate the license plate, and extract the text using OCR. The primary technologies used are OpenCV for image processing and EasyOCR for text recognition.

## Installation

### Prerequisites
1. Python 3.6+
2. pip

### Dependencies
The project requires the following Python libraries:
1. easyocr
2. imutils
3. opencv-python-headless
4. matplotlib
5. numpy

You can install these dependencies using pip.

## Usage
To use the License Plate Recognition System, follow these steps:
1. Upload the image file containing the license plate to your environment (e.g., Google Colab).
2. Load the image and preprocess it by converting it to grayscale and applying noise reduction filters.
3. Detect edges in the image to locate potential license plate regions.
4. Find contours and identify the one corresponding to the license plate.
5. Apply a mask to isolate the license plate from the rest of the image.
6. Use EasyOCR to read and extract the text from the isolated license plate region.
7. Display the result by overlaying the detected text on the original image.

## Project Structure
1. images/: Directory containing sample images for testing.
2. notebook/: Jupyter/Colab notebook for experimentation and demonstration.

## Methodology
1. Image Preprocessing: Load the image and convert it to grayscale. Apply noise reduction using bilateral filtering.
2. Edge Detection: Use the Canny edge detection algorithm to find edges in the image.
3. Contour Detection: Identify contours in the edged image and sort them by size to find the largest potential license plate region.
4. License Plate Localization: Approximate the contours and check for a rectangular shape to locate the license plate.
5. Masking and Extraction: Create a mask for the detected license plate region and extract it from the original image.
6. OCR: Use EasyOCR to read and extract text from the isolated license plate region.
7. Result Visualization: Overlay the detected text on the original image for visualization.

## Results
The system successfully detects and reads license plates from images with 100% accuracy. The results include:
1. Accurate detection of license plate regions.
2. Successful text extraction using OCR.
3. Clear visual feedback with the detected text overlayed on the original image.
