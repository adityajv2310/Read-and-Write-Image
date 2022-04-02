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
### Developed By:Aditya JV
### Register Number:212220230002
i) #To Read,display the image
import cv2
import random
col=cv2.imread("su.jpg",1)
cv2.imshow("col",col)
cv2.waitKey(0)

#Gray Image
gray=cv2.imread("su.jpg",0)
cv2.imshow("gray",gray)
cv2.waitKey(0)

ii) #To write the image
cv2.imwrite("iron.jpg",gray)

iii) #Find the shape of the Image
print(col.shape)

iv) #To access rows and columns
import random
for i in range(100):
for j in range(col.shape[1]):
col[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("col",col)
cv2.waitKey(0)

v) #To cut and paste portion of image
color=cv2.imread("su.jpg",1)
tag=color[300:400,300:400]
color[50:150,50:150]=tag
cv2.imshow("color",color)
cv2.waitKey(0)

## Output:

### i) Read and display the image

![Screenshot (156)](https://user-images.githubusercontent.com/75235386/161376402-4e511311-5f46-4310-98a8-6418a2ceaa0b.png)

Gray image
![Screenshot (157)](https://user-images.githubusercontent.com/75235386/161376424-f96ce0ee-cbc7-4639-92b2-e0a2785a90d6.png)


### ii)Write the image
![Screenshot (160)](https://user-images.githubusercontent.com/75235386/161376550-9db8aea0-6890-43b3-8dc8-eef1e09afe00.png)


### iii)Shape of the Image
![Screenshot (160)](https://user-images.githubusercontent.com/75235386/161376554-f50f184a-4115-4878-963b-8085d1d0a4e4.png)


### iv)Access rows and columns
![Screenshot (158)](https://user-images.githubusercontent.com/75235386/161376561-cb6649d2-d802-4fd5-afaf-bb88623f67bb.png)


### v)Cut and paste portion of image
![Screenshot (159)](https://user-images.githubusercontent.com/75235386/161376566-b88fd129-8a4e-43fd-a0cc-1998342dcc74.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


