# SVG2PNG #

This is a small project that converts a PNG file into an SVG image. For each pixel in the PNG we generate 
a square in the SVG canvas colored with the same color of the pixel and a border with a color which 
is slighly lighter. At the bottom of the image a palette is also created to show all the different colors 
used in the bitmap. It is designed to take a small bitmap and generate a large SVG representation of it.

To see what it does look here: https://github.com/cesarmiquel/PNG2SGV/wiki/PNG2SVG

## About the script ##

The script is short and written in PHP. It takes a single argument which must be a PNG file and outputs
to standard out an SVG image. If I want to convert the file mario.png to SVG all I need to do is:

    $ php png2svg.php mario.png > mario.svg

You can open the resulting image with Inkscape. The sample output looks like this:

![Sample output](https://a248.e.akamai.net/assets.github.com/img/276ca7d5eb24a474a0e89b929be7c1fcfe5eb82f/687474703a2f2f6934302e74696e797069632e636f6d2f313431316737372e706e67 "Sample output")

The only requirement is that PHP must be compiled with GD support.