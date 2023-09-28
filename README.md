# Hand Segmentation using YOLOv8 and SAM

This repository contains a solution for segmenting hands from images and producing accurate results by removing the background. The task is based on a dataset provided by Aitaca, which can be accessed [here](https://drive.google.com/file/d/1Mc72BLGnZZQ0mhnh9rHOdJzYmITN-PPL/view?usp=sharing).

## Before You Start
Before you begin working on this task, make sure you have the following prerequisites in place:

1. **Install ultralytics**: You will need YOLOv8 for object detection and segmentation. Follow the installation instructions for YOLOv8.

2. **Import Necessary Libraries**: Ensure that you have the necessary Python libraries installed, including but not limited to OpenCV, NumPy, and PyTorch.

## Data Processing
1. **Create a New Dataset Structure**
To work with the provided dataset, you should create a new structure that organizes the data. You may need to divide the dataset into training and testing subsets.

2. **Auto-Annotation**
You can perform auto-annotation to label the hand regions in your dataset. This can be done using tools like labelImg or custom scripts to create YOLOv8-compatible annotations.

3. **Generate Segmentation Dataset Using YOLOv8 and SAM**
Use YOLOv8 and SAM (Semantic Autoencoder Model) to generate a segmentation dataset from the annotated data. This step helps in creating pixel-wise segmentation masks for the hands.

4. **Create a New Dataset with Train/Val Sets**
Split your dataset into training and validation sets. Ensure that you have a clear structure for organizing images and corresponding segmentation masks.

## Train YOLOv8 Instance Segmentation Model
**Custom Training**
Train a custom YOLOv8 model on your segmented dataset. Fine-tune the model to accurately detect and segment hands in images.

**Validate Custom Model**
Evaluate the performance of your custom model on a validation set to ensure it meets the accuracy requirements for background removal.

**Save Trained Model**
Save the trained YOLOv8 model along with the weights so that it can be used for background removal.

## Background Removal
Use the trained model to remove the background from images containing hands.

# Repository Structure
**Notebook**: Jupyter Notebook file that provide code and explanations for the steps mentioned above.
`Hand_Segmentation_in_Images.ipynb`
**Dataset YAML format**:Example of the YAML format used for defining our dataset.
`dataset.yaml`
## YOLOv8 instance segmentation pretrained model
the Link of the best YOLOv8 instance segmentation pretrained model.  [here](https://drive.google.com/file/d/1XmHYqArq4yagI5MOiQrVUQdNvT_q_lNH/view?usp=sharing).


