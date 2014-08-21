# Raspberry Pi - No LED Camera

## What is it?

This project represents a simple Python script that will take pictures
using a Raspberry PI camera module. The main difference between this 
script and the `raspistill` command is that it will turn the red LED
off before taking pictures. 

The main purpose of this project is to assist with gathering image
samples for my Machine Learning Deer Detector project (you can read
more about it [here](http://craigthomas.ca/blog/2014/08/04/deer-detection-with-machine-learning-part-1/).

The project contains code to:

* Take a set number of pictures with the Raspberry Pi camera


## License

This project makes use of an MIT style license. Please see the file called 
LICENSE for more information. 


## Requirements

You will need a Raspberry Pi with a Pi Camera module installed. It is 
recommended that you install the latest version of [Raspbian](http://www.raspbian.org/) 
with the Pi Camera module enabled (do this using `sudo raspi-config`). 
Because the script requires direct access to the camera, you will
also need to run it as root with `sudo`.


## Running

### Command Line Help

There are several options available for the program. Running the script
with the `-h` option will display a helpful description of the options:

    python rpinoledcamera.py -h

### Taking Pictures

To take pictures of various objects, you can specify the number of pictures
to take as well as a time delay between successive pictures. For example,
to take 10 pictures:

    python rpinoledcamera.py -n 10

To take 10 pictures with a delay of 5 seconds between each:

    python rpinoledcamera.py -n 10 -d 5

Saving files to a different path:

    python rpinoledcamera.py -p /path/to/save/to

