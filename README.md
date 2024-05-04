# Image-Signal-Processing
This repository Contains a simple implementation of Image signal Processing techniques like Histogram equalization etc which is used in Computer Vision tasks heavily.

# Image Signal Processor (ISP)

### Background
* An ISP is a processing block that converts raw sensor images into a colour array. There is a surprising amount of image processing that occurs between image capture and output colour images.
* This Repoitory contains processes which is under-taken in a ISP processing block.

### The following processing will be done:
* Read in the image
* Demosaic (convert raw to RGB) : The demosaic process converts raw pixel data into RGB image data. Each raw sensor pixel contains only one colour. Part of the demosaic process is to use interpolation to generate the missing colours for each pixel (i.e. a red pixel will get green and blue pixel information from the neighbouring pixels. Link : https://docs.opencv.org/3.4/de/d25/imgproc_color_conversions.html .
* Apply Colour Correction Matrix : A colour correction matrix is applied to improve colour reproduction accuracy.
* Apply Gamma Correction.
* Apply Denoise (e.g. bilateral filter).
* Apply Edge Enhancement (e.g. unsharp mask).
* Apply Contrast Enhancement (e.g. CLAHE)
* Save result to an output file (e.g. imsave() function from matplotlib).
