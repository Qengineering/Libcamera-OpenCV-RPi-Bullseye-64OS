# Libcamera OpenCV RPi Bullseye 64OS
![output image]( https://qengineering.eu/images/CameraWall.webp )<br/>
## Libcamera + OpenCV on a Raspberry Pi 4 with 64-bit Bullseye OS
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>
In the new Debian 11, Bullseye, you can only capture live video with a streaming framework, like GStreamer or FFmpeg. This is an example of libcamera working on a Raspberry Pi with an 64-bits OS.<br/>

------------

## Dependencies.<br/>
To run the application, you have to:
- A Raspberry Pi 4. 
- GStreamer 1.18.4 installed. [Install GStreamer](https://qengineering.eu/install-gstreamer-1.18-on-raspberry-pi-4.html) <br/>
- OpenCV 64 bit installed. [Install OpenCV 4.5](https://qengineering.eu/install-opencv-4.5-on-raspberry-64-os.html) <br/>
- Code::Blocks installed. (```$ sudo apt-get install codeblocks```)
- A working Raspicam

------------

## Installing the app.
To extract and run the app in Code::Blocks <br/>
$ mkdir *MyDir* <br/>
$ cd *MyDir* <br/>
$ wget https://github.com/Qengineering/Libcamera-OpenCV-RPi-Bullseye-64OS/archive/refs/heads/main.zip <br/>
$ unzip -j master.zip <br/>
Remove master.zip, LICENSE and README.md as they are no longer needed. <br/> 
$ rm master.zip <br/>
$ rm LICENSE <br/>
$ rm README.md <br/> <br/>
Your *MyDir* folder must now look like this: <br/> 
GStreamer_RPi_64_Bullseye.cpb <br/>
main.cpp <br/>

------------

## Running the app.
To run the application load the project file GStreamer_RPi_64_Bullseye.cbp in Code::Blocks.<br/> 
Next, follow the instructions at [Hands-On](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html#HandsOn).<br/>
On this [page](https://qengineering.eu/install-gstreamer-1.18-on-raspberry-pi-4.html) you can see how to make the **webcam** work.

------------

## Frame rate.
The Raspicam supports many sizes and frame rates, as you can see [here](https://www.raspberrypi.org/documentation/raspbian/applications/camera.md).<br/>
You can switch between the different options by altering the parameters in the pipeline.<br/>
As long it's a valid combination, it will work. For instance:<br/>
```
    //pipeline parameters
    int capture_width = 640 ;
    int capture_height = 480 ;
    int display_width = 640 ;
    int display_height = 480 ;
    int framerate = 90 ;
```

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 

