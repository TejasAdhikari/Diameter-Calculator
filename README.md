# Diameter-Calculator

Image Processing Tool Box required

1. Import Image - The command imreadreads an image and converts it into a “3-dimensional” matrix in the RGB color space.
2. Segment the image into a binary image to differentiate the background  from  the  desired  objects.        
  i.  The  first  step  taken  is  to  divide  the  image  into  three images based on the intensities of each red, green and blue componentwithin the image. This is
      Color Based  Image Segmentation.  
  ii.  The  blue  plane  is  the  best choice  to  use  for  Image Thresholding ( converting into a binary image 1 (white) or 0 (black))  because  it  provides  the 
       most  contrast  between  the desired  object  (foreground)  and  the  background.         
  iii. There is quite a bit of “noise” and we need to clean the image up significantly to improve the accuracy of our diameter measurement. 
3. The "regionprops" function is  the  tool  that  will  providethe MajorAxisLengthof  the  blob  in  the image.        
4. As a result the diameter is displayed/.
