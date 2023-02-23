# OMR Grader

Grader for bubble sheet multiple choice tests using Optical Mark Recognition, Python, and OpenCV. Images should be 300 dpi for maximum accuracy. This fork includes an option for multi-page PDF processing, very handy for grading multiple-choice exams in large groups.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisities

* Python 3
* OpenCV 3.4.3 or later
* NumPy
* imutils
* SciPy (Windows only)
* ZBar
* pyzbar

### Installing on Mac/Linux
To install the libraries, run the following commands:
```
$ brew install python3
$ pip install opencv-python
$ pip install numpy
$ pip install imutils
$ brew install zbar
$ pip install pyzbar
$ pip install xlsxwriter
$ pip install pdf2image
```

### Installing on Windows Subsystem for Linux
To install the libraries, run the following commands:
```
$ apt install python3
$ apt install python3-opencv
$ apt install python3-pip
$ pip3 install numpy
$ pip3 install scipy
$ pip3 install imutils
$ sudo apt-get install libzbar-dev libzbar0
$ pip3 install pyzbar
```

## Running

`$ python grader.py -i path [-v] [-d] [-s scale]`

### Flags
* `-i path`: path to image file
* `[-v]`: enable verbose mode - program will return image slices for every question
* `[-d]`: enable debug mode - program will display image slices to screen
* `[-s scale]`: factor to scale image slices by

## Acknowledgements
* Adrian Rosebrock's tutorial "Bubble sheet multiple choice scanner and test grader using OMR, Python, OpenCV"
* John Fremlin's tutorial "Rotating an image with OpenCV and Python"
