# HCL-INTERNSHIP-COLOR RECOGNITION USING PYTHON AND OPENCV
## COLOR RECOGNITION USING PYTHON AND OPENCV

In this color recognition Python project, we are going to build an application through which user can automatically get the name of the color('RED,GREEN,BLUE) when webcam is opened

# TECHNOLOGIES USED:

Python

OpenCv

Numpy

# SYSTEM ARCHITECTURE:

![Screenshot (632)](https://user-images.githubusercontent.com/109220331/200894302-e5c0b529-48d5-4fd3-813f-378a877a355a.png)

# WORKFLOW:

![Screenshot (634)](https://user-images.githubusercontent.com/109220331/200894877-6b387dc0-c1bd-419b-9e18-775eca4595b6.png)

# WORKFLOW DESCRIPTION:

Step 1: The first step is to capture the video through the webcam with “cv2.VideoCapture()”. 

Step 2: It is reading the video from the webcam in image frames with “cv2.imread()”

Step 3: Convert the image frame in BGR (BLUE, GREEN, RED) to HSV(hue-saturation-value It stores color information in a cylindrical representation of RGB color points. Hue value varies from 0-179 Saturation value varies from 0-255 and Value value varies from 0-255. It is mostly used for color segmentation purpose.) “hsv=cv2.cvtColor(image, cv2.Color_BGR2HSV)” . 

Step 4: Set the minimum and maximum range of HSV for red green and blue and define the mask for highlight a specific object from the image . 
”mask=cv2.inRange(hsv, min, max)”. 

Step 5: We use kernel for blur an image and Dilation for remove noises from the image. For each color. 
“Cv2.dilate()” 

Step 6: We use bitwise_and operator between the image frame and mask is performed to specifically detect the particular color and leave other color. “Cv2.bitwise_and()”. 

Step 7: Create contour for the individual colors to display the detected colored region distinguish. 

Step 8: Output is detected of the colors name in the real time.

#OUTPUT:

OUTPUT IMAGE FOR COLOR RED

![Screenshot (628)](https://user-images.githubusercontent.com/109220331/200895382-8a6fcf4c-c1e6-4f7d-9041-7e6ac6d5ac3d.png)

OUTPUT IMAGE FOR COLOR GREEN

![Screenshot (629)](https://user-images.githubusercontent.com/109220331/200895450-337f3404-fa10-4595-bd35-553d887e5731.png)


OUTPUT IMAGE FOR COLOR BLUE

![Screenshot (630)](https://user-images.githubusercontent.com/109220331/200895529-dfb17967-8139-43c3-9230-52df7731bcc0.png)
