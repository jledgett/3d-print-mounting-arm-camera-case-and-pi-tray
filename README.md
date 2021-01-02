# 3D Printer: Mounting Arm and Case for Raspberry Pi HQ Camera and Raspberry Pi / OctoPi

## Overview

This collection of files will allow you to print a 3D print a modification to your 3D printer.  This modification adds a mounting arm, case for the Raspberry Pi HQ Camera, as well as a covered tray for a Raspberry Pi 4B.  This is particularly useful for adding a camera to your printer for monitoring and control using OctoPrint / OctoPi.

This system was designed to work with the Creality CR-6 SE printer, but should work with __any__ printer or CNC that uses a 40mm x 40mm extruded aluminum frame (including Ender 3, Ender 3 Pro, CR-10 MAX) .

The Raspberry Pi case for your OctoPi server is designed to allow either direct mounting of the Raspberry Pi to the case using standoffs or dropping in the popular aluminum Flirc case for better heat dissipation.   

The case also supports mounting a **5v** 40mm fan.   Noctua fans are suggested due to their quiet operation and lengthy warranty.   They also included the 3-pin to 2-pin adapter which will allow you connect it directly to pins 4 and 6 of your Raspberry Pi's GPIO.

If you are using the Flirc case, the camera cable and fan cable can both be passed through the GPIO slot on the bottom of the Flirc case.   Remove the cosmetic black plastic TOP panel to increase cooling performance.

## Getting Started

