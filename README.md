# image-processing-lab
🆈🅰🆂🅷🆆🅸🅽🅳<br>
__1.Develop a program to display grayscale image as tiny real and write program<br>__
import cv2<br>
img1=cv2.imread('flower5.jpg',0)<br>
cv2.imshow('flower3',img1)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

![image](https://user-images.githubusercontent.com/98301023/173814042-1f9fd68f-504c-42d3-b854-ff58bf7b027f.png)<br>
<br>
-----------------------------------------------------------------------------------------------------------------------------<br>

2.develop a program to display image to string using metaplotlib<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=mping.imread('flower5.jpg')<br>
plt.imshow(img)<br>

![image](https://user-images.githubusercontent.com/98301023/173814171-2a69155b-4f01-4945-a3ee-eae3aef6bca4.png)<br>



__3.Develop program to perform linear transfermation rotation<br>__
from PIL import Image<br>
img=Image.open("flower3.jpg")<br>
img=img.rotate(180)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

![image](https://user-images.githubusercontent.com/98301023/173815233-90a533a5-efb8-48e2-8a35-fc0b7b9761aa.png)<br>



4.develop a programt to convert color,string to RGB order value<br>
from PIL import ImageColor<br>
#using getrgb for yellow<br>
img1=ImageColor.getrgb("yellow")<br>
print(img1)<br>
#using getrgb for red<br>
img2=ImageColor.getrgb("red")<br>
print(img2)<br>

(255, 255, 0)<br>
(255, 0, 0)
<br>


5.write program to create image using color<br>
from PIL import Image<br>
img=Image.new('RGB',(200,400),(235,255,0))<br>
img.show()<br>

![image](https://user-images.githubusercontent.com/98301023/173815623-c11c4d89-1831-4ee0-a4c2-593f498fc683.png)<br>

<br>

6.develop a program to visualize the image using various color spaces<br>
import cv2<br>
import matplotlib.pyplot as plt<br>
import numpy as np<br>
img=cv2.imread("flower3.jpg")<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
plt.imshow(img)<br>
plt.show()<br>
<br>
![image](https://user-images.githubusercontent.com/98301023/173815954-0de5ebd4-3533-46ba-a3f6-6ea6ccb27355.png)<br>

![image](https://user-images.githubusercontent.com/98301023/173816038-7a4d7d84-002b-47fe-8b06-b3fd613c21ee.png)<br>

![image](https://user-images.githubusercontent.com/98301023/173816088-5b584ac4-cbc8-47ed-96b1-1fb5c5c2e45b.png)<br>


<br>
7.write aprogram to display the image altribute <br>
from PIL import Image<br>
image=Image.open("flower5.jpg")<br>
print("Filename",image.filename)<br>
print("format",image.format)<br>
print("mode",image.mode)<br>
print("size",image.size)<br>
print("width",image.width)<br>
print("height",image.height)<br>
image.close()<br>


Filename flower5.jpg<br>
format JPEG<br>
mode RGB<br>
size (255, 132)<br>
width 255<br>
height 132<br>





8.convert the original image to gray scale and then to to binary<br>
import cv2<br>
img=cv2.imread("plants2.jpg")<br>
print('original image length width',img.shape)<br>
cv2.imshow('original image',img)<br>

#to show resize image<br>
imgresize=cv2.resize(img,(150,160))<br>
cv2.imshow('resized image',imgresize)<br>
print('resized image length width',imgresize.shape)<br>
cv2.waitKey(0)<br>

OUTPUT
original image length width (751, 1000, 3)
resized image length width (160, 150, 3)

![image](https://user-images.githubusercontent.com/98301023/174042548-3d1ec7ff-8b7f-4add-8431-5125c716c172.png)<br>


resized image
![image](https://user-images.githubusercontent.com/98301023/174042760-0bc4c7da-374c-42a0-bd1e-ad6864fe8fc7.png)





9.convert image to binary<br>
#read the image file<br>

img=cv2.imread('butterfly1.jpg')<br>

cv2.imshow("RGB",img)<br>

<br>


#grayscale<br>

img=cv2.imread("butterfly1.jpg",0)<br>

cv2.imshow("gray",img)<br>



#binary image<br>

ret,bw_img=cv2.threshold(img,127,255,cv2.THRESH_BINARY)<br>

cv2.imshow("binary",bw_img)<br>

cv2.waitKey(0)<br>

cv2.destroyAllWindows()<br>

OUTPUT
![image](https://user-images.githubusercontent.com/98301023/174045192-d8c64d61-cad7-4ebc-8640-54f776bb8ba9.png)<br>
![image](https://user-images.githubusercontent.com/98301023/174049390-d6114a69-30e3-4ff7-81f0-2d6e1e8e5b7b.png)<br>


![image](https://user-images.githubusercontent.com/98301023/174049599-4d11d4d7-6f00-479a-8edb-357df4388477.png)<br>




import cv2<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('flower3.jpg')<br>
plt.imshow(img)<br>
plt.show<br>


![image](https://user-images.githubusercontent.com/98301023/175273060-a77cf8ee-f8d3-4471-b16c-c11e1cb43650.png)<br>


10.develop a program to read the image using URl<br>
from skimage import io<br>
import matplotlib.pyplot as plt<br>
url='https://i.guim.co.uk/img/media/a7fe7170defa865d2b96b829f05c5d8fa82d8edf/0_20_2201_1321/master/2201.jpg?width=465&quality=45&auto=format&fit=max&dpr=2&s=72bbae118ff1631bcc0d1f837159a727'<br>
image=io.imread(url)<br>
plt.imshow(image)<br>
plt.show()<br>


![image](https://user-images.githubusercontent.com/98301023/175273244-5fb34328-be3e-4be2-b583-c733ae7c9f2e.png)<br>


11.program to musk and blur the image
import cv2<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('fish.jpg')<br>
plt.imshow(img)<br>
plt.show<br>


![image](https://user-images.githubusercontent.com/98301023/175273430-7bed0f3c-8bc8-40bf-b26c-8b5bdc02f204.png)<br>




hsv_img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
light_orange=(170, 255, 128)<br>
dark_orange=(179, 204, 245)<br>


mask=cv2.inRange(img,light_orange,dark_orange)<br>
result=cv2.bitwise_and(img,img,mask=mask)<br>


plt.subplot(1,2,1)<br>
plt.imshow(mask,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result)<br>
plt.show()<br>


![image](https://user-images.githubusercontent.com/98301023/175273790-3f9061f4-8f59-4678-82f1-96e3a54ad2d3.png)<br>




light_white=(0,190,200)<br>
dark_white=(0,0,139)<br>
mask_white=cv2.inRange(hsv_img,light_white,dark_white)<br>
plt.subplot(1,2,1)<br>
plt.imshow(mask_white,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result_white)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/98301023/175274069-3cc0c31c-be60-441a-81e9-f518662920c0.png)<br>


final_mask=mask+mask_white<br>
final_result=cv2.bitwise_and(img,img,mask=final_mask)<br>
plt.subplot(1,2,1)<br>
plt.imshow(final_mask,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(final_result)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/98301023/175274187-bca6203d-7d25-4593-88b6-405a48c30522.png)



blur=cv2.GaussianBlur(final_result,(7,7),0)<br>
plt.imshow(blur)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/98301023/175274306-18099bd8-dc48-4a1f-a766-5fa8b06d771d.png)<br>
<br>


12.dervelop the program to change the image to different color spaces<br>
import cv2 <br>
img=cv2.imread('fish.jpg')<br>
gray=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)<br>
hsv=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)<br>
lab=cv2.cvtColor(img,cv2.COLOR_BGR2LAB)<br>
hls=cv2.cvtColor(img,cv2.COLOR_BGR2HLS)<br>
yuv=cv2.cvtColor(img,cv2.COLOR_BGR2YUV)<br>
cv2.imshow("gray image",gray)<br>
cv2.imshow("hsv image",hsv)<br>
cv2.imshow("LAB image",lab)<br>
cv2.imshow("HLS image",hls)<br>
cv2.imshow("YUVimage",yuv)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>


![image](https://user-images.githubusercontent.com/98301023/175275496-6503a469-9416-4a57-adfd-78d23889324c.png)<br>
![image](https://user-images.githubusercontent.com/98301023/175275575-e95e3b15-d9e4-4634-893f-61ec69b108b1.png)<br>
![image](https://user-images.githubusercontent.com/98301023/175275672-fe041d01-f413-4166-9b3d-f3898a0ef00c.png)<br>
![image](https://user-images.githubusercontent.com/98301023/175275779-769d7666-ae65-4232-b9f4-7e4654d54bb3.png)<br>
![image](https://user-images.githubusercontent.com/98301023/175275923-53dda87d-076d-479a-af9d-07f5faa08c1f.png)<br>




13.program to create an image using 2D array<br>
import cv2 as c<br>
import numpy as np<br>
from PIL import Image<br>
array=np.zeros([100,200,3],dtype=np.uint8)<br>
array[:,:100]=[255,130,0]<br>
array[:,100:]=[0,0,255]<br>
img=Image.fromarray(array)<br>
img.save('gfhgh.png')<br>
img.show()<br>
c.waitKey(0)<br>

![image](https://user-images.githubusercontent.com/98301023/175276188-391249d1-76a0-4f05-a8db-0c454ece37a9.png)<br>



<br>

<br>
14.Write the program to perform arithmatic operation on image<br>
import cv2<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img1=cv2.imread('fish.jpg')<br>
img2=cv2.imread('plants1.jpg')<br>
#applying numpy addition on images<br>
fimg1=img1+img2<br>
plt.imshow(fimg1)<br>
plt.show()<br>
#saving the output image <br>
cv2.imwrite('output.jpg',fimg1)<br>
fimg2=img1-img2<br>
plt.imshow(fimg2)<br>
plt.show()<br>
#saving the output image<br>
cv2.imwrite('output.jpg',fimg2)<br>
fimg3=img1*img2<br>
plt.imshow(fimg3)<br>
plt.show()<br>
#savin the output image<br>
cv2.imwrite('output.jpg',fimg3)<br>
fimg4=img1/img2<br>
plt.imshow(fimg4)<br>
plt.show()<br>
#saving the output image<br>
cv2.imwrite('output.jpg',fimg4)<br>



![image](https://user-images.githubusercontent.com/98301023/175278179-66d43b70-5e04-4e78-9e0e-9e9dac5172aa.png)<br>
![image](https://user-images.githubusercontent.com/98301023/175278220-8f7705fc-3cd4-4f30-b702-9674b43e5c4a.png)<br>
![image](https://user-images.githubusercontent.com/98301023/175278270-eaf26329-a72a-45cf-a6e2-e82619373ad8.png)<br>
![image](https://user-images.githubusercontent.com/98301023/175278392-8ff56508-97ae-416f-985e-02a64b40f9f3.png)<br>
<br>




28-06-2022<br>
15.Program to implement bitwise operation <br>
1.import cv2<br>
import matplotlib.pyplot as plt<br>
image1=cv2.imread('butterfly1.jpg',1)<br>
image2=cv2.imread('butterfly1.jpg')<br>
ax=plt.subplots(figsize=(15,10))<br>
bitwiseAnd=cv2.bitwise_and(image1,image2)<br>
bitwiseor=cv2.bitwise_or(image1,image2)<br>
bitwisxor=cv2.bitwise_xor(image1,image2)<br>
bitwiseNot_img1=cv2.bitwise_not(image1)<br>
bitwiseNot_img2=cv2.bitwise_not(image2)<br>
plt.subplot(151)<br>
plt.imshow(bitwiseAnd)<br>
plt.subplot(152)<br>
plt.imshow(bitwiseor)<br>
plt.subplot(153)<br>
plt.imshow(bitwisxor)<br>
plt.subplot(154)<br>
plt.imshow(bitwiseNot_img1)<br>
plt.subplot(155)<br>
plt.imshow(bitwiseNot_img2)<br>
cv2.waitKey(0)<br>


OUTPUT<br>
![image](https://user-images.githubusercontent.com/98301023/176416526-f15dcd56-75bf-4984-9b3a-3fed4669d9fd.png)<br>


16.program to implement various blur technique<br>
<br>
import cv2<br>
import numpy as np<br>

image=cv2.imread('butterfly1.jpg')<br>
cv2.imshow('original image',image)<br>


#gaussian Blur<br>
Gaussian=cv2.GaussianBlur(image,(7,7),0)<br>
cv2.imshow('Gaussian Blurring',Gaussian)<br>


#median Blurring<br>
median=cv2.medianBlur(image,5)<br>
cv2.imshow('median Blurring',median)<br>


#Bilateral Blur<br>
bilateral=cv2.bilateralFilter(image,9,75,75)<br>
cv2.imshow('Bilateral Blurring',bilateral)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

OUTPUT<br>
![image](https://user-images.githubusercontent.com/98301023/176417321-2c05839d-f190-4626-8927-92864166efdd.png)<br>

![image](https://user-images.githubusercontent.com/98301023/176417490-685f0d0c-8ba0-4f48-a33c-76db43326d6d.png)<br>

![image](https://user-images.githubusercontent.com/98301023/176417610-2ab1ddf7-d545-4442-ad3e-ad6a1dfbf4f2.png)<br>


![image](https://user-images.githubusercontent.com/98301023/176417769-b349a555-9313-4ec1-a6b9-cbfab29c1adb.png)<br>
<br>


17.Program to perform Image Enhancement<br>
from PIL import Image<br>
from PIL import ImageEnhance<br>
Image=Image.open('butterfly1.jpg')<br>
Image.show()<br>
enh_bri=ImageEnhance.Brightness(Image)<br>
brightness=1.5<br>
image_brightened=enh_bri.enhance(brightness)<br>
image_brightened.show()<br>
enh_col=ImageEnhance.Color(Image)<br>
color=1.5<br>
image_colored=enh_col.enhance(color)<br>
image_colored.show()<br>
enh_con=ImageEnhance.Contrast(Image)<br>
contrast=1.5<br>
image_contrasted=enh_con.enhance(contrast)<br>
image_contrasted.show()<br>
enh_sha=ImageEnhance.Sharpness(Image)<br>
sharpness=3.0<br>
image_sharped=enh_sha.enhance(sharpness)<br>
image_sharped.show()<br>

OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98301023/176419998-a8671fe9-e4d7-4c07-9b19-8ee45af7aa50.png)<br>


![image](https://user-images.githubusercontent.com/98301023/176420108-6e2e5573-b534-4e44-9bfb-abd53b2d0e98.png)<br>

![image](https://user-images.githubusercontent.com/98301023/176420158-556aef84-f2e2-46e5-b106-ebbf3cbfade1.png)<br>


![image](https://user-images.githubusercontent.com/98301023/176420236-93808c30-a360-486e-880d-c54fd24ef82c.png)<br>


![image](https://user-images.githubusercontent.com/98301023/176420455-0cb8b177-c106-4e40-9971-ff5bd5039a35.png)





18.program to perform Morphology operation<br>
import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
from PIL import Image,ImageEnhance<br>
img=cv2.imread('dog1.jpg',0)<br>
ax=plt.subplots(figsize=(20,10))<br>
kernel=np.ones((5,5),np.uint8)<br>
opening=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)<br>
closing=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)<br>
erosion=cv2.erode(img,kernel,iterations=1)<br>
dilation=cv2.dilate(img,kernel,iterations=1)<br>
gradient=cv2.morphologyEx(img,cv2.MORPH_GRADIENT,kernel)<br>
plt.subplot(151)<br>
plt.imshow(opening)<br>
plt.subplot(152)<br>
plt.imshow(closing)<br>
plt.subplot(153)<br>
plt.imshow(erosion)<br>
plt.subplot(154)<br>
plt.imshow(dilation)<br>
plt.subplot(154)<br>
plt.imshow(gradient)<br>
cv2.waitKey(0)<br>

<br>
OUTPUT:<br>

![image](https://user-images.githubusercontent.com/98301023/176420696-b86ccca1-6577-4028-8d5b-f855fa534663.png)<br>
-----------------------------------------------------------------------------------------------------------------------------------------------------------------<br>
19.Develop a program to <br>
i)Read the Image<br>
ii)Write the gray scale image<br>
iii)Display the original image and grayscale image<br>
#13/07/2022<br>
import cv2<br>
originalimg=cv2.imread('dog1.jpg')<br>
grayimg=cv2.imread('dog1.jpg',0)<br>
issaved=cv2.imwrite('d:/dog1.jpg',grayimg)<br>
cv2.imshow('display original image',originalimg)<br>
cv2.imshow('display grayscale image',grayimg)<br>
cv2.waitKey(0);<br>
cv2.destroyAllWindows()<br>
if issaved:<br>
    print('the image is successfully saved')<br>
<br>
OUTPUT:<br>
the image is successfully saved<br>
![image](https://user-images.githubusercontent.com/98301023/178705388-b15098a7-ef37-4387-a853-98ad8bbdea2f.png)<br>

![image](https://user-images.githubusercontent.com/98301023/178705554-12766fde-5d5e-4e00-aed1-50a724be2d0a.png)<br>
-------------------------------------------------------------------------------------------------------------------------------------------------------<br>

<br>

20.)program to perform slicing with background<br>
import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
image=cv2.imread('dog2.jpg',0)<br>
x,y=image.shape<br>
z=np.zeros((x,y))<br>
for i in range(0,x):<br>
    for j in range(0,y):<br>
        if(image[i][j]>50 and image[i][j]<150):<br>
            z[i][j]=255      <br> 
        else:<br>
            z[i][j]=image[i][j]<br>
equ=np.hstack((image,z))<br>
plt.title('graylevel slicing with background')<br>
plt.imshow(equ,'gray')<br>
plt.show()<br>
        <br>
        
        
OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98301023/178706540-03dda4d6-c78f-4149-921a-88abfaad531f.png)<br>

  ----------------------------------------------------------------------------------------------------------------------------------------------------<br>      

21.program to perform slicing without background<br>
import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
image=cv2.imread('dog2.jpg',0)<br>
x,y=image.shape<br>
z=np.zeros((x,y))<br>
for i in range(0,x):<br>
    for j in range(0,y):<br>
        if(image[i][j]>50 and image[i][j]<150):<br>
            z[i][j]=255      <br> 
        else:<br>
            z[i][j]=0<br>
equ=np.hstack((image,z))<br>
plt.title('graylevel slicing with background')<br>
plt.imshow(equ,'gray')<br>
plt.show()<br>
        <br>
        OUTPUT:
        <br>
        ![image](https://user-images.githubusercontent.com/98301023/178709200-c4622c07-9179-4014-af29-67083bf3ba37.png)<br>

      
------------------------------------------------------------------------------------------------------------------------------------------------------------------<br>
        
#13-07-2022<br>
22.IMAGE USING HISTOGRAM<br>

using gray image<br>

import cv2<br>
import matplotlib.pyplot as plt<br>
img = cv2.imread('viratkohli.jpg',0)<br>
hist = cv2.calcHist([img],[0], None, [256], [0, 256])<br>
cv2.imshow("Original image", img)<br>
plt.plot(hist)<br>
plt.xlim([0, 256])<br>
plt.ylim([0, max(hist)+1])<br>
plt.show()<br>
cv2.waitKey(0)<br><br><br>
cv2.destroyAllWindows()<br>

OUTPUT<br>
![image](https://user-images.githubusercontent.com/98301023/178964863-6336f720-7be2-48bb-bc29-00b5b2d71a73.png)<br>
<br>
![image](https://user-images.githubusercontent.com/98301023/178965063-8b1ef275-f5a0-4d04-a7ce-73e626b1cd77.png)<br>


---------------------------------------------------------------------------------------------------------------------------------------------------<br?


import cv2<br><br>
import matplotlib.pyplot as plt<br><br>
img = cv2.imread("viratkohli.jpg")<br><br>
color = ('b','g','r')<br><br>
cv2.imshow("Original image", img)<br><br>
for i,col in enumerate(color):<br><br>
    hist = cv2.calcHist([img],[i], None, [256], [0, 256])<br><br>
    plt.plot(hist, color=col)<br><br>
plt.show()<br><br>
cv2.waitKey(0)<br><br>
cv2.destroyAllWindows()<br><br>

OUTPUT<br><br>
![image](https://user-images.githubusercontent.com/98301023/178970782-b38a4d86-db6b-449e-b3ab-d4c3cba068d2.png)<br>


![image](https://user-images.githubusercontent.com/98301023/178971022-72fa0e5a-4460-4c56-86c7-dd97647d1d33.png)<br>

---------------------------------------------------------------------------------------------------------------------------------------------<br>


#histogram equilyzer<br>
import cv2<br><br>
import matplotlib.pyplot as plt<br>
img = cv2.imread("viratkohli.jpg",0)<br>
equalized_img = cv2.equalizeHist(img)<br>
hist = cv2.calcHist([img],[0], None, [256], [0, 256])<br>
equalized_hist = cv2.calcHist([equalized_img],[0], None, [256], [0, 256])<br>
fig, ax = plt.subplots(2, 2, figsize=(9,7))<br>
ax[0, 0].plot(hist)<br>
ax[0,0].set_title("Histogram of the original image")<br>
ax[0, 1].plot(equalized_hist)<br>
ax[0,1].set_title("Equalized histogram")<br>
ax[1, 0].imshow(img, cmap="gray")<br>
ax[1, 0].set_title("Original image")<br>
ax[1, 1].imshow(equalized_img, cmap="gray")<br>
ax[1,1].set_title("Histogram equalized image")<br>
plt.show()<br>

OUTPUT<br>

![image](https://user-images.githubusercontent.com/98301023/178971324-02c2e4d7-105e-4e02-98bd-ad898a542115.png)<br>
-----------------------------------------------------------------------------------------------------------------------<br>
23.program to perform basic image data analysis using intensity transformation<br>
a]Imge negetive<br>
b]log transformation<br>
c]Gamma correction<br>

%matplotlib Inline<br>
import imageio<br>
import matplotlib.pyplot as plt<br>
import warnings<br>
import matplotlib.cbook<br>
warnings.filterwarnings("ignore",category=matplotlib.cbook.mplDeprecation)<br>
pic=imageio.imread('butterfly3.jpg')<br>
plt.figure(figsize=(6,6))<br>
plt.imshow(pic);<br>
plt.axis('off');<br>

#output
![image](https://user-images.githubusercontent.com/98301023/180028959-f6ce3548-634f-4b5d-adf2-af5adee40f05.png)<br>



#image negative<br>
negative=255-pic #neg=(L-1)-img<br>
plt.figure(figsize=(6,6))<br>
plt.imshow(negative);<br>
plt.axis('off');<br>

OUTPUT<br>
![image](https://user-images.githubusercontent.com/98301023/180035594-74ae8945-c205-41c2-b1bc-da78df9062b0.png)<br>


#Log Transformation<br>
%matplotlib inline<br>

import imageio<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>

pic=imageio.imread('butterfly3.jpg')<br>
gray=lambda rgb : np.dot(rgb[...,:3],[0.299,0.587,0.114])<br>
gray=gray(pic)<br>

max_=np.max(gray)<br>

def log_transform():<br>
    return(255/np.log(1+max_))*np.log(1+gray)<br>
plt.figure(figsize=(5,5))<br>
plt.imshow(log_transform(),cmap=plt.get_cmap(name='gray'))<br>
plt.axis('off')<br>

OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98301023/180034483-7d656077-2048-49fe-a93c-e88d63ff3aa7.png)<br>


#Gamma correction<br>
import imageio<br>
import matplotlib.pyplot as plt<br>

#Gamma encoding<br>
pic=imageio.imread('butterfly3.jpg')<br>
gamma=2.2 #Gamma<1 ~dark: Gamma>1 ~Bright<br>

gamma_correction=((pic/255)**(1/gamma))<br>
plt.figure(figsize=(5,5))<br>
plt.imshow(gamma_correction)<br>
plt.axis('off');<br>


OUTPUT:
![image](https://user-images.githubusercontent.com/98301023/180034818-958bfe51-8251-42f9-8dcc-c5e7a0070559.png)<br>
_________________________________________________________________________________________________________________________

24.program to perform basic image manipulation<br>
a]sharness<br>
b]flipping<br>
c]cropping<br>

#Image sharpen<br>
from PIL import Image<br>
from PIL import ImageFilter<br>
import matplotlib.pyplot as plt <br>

#load the image<br>
my_image=Image.open('myimage.jpg')<br>

#use sharpen function<br>
sharp=my_image.filter(ImageFilter.SHARPEN)<br>

#save the image<br>
sharp.save('D:/image_sharpen.jpg')<br>
sharp.show()<br>
plt.imshow(sharp)<br>
plt.show()<br>

OUTPUT:<br>
![image](https://user-images.githubusercontent.com/98301023/180037807-ace5276e-881c-4531-b659-5ec3a8aeab02.png)<br>


#Image flip<br>
import matplotlib.pyplot as plt<br>
#load the image<br>
img=Image.open('myimage.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
#use the flip function<br>
flip=img.transpose(Image.FLIP_LEFT_RIGHT)<br>

#save the image<br>
flip.save('D:/image_flip.jpg')<br>
plt.imshow(flip)<br>
plt.show()<br>

output:
![image](https://user-images.githubusercontent.com/98301023/180037954-04cfe713-e4cb-409d-a9b0-b50bc8473f76.png)<br>


![image](https://user-images.githubusercontent.com/98301023/180038142-58451710-f259-4271-b432-131df35d9819.png)<br>


#Importing Image class from pil module<br>
from PIL import Image <br>
import matplotlib.pyplot as plt<br>

#opens a image in  RGB mode<br>
im=Image.open('myimage.jpg')<br>
plt.imshow(im)<br>

#size the image in pixels(size of original image)<br>
#(this is not mandatory)<br>
widtg,height=im.size<br>

#cropped image of above dimension<br>
#(it will not change the original image)<br>
im1=im.crop((100,20,200,140))<br>

#show the image in image viewer<br>
#im1.show()<br>
plt.imshow(im1)<br>
plt.show()<br>



output:<br>

![image](https://user-images.githubusercontent.com/98301023/180038247-b53beb54-e645-4a56-9212-a25d49edffb0.png)<br>
________________________________________________________________________________________________________________________<br>

# 25.generate matrixx and display the image data<br>
import matplotlib.image as image<br>
img=image.imread('teddy.jpg')<br>
print('The Shape of the image is:',img.shape)<br>
print('The image as array is:')<br>
print(img)

__OUTPUT___<br>
The Shape of the image is: (1333, 1000, 3)<br>
The image as array is:<br>
[[[243 179  79]<br>
  [243 179  79]<br>
  [243 179  79]<br>
  ...<br>
  [229 160  65]<br>
  [229 160  65]<br>
  [229 160  65]]<br>

 [[243 179  79]<br>
  [243 179  79]<br>
  [243 179  79]<br>
  ...
  [229 160  65]<br>
  [229 160  65]<br>
  [229 160  65]]<br>

 [[243 179  79]<br>
  [243 179  79]<br>
  [243 179  79]<br>
  ...<br>
  [229 160  65]<br>
  [229 160  65]<br>
  [229 160  65]]<br>

 ...<br>

 [[183 126  45]<br>
  [182 125  44]<br>
  [181 124  43]<br>
  ...<br>
  [183 124  44]<br>
  [183 124  44]<br>
  [183 124  44]]<br>

 [[181 126  46]<br>
  [181 126  46]<br>
  [180 125  45]<br>
  ...
  [182 125  46]<br>
  [182 125  46]<br>
  [182 125  46]]<br>

 [[179 126  50]<br>
  [179 126  50]<br>
  [178 125  49]<br>
  ...
  [179 126  50]<br>
  [179 126  50]<br>
  [179 126  50]]]<br>
  # _____________________________________________________________________________________________________________________

# 26.programt to find the brightness of a Image from distance to centre<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
arr = np.zeros((256,256,3), dtype=np.uint8)<br>
imgsize = arr.shape[:2]<br>
innerColor = (255, 255, 255)<br>
outerColor = (0,0,0)<br>
for y in range(imgsize[1]):<br>
 for x in range(imgsize[0]):<br>
    distanceToCenter = np.sqrt((x - imgsize[0]//2) ** 2 + (y - imgsize[1]//2) ** 2)<br>
distanceToCenter = distanceToCenter / (np.sqrt(2) * imgsize[0]/2)<br>
r = outerColor[0] * distanceToCenter + innerColor[0] * (1 - distanceToCenter)<br>
g = outerColor[1] * distanceToCenter + innerColor[1] * (1 - distanceToCenter)<br>
b = outerColor[2] * distanceToCenter + innerColor[2] * (1 - distanceToCenter)<br>
arr[y, x] = (int(r), int(g), int(b))<br>
plt.imshow(arr, cmap='gray')<br>
plt.show()<br>

# OUTPUT<br>

# ________________________________________________________________________________________________________________

# 27.# example of pixel normalization<br>

from numpy import asarray<br>
from PIL import Image<br>
# load image<br>

image = Image.open('bird.jpg')<br>
pixels = asarray(image)<br>
# confirm pixel range is 0-255<br>

#print('Data Type: %s' % pixels.dtype)<br>
print('Min: %.3f, Max: %.3f' % (pixels.min(), pixels.max()))<br>
# convert from integers to floats<br>

pixels = pixels.astype('float32')<br>
# normalize to the range 0-1<br>

pixels /= 255.0<br>
# confirm the normalization<br>

print('Min: %.3f, Max: %.3f' % (pixels.min(), pixels.max())<br>


# aVerage<br>
import cv2<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread("bird.jpg",0)<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
np.average(img)<br>

![image](https://user-images.githubusercontent.com/98301023/186457327-f6a73d13-1564-410f-b1ec-00b673d26d9d.png)<br>

# Standard deviation<br>
from PIL import Image,ImageStat<br>
import matplotlib.pyplot as plt<br>
im=Image.open('bird.jpg')<br>
plt.imshow(im)<br>
plt.show()<br>
stat=ImageStat.Stat(im)<br>
print(stat.stddev)<br>

![image](https://user-images.githubusercontent.com/98301023/186457501-e732cddf-313c-43a8-a3b5-e776f642553d.png)<br>

 # Max<br>
import cv2<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('bird.jpg' )<br>
plt.imshow(img)<br>
plt.show()<br>
max_channels = np.amax([np.amax(img[:,:,0]), np.amax(img[:,:,1]),np.amax(img[:,:,2])])<br>
print(max_channels)<br>

![image](https://user-images.githubusercontent.com/98301023/186457829-096ca043-cc1d-43d2-b332-78ecc7326ef9.png)<br>

![image](https://user-images.githubusercontent.com/98301023/186457949-c72a00bd-e35f-49ff-85ad-cce32960b266.png)<br>


# Min<br>
import cv2<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('bird.jpg' )<br>
plt.imshow(img)<br>
plt.show()<br>
min_channels = np.amin([np.min(img[:,:,0]), np.amin(img[:,:,1]),np.amin(img[:,:,2])])<br>
print(min_channels)<br>


![image](https://user-images.githubusercontent.com/98301023/186458541-df391103-80ff-4ca1-9d95-3b0f872b9e90.png)<br>

# _____________________________________________________________________________________________________________________
# 32.Sobel edge and canny edge detection<br>
import cv2<br>
# Read the original image<br>

img = cv2.imread('lio1.jpg')<br>
# Display original image<br>

cv2.imshow('Original', img)<br>
cv2.waitKey(0)<br>
# Convert to graycsale<br>

img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)<br>
#Blur the image for better edge detection<br>

img_blur = cv2.GaussianBlur(img_gray, (3,3), 0)<br>
# Sobel Edge Detection<br>

sobelx = cv2.Sobel(src=img_blur, ddepth=cv2.CV_64F, dx=1, dy=0, ksize=5) # Sobel Edge Detection on the X axis<br>
sobely = cv2.Sobel(src=img_blur, ddepth=cv2.CV_64F, dx=0, dy=1, ksize=5) # Sobel Edge Detection on the Y axis<br>
sobelxy = cv2.Sobel(src=img_blur, ddepth=cv2.CV_64F, dx=1, dy=1, ksize=5) # Combined X and Y Sobel Edge Detection<br>
# Display Sobel Edge Detection Images<br>

cv2.imshow('Sobel X', sobelx)<br>
cv2.waitKey(0)<br>
cv2.imshow('Sobel Y', sobely)<br>
cv2.waitKey(0)<br>
cv2.imshow('Sobel X Y using Sobel() function', sobelxy)<br>
cv2.waitKey(0)<br>
# Canny Edge Detection<br>

edges = cv2.Canny(image=img_blur, threshold1=100, threshold2=200) # Canny Edge Detection<br>
# Display Canny Edge Detection Image<br>

cv2.imshow('Canny Edge Detection', edges)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

__ OUTPUT__<br>
![image](https://user-images.githubusercontent.com/98301023/186462220-0b2ce596-37a3-44b4-ae82-4d7cb9d0c614.png)<br>

![image](https://user-images.githubusercontent.com/98301023/186462355-aff34292-afc4-477a-9a42-b63317e4491f.png)<br>

![image](https://user-images.githubusercontent.com/98301023/186462495-4847768c-0978-45d3-97ad-fabfb4e15785.png)<br>


![image](https://user-images.githubusercontent.com/98301023/187943058-9f03f838-6d07-4801-ac49-39f0accd68f4.png)


![image](https://user-images.githubusercontent.com/98301023/187943241-4de3df8f-4655-4eb0-a954-780b04f02b14.png)

_________________________________________________________________________________________________________________________<br>


# 33. image processing
# 1.Image restoration:

# (a)Restore a damaged image

import numpy as np
import cv2
import matplotlib.pyplot as plt
# open the image
img=cv2.imread('dimage_damaged.png')
plt.imshow(img)
plt.show()

# load the mask
mask=cv2.imread('dimage_mask.png',0)
plt.imshow(mask)
plt.show()

# inpaint.
dst=cv2.inpaint(img,mask,3,cv2.INPAINT_TELEA)

# write the output
cv2.imwrite('dimage_inpainted.png',dst)
plt.imshow(dst)
plt.show()


# output
![image](https://user-images.githubusercontent.com/98301023/187944659-d573d661-82d0-4ccc-ae7a-00e067d403c5.png)


![image](https://user-images.githubusercontent.com/98301023/187945431-e9fb5235-bd7b-4a38-8a7d-13220789b4a3.png)

![image](https://user-images.githubusercontent.com/98301023/187945482-c54b69dd-b2a2-4358-b504-16abf5bb1a5a.png)


# (b) REmoving Logo's

import numpy as np
import matplotlib as plt
import pandas as pd
import matplotlib.pyplot as plt
plt.rcParams['figure.figsize']=(10, 8)

def show_image(image,tittle='Image',cmap_type='gray'):
    plt.imshow(image,cmap=cmap_type)
    plt.title(title)
    plt.axis('off')
 
def plot_comparison(img_original,img_filtered,img_title_filterd):
    fig,(ax1,ax2)=plt.subplots(ncols=2,figsize=(10,8),sharex=True,sharey=True)
    ax1.imshow(img_original,cmap=plt.cm.gray)
    ax1.set_title('original')
    ax1.axis('off')
    ax2.imshow(img_filtered,cmap=plt.cm.gray)
    ax2.set_title(img_title_filterd)
    ax2.axis('off')
    
    
    
  from skimage.restoration import inpaint
from skimage.transform import resize
from skimage import color


image_with_logo=plt.imread('imlogo.png')

# initialize the mask
mask=np.zeros(image_with_logo.shape[:-1])

# set the pixels where the logo is to 1
mask[210:272,360:425]=1

# apply inpainting to remove the logo
image_logo_removed=inpaint.inpaint_biharmonic(image_with_logo,
                                              mask,multichannel=True)

# show the image and logo removed images
plot_comparison(image_with_logo,image_logo_removed, 'image with logo removed')

          
![image](https://user-images.githubusercontent.com/98301023/187946061-5ee3f246-e39a-4809-90ec-ca8702d661b7.png)

# (2) Noise:
# (a) adding noise
from skimage.util import random_noise

fruit_image=plt.imread('fruitts.jpeg')


# add noise to the image
noisy_image=random_noise(fruit_image)

# show the original and resulting image
plot_comparison(fruit_image,noisy_image,'noisy image')


![image](https://user-images.githubusercontent.com/98301023/187946297-4c42fcdf-966e-4658-91c2-c9e6beb4e45a.png)


# (b) Reducing noise
from skimage.restoration import denoise_tv_chambolle

noisy_image=plt.imread('noisy.jpg')

# Apply total variation filter dnoising
denoised_image=denoise_tv_chambolle(noisy_image,multichannel=True)

# show the noisy and denoised image
plot_comparison(noisy_image,denoised_image,'denoised image')


![image](https://user-images.githubusercontent.com/98301023/187946606-0849defc-9b63-4104-901a-1a349d3b42fc.png)

# (c) Reducing Noise while preserving edges

from skimage.restoration import denoise_bilateral
landscape_image=plt.imread('noisy.jpg')

# Apply bilateral filter denoising

denoised_image=denoise_bilateral(landscape_image,multichannel=True)

# show original and resulting image
plot_comparison(landscape_image,denoised_image,'denoised Image')


![image](https://user-images.githubusercontent.com/98301023/187946989-4eab0673-2c58-4c64-a746-30527ca3deee.png)


# (3) Segmentation
# (a) Superpixel Segmentation

from skimage.segmentation import slic
from skimage.color import label2rgb

face_image=plt.imread('face.jpg')

# obtain the segmentation with 400 regions
segment=slic(face_image,n_segments=400)

# put segment on top of original image to compare
segmented_image=label2rgb(segment,face_image,kind='avg')

# show the segmented image
plot_comparison(face_image,segmented_image,'segmentd image,400 superpixels')

![image](https://user-images.githubusercontent.com/98301023/187947198-cbc1d248-5454-4377-b0da-5c8c1465a9e3.png)


# (4) Counters:
 #   (a) counting shapes
    
def show_image_contour(image,counters):
    plt.figure()
    for n,contour in enumerate(contours):
        plt.plot(contour[:, 1],contour[:, 0],linewidth=3)
    plt.imshow(image,interpolation='nearest',cmap='gray_r')    
    plt.title('contours')
    plt.axis('off')
    
    
from skimage import measure,data

# obtain the horse image
horse_image=data.horse()

# find the contour with a constant level value of 0.8
contours=measure.find_contours(horse_image,level=0.8)

# show the image with contour found
show_image_contour(horse_image,contours)

![image](https://user-images.githubusercontent.com/98301023/187947492-ad8c29eb-6e5e-4532-86f8-0db42b1fa75d.png)


# (b) Find the contours of an image that is not binary
from skimage.io import imread
from skimage.filters import threshold_otsu
image_dices=imread('diceimg.jpg')

# make the image gray scale
image_dices= color.rgb2gray(image_dices)

#obtain the optimal thresh value
thresh=threshold_otsu(image_dices)

# Apply thresholding
binary=image_dices> thresh

# find contours at a constant value of 0.8
contours=measure.find_contours(binary,level=0.8)

# show the image
show_image_contour(image_dices,contours)

# (b) Find the contours of an image that is not binary
from skimage.io import imread
from skimage.filters import threshold_otsu
image_dices=imread('diceimg.jpg')

# make the image gray scale
image_dices= color.rgb2gray(image_dices)

# obtain the optimal thresh value
thresh=threshold_otsu(image_dices)

# Apply thresholding
binary=image_dices> thresh

# find contours at a constant value of 0.8
contours=measure.find_contours(binary,level=0.8)

#  show the image
show_image_contour(image_dices,contours)

![image](https://user-images.githubusercontent.com/98301023/187947649-6f1c2a06-093e-4d79-9c16-5ea646b835d3.png)


#(c) create list with the shape of each contour
shape_contours=[cnt.shape[0] for cnt in contours]


# set as the maximum size of the dots shape
max_dots_shape=50

# count dots in contours excluding bigger than dots size
dots_contours=[cnt for cnt in contours if np.shape(cnt)[0]<max_dots_shape]

# shows all contours found
show_image_contour(binary,contours)

# print the dice's number
print('dices dots number:{}'.format(len(dots_contours)))

![image](https://user-images.githubusercontent.com/98301023/187947824-0cd061cc-50e6-4f6a-85c8-3be278315ec0.png)
