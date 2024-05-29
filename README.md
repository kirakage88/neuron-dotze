# Neuron

## Table of Contents
1. [Download](#download)
2. [Installation](#installation)
3. [Introduction](#introduction)
4. [Features](#features)
5. [Usage](#usage)
6. [Model](#model)
7. [Possible Errors and Fixes](#possible-errors-and-fixes)
8. [Notes](#notes)
9. [Future Updates/Features](#future-updatesfeatures)
10. [Contact](#contact)
11. [License](#license)

## Download
Due to the large file size, the installer will be linked through the following:  
[Neuron Installer](https://mega.nz/folder/QecCkCaZ#2uXeqCGW5okxbQ4Ya5XH_g)

Install app outside Program Files x86.
Recommended: Documents or Desktop or any directories that have no security access.

- Installer Size: 2.57 GB
- Folder Size: 7.50 GB

## Installation
Notes:
A terminal is shown to view any background processes such as downloading transfer models, matplotlib font cache building, training progress, etc. Also, opening the ppt
file would sometimes take a long time.

To install Neuron, follow these steps:
1. Install the app with the installer.
2. Right-click the directory of the app and then click 'Remove Access'.
3. Click Remove Access option.
4. Click Stop Sharing.


## Introduction
Neuron is an educational application designed to provide an in-depth understanding of Convolutional Neural Networks (CNNs), a cornerstone of modern computer vision. This project focuses on building a CNN model using custom datasets and utilizes the PyTorch library for developing and training the CNN. By integrating the powerful and flexible PyTorch workflow with a user-friendly Tkinter GUI, Neuron offers hands-on experience with deep learning, making the complex process of building and understanding CNNs more accessible.

The GUI serves as an educational tool that demonstrates how CNNs work in real-time, making Neuron approachable for users with varying levels of expertise in machine learning and computer vision. Whether you are a beginner looking to explore the basics or an advanced user aiming to deepen your knowledge, Neuron provides a comprehensive platform to enhance your understanding of CNNs.

## Features
- Interactive Trainable Models
- Interactive Predictor/Testing Models
- High Accuracy Pretrained Models (see notes)
- Introductory PowerPoint Presentation
- Data Visualization of Input and Output in Trainable Section

## Usage
After installing the application, you can use Neuron by following these steps:
- **Opening the app:** Opening the app can take a few seconds due to torch library initialization.

### Navigating the App

**Home Page**
1. Click the "Get Started" link to open the introductory presentation about Machine Learning.
2. Click the "Train" button to go to the Train Page.
3. Click the "Test" button to go to the Test Page.

**Train Page**
1. Click the dropdown and select the desired model; a visualization of data will show.
2. Enter any positive number of epochs. Training won't start unless you input a positive integer.
3. Click "Start" to start training.
4. The right box includes the training status, which includes the test and train losses, and test and train accuracies.
5. Click "Return" to return to the home page.

**Test Page**
1. Click the dropdown and select the desired model and wait for the ready status to show below the graph frame.
2. Drag and drop any images in a jpg format.
3. The image will then pop up alongside the predicted label and accuracy.
4. See the README Model section or details in the directory for further details about each model.

## Model

### 1. MNIST (Handwritten Digit Recognition)

**Details**
- The Hello World of Machine Learning
- A model used to recognize single handwritten digits (0-9) in an image size of 28x28 pixels.
- The model is trained specifically for inverted images in jpg format and RGB channel.
- The model boasts a training accuracy of 99% and testing accuracy of 99%, and is trained for a total of 445 seconds (~7 minutes). See documentation/ for further details.

**How to Use**
- Create a test image using MsPaint.
- In MsPaint, write any number in black color using the paintbrush, then use the 'select' tool in the home tab.
- Right-click the canvas then invert the colors.
- Save the test image in a jpg format.

### 2. Cats Vs Dogs Model (Cat and Dog Classification)

**Details**
- A model used to recognize whether a picture is of a cat or a dog.
- The model is trained specifically for images in jpg format and RGB channel.
- This model boasts a training accuracy of 95% and testing accuracy of 97%, and is trained for a total of 569 seconds (~9 minutes). See documentation/ for further details.

**How to Use**
- Use any image as long as the image is in jpg format and uses RGB channel.

### 3. Waste Model (Biodegradable, Non-Biodegradable, Recyclable Classification)

**Details**
- A model used to recognize certain classes of waste and classify them into biodegradable, non-biodegradable, and recyclable materials.
- This model is trained specifically for images in jpg format and RGB channel.
- This model boasts a training accuracy of 91% and testing accuracy of 93%, and is trained for a total of 2216 seconds (~37 minutes). See documentation/ for further details.

**How to Use**
- Use any image as long as the image is in jpg format and uses RGB channel.

**List**

**Biodegradable**
- coffee grounds
- eggshells
- food waste
- tea bags
- cardboard boxes
- cardboard packaging
- magazines
- newspaper
- office paper
- paper cups

**Non-Biodegradable**
- clothing
- shoes
- plastic shopping bags
- plastic straws
- plastic trash bags
- styrofoam cups
- styrofoam food containers

**Recyclable**
- aerosol cans
- aluminum food cans
- aluminum soda cans
- glass beverage bottles
- glass cosmetic containers
- glass food jars
- plastic cup lids
- plastic detergent bottles
- plastic food containers
- plastic soda bottles
- plastic water bottles
- steel food cans

## Possible Errors and Fixes
1. **Module Errors when opening the app**
   - Install the required libraries listed in the requirements txt.
  
2. **PPT file won't open**
   - Wait maybe for a few seconds or a minute and check terminal.
   - If nothing happens, or an error 'not found' would appear folow these steps:
   1. Open the app diretory, then copy the assets folder.
   2. Paste the folder inside the "_internal/".

3. **Model stuck at Loading**
     - Check Terminal to see if the model (EfficientNet Models) are currently downloading.

Note: If you encounter any error please attach an image of the error as well as the name of the issue ins the "Issues" page of the repository.

## Notes
- Regarding the defense, the app failed to recognize images due to an unrecognized error. The unrecognized error was a misindented load model function which would fail to load the saved parameters of any model, thus would only give random parameters and predict the image randomly.
- Regarding accuracies, accuracy is presented in a graph and PDF which is saved in the '.../documentation' directory.
- Open main-code.py to view the code of the app.
- The data folder (images used for training) will be sent through a Google Drive link.

## Future Updates/Features
- Add drawing canvas for MNIST Model.
- Allow the app to be resized and adjust according to the chosen resolution.
- Add settings for custom colors, changing trainable model parameters (Learning Rate, etc.).
- Add more data visualizations (Confusion Matrix, etc.).
- Add Fashion MNIST Model.
- Improve Accuracy of Waste Model.
- Add other models.
- Include 'Creating and Training your own Model with PyTorch' course/presentation.
- Add videos for increased usage accessibility.
- Add Model Summaries.
- Improve presentation, add links to courses or other related links.

## Contact
For any questions or feedback, and if you wish to provide more datasets to add a model or improve a model, please contact us through the following:

- Email: 200931726@my.xu.edu.ph

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
