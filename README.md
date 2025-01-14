# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.

## Program:

# Developed By: sasidharan 
# Register Number : 212221240049

```
# To Read,display the image

import cv2
image=cv2.imread("sasi.jpg")
cv2.imshow("image",image)
cv2.waitKey(0)

# To write the image
cv2.imwrite("image2.png", image)

# Find the shape of the Image
print(image.shape)

# To access rows and columns
for i in range(70,90):
for j in range(110,170):
image[i][j]=[0,0,0]
cv2.imshow("image",image)
cv2.waitKey(0)

# To cut and paste portion of image
image[70:90,110:175]=image[70:90,110:175]
cv2.imshow("image",image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

![image](1.png)

<br>
<br>

### ii)Write the image

![image](2.png)

<br>
<br>

### iii)Shape of the Image

![image](3.png)

<br>
<br>

### iv)Access rows and columns

![image](4.png)

<br>
<br>

### v)Cut and paste portion of image

![image](5.png)

<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.

