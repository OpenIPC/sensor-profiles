![OpenIPC logo][logo]

## Collection of profiles for various sensors

### Introduction

Parameters relating to light handling, exposure, colors, contrast, noise reduction, sharpening, etc, etc are saved as sensor-profiles for OpenIPC cameras.

To load a profile, copy the .bin file to the camera /etc/sensors directory and change the entry in /etc/majestic.yaml to point to the newly copied file.


### IMX335

#### [imx335_ssc338q_20240628.bin](https://github.com/OpenIPC/sensor-profiles/raw/master/files/imx335_ssc338q_20240628.bin) 8fb07710f42ec8c364c3c684a627b710

New default sensor profile for FPV pilots
Choose this config if you fly freestyle FPV
(previously named greg12color5.bin)

- works indoors or outdoors, sunny, overcast, morning, noon, evening. Very dark will be very dark
- stays at 120fps (or your chosen frame-rate) rather than cut fps in lower light
- keeps ground visible when sky is bright
- less contrasty for better details in darker areas when flying
- noise reduction / sharpness tweaked for all conditions
- try to look beautiful all the time

Also works on imx415

For cleanest image, set max shutter (aka exposure in majestic.yaml) to 1 divided by fps (eg 1/120 = 8.333ms for 120fps)
 
by Greg Sparks



### IMX415

#### [imx415_ssc338q_20240613.bin](https://github.com/OpenIPC/sensor-profiles/raw/master/files/imx415_ssc338q_20240613.bin) d7174c3e0e2eb208b78650b65dad973f

Improved default imx415_fpv profile for FPV pilots
formally named imx415_fpv9.bin

For cleanest image, set max shutter (aka exposure in majestic.yaml) to 1 divided by fps (eg 1/120 = 8.333ms for 120fps)

by Greg Sparks




[logo]: https://openipc.org/assets/openipc-logo-black.svg
