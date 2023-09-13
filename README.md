# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import opencv

### Step2:
Read the original Image.

### Step3:
Store the required conversion of the image in a variable.

### Step4:
Show the image stored in the given variable.

### Step5:
Destroy all the windows and end the program.

## Program:
### Developed By:    Ronick Aakshath P
### Register Number: 212222240084
### i) Convert BGR and RGB to HSV and GRAY
```
import cv2
houseImage = cv2.imread('pic.jpeg')
cv2.imshow('Original Image',houseImage)
hsvImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsvImage)
hsvImage1=cv2.cvtColor(houseImage,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(houseImage,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### ii)Convert HSV to RGB and BGR
```
import cv2
houseHSVImage = cv2.imread('pic.jpeg')
cv2.imshow('Original HSV Image',houseHSVImage)
RGBImage = cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage=cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### iii)Convert RGB and BGR to YCrCb
```
import cv2
houseImage = cv2.imread('pic.jpeg')
cv2.imshow('Original HSV Image',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('pic.jpeg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('Merged BGR image',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### v) Split and merge HSV Imageimport cv2
```
image = cv2.imread('pic.jpeg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow
```
## Output:
### i) BGR and RGB to HSV and GRAY
![1](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/0d626644-4324-4cf4-97ba-8aa1f3c2a005)
<br>
![2](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/df3be042-68d8-4879-8005-32d1f03db802)
<br>
![3](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/8bbb055f-a2b5-4f16-97bb-f0a56743c888)
<br>
![4](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/a965b950-6378-4891-8a2a-b9a2ec277b1b)
<br>
![5](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/79dadcad-4546-45f6-9a60-d63a5a58dfb0)

### ii) HSV to RGB and BGR
![6](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/64ef6f07-7ca8-4ba4-9bab-a3e1a8706a08)
<br>
![7](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/1025de9a-2efe-48ed-878c-2ceff88260b8)
<br>
![8](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/9dbe1d34-4c08-4324-b6b1-c4a38c312223)
<br>
### iii) RGB and BGR to YCrCb
![9](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/dc019036-81a0-478b-a6ea-55187ad2e21a)
<br>
![10](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/1ed695b2-66b2-4219-93e2-a39b465d5a17)
<br>
![11](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/ba80ca0b-b292-47ad-8148-59e600271fb9)
<br>
### iv) Split and merge RGB Image
![12](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/f34a146d-952d-4ac8-b514-22b099d02eca)
<br>
![13](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/62b12674-3749-448f-b16e-c6b139db2f8b)
<br>
![14](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/a2d130f9-be39-4d41-a692-6816d7aa7c4d)
<br>
![15](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/d84e20ae-fe6e-48b7-a5cf-6d8b89fb4365)
<br>
### v) Split and merge HSV Image
![16](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/ea937ccf-07e0-493a-9650-186c77a57175)
<br>
![17](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/b21cb6f4-4115-4e2f-8614-7f78e280b928)
<br>
![18](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/a63941ea-915d-4305-9c7f-c3d0d4ca95a5)
<br>
![19](https://github.com/Ronick2005/COLOR-CONVERSION/assets/83219341/3b7c7fab-b970-4c58-acb6-0328adadf4dd)
<br>
## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
