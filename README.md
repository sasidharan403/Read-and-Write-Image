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
image=cv2.imread("F4thai.png")
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

![image](https://user-images.githubusercontent.com/74660507/160992657-b8695c7f-aca1-47fd-80c6-1a598a378482.png)

<br>
<br>

### ii)Write the image

![image](https://user-images.githubusercontent.com/74660507/160993167-75b1ab3d-3a84-401c-85e2-e8be317454a7.png)

<br>
<br>

### iii)Shape of the Image

![image](https://user-images.githubusercontent.com/74660507/160993079-ae353ca4-dedf-48cb-bc2e-478ed53e9e7f.png)

<br>
<br>

### iv)Access rows and columns

![image](https://user-images.githubusercontent.com/74660507/160993376-f553254c-19c9-46da-a3d2-da9c7b96af85.png)

<br>
<br>

### v)Cut and paste portion of image

![image](https://user-images.githubusercontent.com/74660507/160993549-d4c5319e-32e4-4999-a3ed-35afdefe1aa8.png)

<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.

