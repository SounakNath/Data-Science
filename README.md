Real Time Sudoku Solver

This project has been orignally refered from https://github.com/anhminhtran235 and modified as per requirement here.

As the name suggests, the application solves standard Sudoku puzzle in real time. The application is based primarily on Image Processing and Machine Learning(CNN).

After the application starts, through video capturing, it identifies the Sudoku board, solves the puzzle and writes the solution on board itself.

References :

Data to train the CNN : Chars74K for Computer Fonts http://www.ee.surrey.ac.uk/CVSSP/demos/chars74k/

OpenCV Tutorials : https://www.geeksforgeeks.org/ , https://docs.opencv.org/

Python coding solutions : https://stackoverflow.com/

How does it work?

Below mentioned python modules are need as a prerequisite.

MainFile.ipynb is the entry point of the application.

The application converts colored image to gray scale, performs Gaussian blurring and then adaptive thresholding.

Then it finds the contours, gets the biggest contour, get corners, warp image according to perspective transform.

Then application solves the puzzle and displays the solution on image in real time

How to run?

Download all files. Ensure all mentioned python packages are installed. Run MainFile.ipynb

The Convoltional Neural Network(CNN) has been already been trained and the architecture(weights) have been stored in digitRecoginition.h5

Required Python Modules :

keras [2.8.0]

numpy [1.20.3]

opencv-python [4.5.5.64]

scipy [1.7.1]

import-ipynb [0.1.3]

tensorflow [2.8.0]
