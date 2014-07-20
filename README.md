ArduinoOnBeagleBone
===================

Arduino and AVR compilation tools for BeagleBone (currently command-line only)

This will give you the command-line tools needed to compile AVR programs
and Arduino sketches.  In this way it is similar to WinAVR for Windows and 
CrossPack for Mac OS X.

Specifically, the versions of the tools created are:
- avr binutils-2.22
- avr gcc-4.5.3
- avr-libc-1.8.0 
- avrdude 5.11.1

![arduino on beaglebone](http://farm8.staticflickr.com/7133/7498727432_681c5955ba_n.jpg)

Update 19 Jul 2014: @schiavone has updated the process to work with modern Arduino, see: https://docs.google.com/document/d/1k3ltjBM7x6sSX8FyFmMQFxjCXu7EGPTC8_UaT0u0PGM/edit?usp=sharing


Quickstart
-----------

1. Get & install the tools tarball with:
```
    # cd /
    # wget http://cloud.github.com/downloads/todbot/ArduinoOnBeagleBone/avrtools-arduino-beaglebone-20120630.tar.gz
    # tar xvzf avrtools-arduino-beaglebone-20120630.tar.gz
    # . /usr/local/avr/arduino-setup
```

2. Go into your sketch directory and start compiling
```
    # cd ~/sketches/MyAwesomSketch
    # ln -s $AVRDIR/arduino.mk Makefile
    # make
    # make upload
    # make monitor
```

More Info
---------

For details on how to use this package, see:
  ["using-beaglebone-avr-arduino-tools.txt"](https://github.com/todbot/ArduinoOnBeagleBone/blob/master/using-beaglebone-avr-arduino-tools.txt)



For details on how these tools were compiled, see:
  ["building-beaglebone-avr-arduino-tools.txt"](https://github.com/todbot/ArduinoOnBeagleBone/blob/master/building-beaglebone-avr-arduino-tools.txt)



