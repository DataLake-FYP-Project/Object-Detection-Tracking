# YOLOv8 Training using CVAT annotation
This README explains how to organize dataset in Google Drive for training a YOLOv8 model.

# Folder Structure
*Root Folder*: Create a folder in your Google Drive (e.g., YOLO_Dataset).
*Subfolders*:
images: Contains training and validation images.
labels: Contains annotation files corresponding to the images.

# Steps to Prepare the Dataset
**Create the Main Folder:**
Create a folder in Google Drive named YOLO_Dataset.

**Create Subfolders:**

Inside YOLO_Dataset, create two subfolders:
images
labels

**Organize Training and Validation Data:**
Inside images, create two subfolders:
train: Place all the training images here.
val: Place all the validation images here.

Inside labels, create two subfolders:
train: Place all the annotation .txt files corresponding to the training images here.
val: Place all the annotation .txt files corresponding to the validation images here.

**Prepare Images:**
Ensure all images are in a supported format (e.g., .jpg, .png).
Place training images in YOLO_Dataset/images/train/.
Place validation images in YOLO_Dataset/images/val/.

**Prepare Annotations:**
Ensure all annotation files are in YOLO format (each .txt file contains the bounding box information for a corresponding image).
Place annotation files for training images in YOLO_Dataset/labels/train/.
Place annotation files for validation images in YOLO_Dataset/labels/val/.

# Important Notes
**Matching File Names:**
Each image must have a corresponding .txt file with the same name in the respective folder.
Example:
Image: train/image1.jpg
Annotation: labels/train/image1.txt

**Validation Data:**
The validation images and their annotations are used to evaluate the model during training.