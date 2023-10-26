This Python script is designed to perform image segmentation based on label files. It processes a set of images along with their corresponding label files, where the label files contain coordinates for segmenting objects in the images. The script reads the labels, creates segmentation masks, and overlays the masks on the original images, saving the segmented images in an "output" directory.

Requirements
To run this script, you will need the following dependencies:

Python
OpenCV (cv2)
NumPy
You can install these dependencies using popular package managers such as pip.

Usage
Ensure you have the required dependencies installed.
Organize your files as follows:
Images in the "images" directory
Label files in the "labels" directory
Run the script.
The script will process each label file, create segmentation masks, overlay them on the corresponding images, and save the segmented images in the "output" directory.

File Structure
images/: Directory containing the original images.
labels/: Directory containing label files with object coordinates.
output/: Directory where segmented images will be saved.
Output
The script produces segmented images in the "output" directory. Each segmented image retains the same name as the original image it was created from.

Note
The script uses label files to define object coordinates for segmentation.
It supports two classes: class 0 (green) and class 1 (red).
It scales the coordinates to match the size of the input image.
Example
Suppose you have an image named "example.jpg" in the "images" directory and a corresponding label file "example.txt" in the "labels" directory. After running the script, you will find the segmented image in the "output" directory as "example.jpg."