You will need the following non-included parts:
- [Raspberry Pi 4B](https://smile.amazon.com/gp/product/B08DJ9MLHV/)
- [Raspberry Pi HQ Camera](https://www.canakit.com/raspberry-pi-hq-camera.html)
- [SD Card](https://smile.amazon.com/gp/product/B07FCMKK5X)
- [6mm CS-mount Lens](https://smile.amazon.com/gp/product/B088GWZPL1)
- [Flex Cable for Raspberry Pi Camera or Display - 18" / 457mm](https://www.adafruit.com/product/1730)
- [Mini Ball Head](https://smile.amazon.com/gp/product/B01N7RYA87) NOTE: Alternatively, you can mount directly to the mounting arm but will lose the ability to adjust the pitch of the camera up and down.
- [Noctua 40mm 5V Fan (3-pin)](https://smile.amazon.com/gp/product/B00NEMGCIA) (includes 3-pin to 2-pin adapter)
- *Screws, Nuts, Bolts*
  - (2x) 1/4"-20 x 1/2" bolts
  - (1x) 1/4"-20 jam nut
  - (4x) M4 x 40mm machine screws
  - (4x) M4 nuts
  - (6x) M4 washers
  - (4x) M2.5 x 30mm (or M2.5 x 35mm) 
  - (8x) M2.5 nuts
  - (8x) M2.5 washers
  - (4x) M2.5 nylon/rubber isolating washers
- [Flirc Raspberry Pi 4 Case](https://www.amazon.com/Flirc-Raspberry-Pi-Case-Silver/dp/B07WG4DW52/) _**OR**_
   - (4x) M2.5 x 10mm stand offs with matching screws
   - (4x) M2.5 nuts
   - (4x) M2.5 nylon/rubber isolating washers


You will need the following additional tools:
- Screwdriver for M2.5 screws
- Screwdriver for M4 screws
- Needle-nose pliers
- 1/4"-20 tap and die set for cleaning up threads of leveling feet


## Printing Instructions

:warning: **IMPORTANT:** Please review each part in your slicing software before printing to ensure a logical face is touching the build plate!      

These print settings were used to print using a Creality CR-6 SE using Hatchbox Black 1.75mm PLA.   You may need to adjust these settings slightly for other printer and filament combinations.

- Print Resolution: 0.2
- Infill (unless otherwise noted below): 40%
- Supports (unless otherwise noted below): No
- Printing Temperature: 200C
- Build Plate Temperature: 60C
- Part-specific notes:
   - **Short Leveling Foot 1g - Print 5.stl**: Print 5 of these at 100% infill.
   - **Long Leveling Foot 1g - Print 2.stl**: Print 2 of these at 100% infill.
   - **Tripod Thread Mount 34g.stl**: This piece is optional.   Print it if you want to mount accessories such as an LED light.   For this piece you will need to print a "Touching Buildplate" support for overhanging angles exceeding 47°.  This is the only piece that needs to be printed with supports.
  - **OPTIONAL Octopi Tray Spring Clip For FLIRC Case 4g.stl**: This is only needed if you are dropping in a Flirc case.  It ensures the case stays aligned properly.


## Assembly Instructions

1. Clean up the threaded parts (both male and female) using a tap and die.   Silicone spray can assist with lubricating the threads before screwing them.

1. Attach the fan to the OctoPi Tray using the self-tapping mounting screws that came with the fan.

1. Use an M4 screw and nut to attach the Mounting Arm to the Mounting Arm Rail Clamp.

1. Use the three remaining M4 screws, washers, and nuts as well as the OctoPi Tray spacers to attach the Mounting Arm to the OctoPi Tray. 

1. Attach the five Short Leveling Feet to the appropriate holes on the bottom of the OctoPi tray and Mounting Arm.

1. Snap the Mounting Arm Rail Clamp to the left front of the 3d printer.   

1. Attach the Raspberry Pi camera cable to the Raspberry Pi.

1. Attach the fan cable adapter to pins 4 and 6 (pin 4 is 5v, pin 6 is ground) of the Raspberry Pi.  

1. If using a Flirc case, unclip the cosmetic black top panel and set aside.  Place the Pi inside the case and route the cables through the bottom GPIO slot.

1. Place the Raspberry Pi in the OctoPi tray and route the Raspberry Pi camera cable through the triangular opening of the tray.   Feed the cable up through the cable guiding slot in the mounting arm.

1. Attach the lens to the camera.

1. Feed the other end of the Raspberry Pi camera cable through the slot of the Camera Case back and attach it to the Raspberry Pi HQ Camera.  Ensure correct orientation.  

1. Place the four M2.5 x 30mm screws and washers through the rear of the Camera case back and the HQ camera.   Place a nylon/rubber M2.5 washer on each of the four screws.   Then place an M2.5 nut on each of the four screws, finger tightening to hold the camera in place.  

1. Attach the mini ball head to the Mounting Arm using 1/4"-20 x 1/2" bolt.

1. Screw the 1/4"-20 jam nut on the mini ball head.    

1. Carefully attach the Camera case back and HQ camera to the mini ball head using the HQ camera's integrated tripod thread.   Tighten the jam nut in place to secure the the camera.

1. Route the USB-C power source along the rail of your printer, tucking the cord into the top channel of the aluminum extrusion where possible.   Route the cable under the OctoPi Tray spacer closest to the printer.

1. Route the USB-C power source through the square hole in the OctoPi Tray Lid and plug it in to the Raspberry Pi.   

1. If using a Flirc case, place the spring clip in the side of the case closest to the USB and network ports.   This clip simply holds the Flirc case against the side of the case opposite the fan.

1. Drop the OctoPi Tray Lid in place.

1. Use the USB C cord retainers to clip the USB C power source into place on the rail.

1. [Install OctoPi on your Raspberry Pi](https://octoprint.org/download/) (the SD card is accessible through the slot on the end of the OctoPi Tray).

1. Once OctoPi is running, go the Control tab and you should see a web camera image.    

1. The camera may appear in 4:3 ratio instead of 16x9 regardless of the OctoPrint settings.   You can fix this by SSHing into your OctoPi and editing: `boot/octopi.txt`

1. Adjust the focus and apeture of your camera and tighten the adjustment thumbscrews in place.   

1. Slide the Camera Case Front carefully on to the four screws.   Using the M2.5 washers and nuts, carefully secure the case in place.

1. If you wish to use the Tripod Thread Mount, insert the 2 Long Leveling Feet to the mount.

1. Clamp the Tripod Thread Mount to the left rear of the 3d printer.   Your light, etc. can be attached to the mount using the remaining 1/4"-20 x 1/2" bolt.

1. Adjust all the leveling feet.

1. Plug in a voltage isolated **(NO 5V PIN!)** USB-A to Micro USB cable from the Raspberry Pi to the printer.  It is **very important** to ensure that your cable does not have a 5V pin or your printer  and Raspberry Pi may be damaged!
