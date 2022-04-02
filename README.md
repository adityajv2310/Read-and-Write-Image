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
#Developed By: Aditya JV

#Register Number: 212220230002

 #To Read,display the image
```
import cv2
color_image=cv2.imread('Batman.jpg', 1)
grey_image=cv2.imread('Batman.jpg', 0)
cv2.imshow('colorimage', color_image)
cv2.imshow('greyimage', grey_image)
cv2.waitKey(0)
```
 #To write the image
```
cv2.imwrite('new1.jpg', grey_image)
```
 #Find the shape of the Image
```
print(color_image.shape)
```
 #To access rows and columns

```
import random
for i in range(100):
    for j in range(color_image.shape[1]):
        color_image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("color",color_image)
cv2.waitKey(0)
```
 #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('Batman.jpg', -1)
tag=color_image[300:400, 300:400]
color_image[50:150, 50:150]=tag
cv2.imshow('color', color_image)
cv2.waitKey(0)

```


## Output:

### i) Read and display the image

![colorimage 02-04-2022 12_03_07](https://user-images.githubusercontent.com/75235386/161373801-565f7834-8aed-419e-9f06-204c4a015a1b.png)

![greyimage 02-04-2022 12_17_52](https://user-images.githubusercontent.com/75235386/161373851-a5eb5099-39d9-4398-9bf0-20f819593515.png)


### ii)Write the image


![Read and Write Image - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge 02-04-2022 13_49_26 (3)](https://user-images.githubusercontent.com/75235386/161374504-72b0cb6f-18bd-4b69-a08d-1561299934e2.png)


### iii)Shape of the Image

![Read and Write Image - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge 02-04-2022 13_49_26 (3)](https://user-images.githubusercontent.com/75235386/161374737-dca53147-db87-4f80-8734-32f4a9a7686b.png)


### iv)Access rows and columns

![color 02-04-2022 13_49_04](https://user-images.githubusercontent.com/75235386/161374555-6773a20f-da43-4076-b32e-a2b7a31e0c22.png)

### v)Cut and paste portion of image

![color 02-04-2022 13_49_13](https://user-images.githubusercontent.com/75235386/161374668-4211910e-a9ed-4df3-9b72-ecc9ab2bfb5b.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


