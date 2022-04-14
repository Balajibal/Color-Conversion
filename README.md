# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
 Convert BGR and RGB to HSV and GRAY

### Step2:
Convert HSV TO RGB AND BGR

### Step3:
Convert RGB and BGR to YCrCb

### Step4:
To Split and merge RGB Image

### Step5:
To Split and merge HSV Image

## Program:
```python
# Developed By: BALAJI N
# Register Number: 212220230006
# i) Convert BGR and RGB to HSV and GRAY
import cv2
goku = cv2.imread('goku.jpg')
modimg1 = cv2.cvtColor(goku,cv2.COLOR_BGR2HSV)
cv2.imshow('COLOR_BGR2HSV',modimg1)
cv2.waitKey(0)
modimg2 = cv2.cvtColor(goku,cv2.COLOR_RGB2HSV)
cv2.imshow('COLOR_RGB2HSV',modimg2)
cv2.waitKey(0)
modimg3 = cv2.cvtColor(goku,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',modimg3)
cv2.waitKey(0)
modimg4 = cv2.cvtColor(goku,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',modimg4)
cv2.waitKey(0)





# ii)Convert HSV to RGB and BGR
modimg5 = cv2.cvtColor(goku,cv2.COLOR_HSV2BGR)
cv2.imshow('COLOR_RGB2HSV',modimg5)
cv2.waitKey(0)
modimg6 = cv2.cvtColor(goku,cv2.COLOR_HSV2RGB)
cv2.imshow('COLOR_HSV2RGB',modimg6)
cv2.waitKey(0)





# iii)Convert RGB and BGR to YCrCb
modimg7 = cv2.cvtColor(goku,cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb',modimg7)
cv2.waitKey(0)
modimg8 = cv2.cvtColor(goku,cv2.COLOR_BGR2YCrCb)
cv2.imshow('RCB2YCrCb',modimg8)
cv2.waitKey(0)




# iv)Split and Merge RGB Image
import cv2
img = cv2.imread("goku.jpg")
b,g,r = cv2.split(img)
cv2.imshow("RED MODEL", r)
cv2.imshow("GREEN MODEL", g)
cv2.imshow("BLUE MODEL ", b)
merger = cv2.merge([b,g,r])
cv2.imshow("MERGED IMAGE", merger )
cv2.waitKey(0)
cv2.destroyAllWindows()


# v) Split and merge HSV Image
import cv2
img = cv2.imread("goku.jpg")
img1= cv2.resize(img, (270,190))
hsv = cv2.cvtColor(img1 , cv2.COLOR_BGR2HSV)
cv2.imshow("INITIAL_HSV ", hsv)
h,s,v = cv2.split(hsv)
cv2.imshow("RED MODEL", h)
cv2.imshow("GREEN MODEL", s)
cv2.imshow("BLUE MODEL ", v)
merger = cv2.merge([h,s,v])
cv2.imshow("MERGED IMAGE", merger )
cv2.waitKey(0)
cv2.destroyAllWindows()




```
## Output:
### i) Original Image
![goku](https://user-images.githubusercontent.com/75234946/162558259-a5743cd3-d94c-4b6c-abc9-71a68af11e47.jpg)

### ii) BGR and RGB to HSV and GRAY
![Screenshot (37)-COLLAGE](https://user-images.githubusercontent.com/75234946/163384517-fcfda655-6ce4-47d9-b585-17165eea4b3c.jpg)





### iii) HSV to RGB and BGR
![Screenshot (44)-COLLAGE](https://user-images.githubusercontent.com/75234946/163384850-349f59e5-04ed-46a2-9013-bd5c1091fc76.jpg)




### iv) RGB and BGR to YCrCb
![Screenshot (51)-COLLAGE](https://user-images.githubusercontent.com/75234946/163385132-7e2bfad1-39c4-45a1-839a-a90c1c72e548.jpg)




### v) Split and merge RGB Image
![Screenshot (73)-COLLAGE](https://user-images.githubusercontent.com/75234946/163385817-22d191ac-43f1-4736-af43-7469dec7f0d0.jpg)


### vi) Split and merge HSV Image
![Screenshot (77)-COLLAGE](https://user-images.githubusercontent.com/75234946/163387253-9d87a80d-7c81-4142-b15e-55e14e79aaf0.jpg)




## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
