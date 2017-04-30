# Introduction And Motivation
Hopefully some of you found this fork of the ECE385-HelperTools; thats because my modification of this set makes it easier to work on the things that matter.
 
All credit to github user Atrifex for writing the tools that do the heavy lifting; I really just cleaned up the folder system, made the script i wanted (png-to-palette-relative-resizer.py) work out of the box, and helped out the people that were looking for a tool to make arrays for easy loading. 

A tutorial on how to use the array based process might follow; it depends on interest! 

# How to Use these scripts

1.  Gather all the images that you plan on using in the sprite_originals folder
2.  Go to <http://www.piskelapp.com> and click on create a sprite
3.  Import an image and look at the bottom right corner of the screen. There you will see a list of colors that appear in your image.
4.  Make a list (record RGB values) of important colors that appear in the image.
     -   The more accuracy you want, the more colors you should include; try and gather ones that look visually unique! The script handles up to 47 colors. 
5.  Repeat steps 3 and 4 for each image.
6.  Take this list and place it within `palette_hex` as hex values in the format 0xRGB
    -   Example `palette_hex = ['0xFF0000' , '0x047cc0', '0x14b8eb', '0x42fdff', '0x37dcff']`
7. Open a terminal, cd over to your clone of this repo!  
8. Run the ImageToArray.py script for each image; the command will be something like "python3 ImageToArray.py" . Fill out the prompts as necessary (sprite name, height and width of the desired sprite)
9. If you look in the sprite_bytes folder, the sprites are now each their own array file; you can copy and paste these into your sv files as you need! 


# FAQ

1.  What is PIL and why is it missing?
    -   PIL is the Python Imaging Library and it is missing because you haven't downloaded it.
    -   I recommend downloading [Anaconda][AnacondaDownload].

[AnacondaDownload]: <https://www.continuum.io/downloads>

