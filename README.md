# FISH-DETECTION
A robust fish detection model for real-time underwater fish detection in any marine environments using yolov7.
![Screenshot 2024-04-12 105641](https://github.com/meerap1/FISH-DETECTION/assets/156745402/4e4f685c-247d-44a7-b076-523683229a50)

## Table of Content
1. Introduction
2. Data Source
3. Creating Virtual Environment
4. Setup Yolov7 Repository
5. Modify Yolov7 files
6. 


### Introduction
I'm excited to share with you my latest project: a YOLOv7 model for fish detection. Leveraging state-of-the-art deep learning techniques, this model is designed to accurately identify and localize fish in images. Utilizing Anaconda Prompt, I've crafted an environment where you can easily set up and run the model on your own machine.

### Data Source:
The data used in this repository for fish object detection in marine videos was sourced from another repository, which provided annotated video clips. A subset of over 1500 + images from this dataset was selected for training purposes. This curated dataset encompasses both positive and negative images, where positive images contain instances of fish, annotated with bounding boxes and class labels, while negative images depict marine scenes without fish objects.

### Creating Virtual Environement:
To create a virtual environment, open Anaconda Prompt and use the following code: <br/>
<br/>
`conda create -n yolov7_custom python=3.9` <br/>
<br/>
After hitting enter, type 'Y' and hit enter again. Once the environment is created, activate it with the command: <br/>
<br/>
`conda activate yolov7_custom` <br/>
<br/>
###  Setup Yolov7 Repository
Download the official YOLOv7 repository from the [link](https://github.com/WongKinYiu/yolov7) <br/>
<br/>
Download the zip file into your **yolov7_custom** folder. Once downloaded, unzip it and rename the folder to **yolov7_custom**. Then, move the folder to the main directory **yolov7_custom**and delete the empty directory. <br/>
<br/>
Inside the extracted repository, open the **requirements.txt** file. Check the Torch version; it should be greater than or equal to 1.7 but not 1.12. Similarly, the TorchVision version should be greater than or equal to 0.8.1 but not 0.13. Make note of these versions and visit the PyTorch website to install PyTorch with CUDA support, meeting the requirements listed in the txt files. <br/>
<br/>
![Screenshot 2024-04-16 115159](https://github.com/meerap1/FISH-DETECTION/assets/156745402/b0e2bf66-3340-48e4-bc3a-0f1cf753b797) <br/>
<br/>
Remove the lines referencing Torch and TorchVision from the 'requirements.txt' file, then save the file. Additionally, create a new text file and paste the pip install command used to install PyTorch with CUDA support. Ensure the command is correctly formatted, like so: <br/>
![Screenshot 2024-04-16 120410](https://github.com/meerap1/FISH-DETECTION/assets/156745402/d0187060-3507-4bc9-a362-e672b4788189)  <br/>
 <br/>
Save the file as **requirements_gpu.txt** <br/>
<br/>
Now, in Anaconda Prompt, navigate to the **yolov7_custom** directory and execute the command: <br/>
<br/>
`pip install -r requirements.txt` <br/>
<br/>
this will install all the libraries that are part of the requirements.txt once it is done execute another command <br/>
<br/>
`pip install -r requirements_gpu.txt` <br/>
<br/>
This will install PyTorch with CUDA support. <br/>
<br/>
### Modify Yolov7 Files




