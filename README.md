# Car License Plates Reader
## Image Processing 2023-2024

Authors:  </br>
Luke
Panos

## Description of the project
This is a project based on Image Processing technology and it aims to give the user the ability to import sample images of cars with license plates displayed. The product will read and recognize by returning the license plate number into text.

## Technology Selection
|     Technology     |        Description        |                Official website                |
| :----------------: | :----------------------:  | :--------------------------------------------: |
|        Python      | Python Programming Language |               https://www.python.org/        |
|        OpenCV      | Open Computer Vision Library |               https://opencv.org/           |
|  Jupyter Notebook  | interactive development environment for notebooks |               https://jupyter.org/           |


## How it works:

![Step-by-step illustration of Licence Plate Isolation](Sample%20Inputs/garda_car.gif)

We start by reading in our image of the vehicle with a licence plate visible. We then convert this image to HSV, extracting the V channel to perform our thresholding, after which we draw and fill in the contours that meet our requirements (i.e. roughly following standardized plate formats). After which we use the drawn contours to extract the ROI (region of interest) where the licence plate should be.