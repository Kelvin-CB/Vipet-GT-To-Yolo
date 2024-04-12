## Author

This project was developed by Kelvin Carvalho. If you have any questions, suggestions, or would like to contribute to the project, please feel free to contact:

- [Kelvin Carvalho](mailto:devkel.kcb@gmail.com)


# Viper-GT Video Annotations Converter to VOC and YOLOv8 Format

This project consists of a Python code in Jupyter Notebook format that converts videos annotated with Viper-GT software to sequences of video frames with annotations in VOC format, and subsequently converts these VOC annotations to YOLOv8 dataset format.

## Requirements

- Python 3.8
- Jupyter Notebook
- Python Libraries: cv2, matplotlib, numpy, xml.etree.ElementTree, sys, pickle, warnings, shutil, os, pandas, re, moviepy, json

## Features

### 1. Video to Image Sequences and Annotations Conversion

The first cell of the notebook handles the conversion process of annotated videos generated by Viper-GT. It takes the input video and transforms it into a series of JPG frames, preserving the annotations. Additionally, for each frame, it generates a corresponding JSON file containing the annotations specific to that frame. This conversion process allows for easier manipulation and analysis of individual frames and their associated annotations.

### 2. Conversion of Viper-GT Annotations to YOLOv8 Format

The second cell focuses on the conversion of the frames and annotations obtained from the previous step into a format compatible with YOLOv8, a popular object detection framework. This conversion is crucial for training YOLOv8 models using the annotated data. The annotations are processed and transformed into text files with specific formatting required by YOLOv8. This step enables seamless integration of the annotated data into the YOLOv8 training pipeline, facilitating the development of accurate object detection models.



## Usage

1. Make sure you have all the requirements installed.
2. Input the path of the annotated video and the path of the Viper-GT annotation file.
3. Choose a path for the output folder of the generated images/frames and annotations.
4. Choose a name for the object you want to extract from the annotations.
5. Choose the path for the output folder of yolov8 dataset.
5. Run the notebook.

## Project Structure

- **Root Folder**: Root folder for the project.
  - **AnnotatedVideoFilePath**: Folder containing annotated videos.
  - **xgtfFilePath**: Folder containing Viper-GT annotation files (`.xgtf`).
  - **OutputImagesFolderPath**: Output folder for generated images/frames.
  - **OutputAnnotationsFolderPath**: Output folder for converted annotation files.
  - **YoloV8DatasetPath**: Output folder for dataset in YOLOv8 format.


## Contribution

Contributions are welcome! Feel free to open issues and send pull requests.
