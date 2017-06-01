#Binary Files
Bootloader: wrt7688.ldr 
Lede: wrt7688.img


#Updating the bootloader

You can update the bootloader with a USB drive. 
You may need to update the bootloader in rare cases when there is a new version of the bootloader or when you build your own bootloader.
Do not disconnect the power source or unplug the USB drive during bootloader update process, or else the data in the flash will be damaged causing a device malfunction and failure to boot up again.
This feature is implemented by the bootloader, it's crucial to flash with a working bootloader. A broken bootloader cannot be updated again. In this case you must re-program the Flash ROM through a hardware programmer.

Requirements

The USB drive must be in FAT file system or the file cannot be recognized by your MiCa7688 board.

Steps

Save the bootloader file (lks7688.ldr) in the root directory of a USB drive and make sure the filename is kept as lks7688.ldr. You can download the latest bootloader from Downloads page.
Unplug the power and plug in the USB drive to the OTG usb port of your MiCa7688.
Press and hold the WiFi button and plug in the power.After 20 seconds the WiFi LED will turn on. Release the WiFi button.
The board will read the bootloader (the WiFi LED blinks fast) and perform the bootloader update process (the WiFi LED blinks slowly). 
It takes about 2 seconds to finish the bootloader update process.


#Update the firmware with a USB drive

This github include the latest firmware for your MiCa7688 ,  which may not have been installed at the factory. It is strongly recommended to update the firmware of your new board before proceeding with development. This section describes how to update the firmware with a USB drive and an OTG cable. 

Steps

Download the latest MiCa7688 Firmware.
Copy the image wrt7688.img file to the root directory of a FAT32 USB drive.
Unplug the usb power.
Attach the USB drive to the HOST port of the board with an OTG cable.
Press and hold the on-board WiFi button.
Plug in the usb power.
Keep holding the WiFi button for about 5 seconds. Do not release until the yellow LED for WiFi is off.
DO NOT press the WiFi button longer than 20s or it will upgrade the bootloader.
The WiFi LED blinks fast for about 3 minutes.
The device will automatically reboot after firmware update is complete.

