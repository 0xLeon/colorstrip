# slitscan
### (fork from https://git.io/vF9pm)
Python video slit scan generator based on OpenCV

Testet with Python 3.6, should work back to 2.7, too. After installation, use the command line phrase "slitscan -h" to learn about the features.

## Installing
### Mac
If not already done: `brew install python3`

Then: `pip3 install git+https://github.com/samrdev/slitscan.git`

### Other (e.g. Windows)

First search on Google about installing _python (3.6)_ and _pip_!

Then: `pip install git+https://github.com/samrdev/slitscan.git`

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
