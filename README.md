# PolaroidGenerator
Convert any picture into a polaroid format that can be printed from any 4 by 6 photo printer

The polaroid_resize.py file is the script needed to convert any picture into a polaroid ready format. You can run it however you run Python 2.7 files. 

If you have never run a Python file before, please see the following links:
- Windows: http://stackoverflow.com/questions/1522564/how-do-i-run-a-python-program
- Mac: http://stackoverflow.com/questions/21492214/how-to-run-python-script-on-terminal

The motive behind this script is to allow one to cheaply print any photograph in polaroid dimensions. Currently, using online services cost around $2-$8 to convert a picture into a polaroid photo. 

This script converts a picture into polaroid dimensions and overlays it on a 4 by 6 background which costs 10 cents to print. It also draws lines on the picture where you have to cut to obtain the final photograph.

Before you run the script you need the following installed:
1. Numpy
2. OpenCV 2.4.13
3. Python 2.7

In the script:
1. You have to specify the input file name and the output file name as specified. Place the script in the same directory as the input file
2. The script converts Portrait, Landscape and Square photographs using different dimensions that are commonly used in popular polaroid models:
  - Portrait: FUJI FP-100 Silk Film (http://www.fujifilm.com/products/instant_photo/pdf/fp_100c_datasheet.pdf)
  - Landscape: Instax Wide Film (http://www.fujifilm.com/products/instant_photo/films/instax/)
  - Square: Polaroid SX-70 Film (https://www.bhphotovideo.com/c/product/1042372-REG/impossible_prd3105_instant_color_film_for.html)
3. The script will only convert input photos with the following aspect ratios (image height:image width)
  - Portrait: 1.26 - 1.34
  - Landscape: 0.745 - 0.754
  - Square: 0.99-1.01

After running the script:
1. You can print the final file at any photo printer using the 4x6 format
2. The lines on the photograph indicate where to cut the final photo to obtain the Polaroid photograph

Version 2 will contain:
1. Polaroid filtering to make photos look vintage
2. Support for images with varying aspect ratios
