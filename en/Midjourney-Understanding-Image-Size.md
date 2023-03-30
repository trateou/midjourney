#### There are lots of terms for how "big" an image is. Many use words like resolution, file size, pixel count, dots per inch, and high resolution interchangeably. Understanding what these words mean can help you get the results you want from Midjourney images.

This guide is a simplified, non-technical, easy-to-understand explanation of image size, dimensions, resolutions, and DPI.

___

## Image Size Basics

Examples will use this simple sailboat picture.  
![MJ_ImageSize_Boat](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImageSize_Boat.png)

### What is an image file?

Image files like .jpg, .png, or .gif are instructions for creating an image.  
Each image is a mosaic of small colored tiles (pixels) that form the picture.

![MJ_ImageSize_Resolution_Instructions](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImageSize_Resolution_Instructions.png)

_Think about image files as a set of instructions on how to arrange colored pixels to create an image._

### What is File Size?

The file size is directly related to the amount of information inside the file. In the boat picture, the file contains 10 rows and 10 columns, or 100 pieces of information. If each colored dot is one byte of information, the image file would be 100 bytes.  
If the file has a grid of 200 x 400 pieces of color information, it would be an 80,000-byte file (200\*400=80,000) or 80,000-byte/1000 = 80-kilobyte file.

### Image Dimensions

People generally don't talk about the file size of an image in kilobytes or megabytes. They talk about the dimensions (the number of columns and rows information) of the image. The boat.jpg example above is described as a 10x10 pixel image.  
1024x1024, 720p, 4K, are all shorthand ways of talking about the pixel dimensions of an image.  
  
There are no "high-resolution" image files when working on monitors, phones, TVs, or other screens. The only thing that matters is how much information you have (the image dimensions) vs. the size of the display.  
The boat.jpg image might be a great size on a vintage flip phone, fine on your tablet, and not enough on your brand-new monitor.

![MJ_ImageSize_Resolution_screenSize](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImageSize_Resolution_screenSize.png)

_The same image dimension is seen on multiple screens._

___

## DPI Dots Per Inch

Dots Per Inch, Pixels Per Inch, Dots Per Centimeter, and Points Per Inch all refer to generally the same concept. The amount of information in a given length. 300 "dots" per inch means there are 300 pieces of color information (pixels, printed CMYK dots, etc.) in each inch.  
DPI is NOT a measurement that is useful on screens. The dimensions of the file are what matters on screen. DPI is VERY important when printing. The general standard for a great-looking print is 300 dots of color in every inch. 300DPI is the point where the individual dots are so closely packed together you can't distinguish individual dots, and the picture looks smooth and crisp.

### So... What DPI is this file?

It depends! Knowing that your file only contains instructions on how to make an image, the DPI is only determined when you tell the printer how closely or loosely that information is packed together.  
Think about building the file with Legos. You can take the same set of instructions, and if you have a pile of small 1x1 bricks, you pack your information into a smaller space than if you start with a pile of 2x2 bricks.

![MJ_ImageSize_Resolution_TileSize](https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/MJ_ImageSize_Resolution_TileSize.png)

_The same "file instructions" using two sizes of tiles._

### A Simplified Example of the Math

For this example, you have a 1200x1200 pixel image. What DPI is that image? It depends on how large you want it to print out.  
1200/300 = 4. A 1200x1200 pixel image would produce a great looking 4in x 4in image.  
1200/150 = 8. A 1200x1200 pixel image would produce an OK-looking 8in x 8in image.  
1200/100 = 12. A 1200x1200 pixel image would produce a pretty bad looking 12in x 12in image.

___

## Midjourney Image Sizes

The default size of the initial 2x2 grid is 512 x 512 pixels.  
The default upscale size is 1024 x 1024 pixels.

[Read More about image sizes and upscalers](https://docs.midjourney.com/docs/upscalers)

Was this article helpful?