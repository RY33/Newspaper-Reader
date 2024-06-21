

# Newspaper Reader
## Description
This project utilizes YOLOv8 and other techniques to read newspapers. It identifies headings, subheadings, text bodies, and images from newspaper images or videos and converts them into an audio file for convenient listening. The project ensures the content is read in the correct order, following the hierarchy of headings, subheadings, and main text.

<picture><img src = "demo/Screenshot 2023-05-24 133156.png?raw=true" width = 550px></picture> 

### The following steps give breakdown of the the project:

### 1. Identifying components:
The YOLOv8 model is trained on a custom dataset to detect and classify different components in a newspaper, such as headings, subheadings, text bodies, and images.

### 2. Read order:
Custom algorithms are implemented to determine the order of reading, starting from headings, followed by subheadings (if any), and then the main text.

### 3. Image-to-text conversion:
Tesseract OCR is used to extract text from newspaper images and convert it into digital text.

### 4. Text-to-audio conversion:
The extracted text is converted into an audio file using GTTS (Google Text-to-Speech) .

## How to Run
Pre-trained model and notebook:

Use the provided pre-trained model and the accompanying Colab/Jupyter notebook.
If you only want to use the YOLO model, skip the training section of the notebook and proceed directly to the "Test" section. Modify the code according to your requirements in the "Read Order" part.
Note: Adjust the input and output locations in the code to match your setup. The default locations are set to my Google Drive.

## Train your own model:

To train your own YOLO model, refer to the "Training" section of the notebook.
Use the provided training dataset, which includes annotated images.
To create your own dataset, capture images of newspapers and annotate them using any annotation software, converting them into a YOLO-compatible format.
Note: Make sure to follow the instructions and adjust the code to suit your specific needs.
