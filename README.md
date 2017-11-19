# slitscan
Python video slit scan generator based on OpenCV

Generates a color strip of a given image sequence and returns the result as image object.

Using OpenCV, this function creates a color slit scan from the given input
file. By default, the average color of 5 frames is condensed into one stripe
in the output image.

If you encounter errors, this is probably due to unsupported video formats.
Check if your Python OpenCV bindings are compiled using ffmpeg. If not,
you have to manually compile OpenCV with Python bindings including ffmpeg.
This is usually true for Linux and OS X because the PyPi installed OpenCV
bindings do not support ffmpeg for these plattforms. The Windows version
does support ffmpeg, but with the limitation of LGPL licensed code. If
in doubt, convert your video to uncrompressed AVI or comparable.

Testet with Python 3.6, should work back to 2.7, too. After installation, use the command line phrase "slitscan -h" to learn about the features.

## Installing
### Mac
If not already done: `brew install python3`

Then: `pip3 install git+https://github.com/0xLeon/slitscan.git`

### Other (e.g. Windows)

First search on Google about installing _python (3.6)_ and _pip_!

Then: `pip install git+https://github.com/0xLeon/slitscan.git`

## Using
    slitscan --help

### Usage & Arguments
    slitscan [-h] [--outfile OUTFILE] [--height HEIGHT] [--frame-aggr FRAME_AGGR] INFILE

### Optional argument definition

    -h, --help

show this help message and exit


    --outfile OUTFILE

Output file name relative to input file, can be specified absolute


    --height HEIGHT

Height of the output slit scan image


    --frame-aggr FRAME_AGGR

Number of frames to aggregate into one stipe

## Feel free to contribute!
This is a new script. If you know python, please make the script running more smooth and faster.
### Roadmap:
- parallelisation _for faster and smoother script running_
- progress
- summary
