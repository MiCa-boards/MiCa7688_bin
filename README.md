# Binary Files

Bootloader: wrt7688.ldr 
Lede: wrt7688.img


# Updating the bootloader

You can update the bootloader with a USB drive. <br/>
You may need to update the bootloader in the few cases when either a new version is relreased or you build your own.<br/>
Do not disconnect the power source or unplug the USB drive during bootloader update process to avoid corrupting the data in the flash memory resulting in a device malfunction and booth failure.<br/>
A broken bootloader can no longer be updated. In this case you must re-program the Flash ROM through a hardware programmer.<br/>
Requirements<br/>
<br/>
The USB drive must have FAT file system or it will not be recognized by the MiCa7688 board.<br/>
<br/>
Steps<br/>
<br/>
Save the bootloader file (lks7688.ldr) in the root directory of a USB drive and make sure the filename is kept as lks7688.ldr. You can download the latest bootloader from Downloads page.<br/>
Unplug the power and plug in the USB drive to the OTG usb port of your MiCa7688.<br/>
Press and hold the WiFi button and plug in the power. After 20 seconds the WiFi LED will turn on. Release the WiFi button.<br/>
The board will read the bootloader (the WiFi LED blinks fast) and perform the bootloader update process (the WiFi LED blinks slowly). <br/>
It takes about 2 seconds to finish the bootloader update process.<br/>
<br/>
# Update the firmware with a USB drive
<br/>
This github include the latest firmware for your MiCa7688 ,  which may not have been installed at the factory. It is strongly recommended to update the firmware of your new board before proceeding with development. This section describes how to update the firmware with a USB drive and an OTG cable. <br/>
<br/>
Steps<br/>
<br/>
* Download the latest MiCa7688 Firmware.<br/>
* Copy the image wrt7688.img file to the root directory of a FAT32 USB drive.<br/>
* Unplug the usb power.<br/>
* Attach the USB drive to the HOST port of the board with an OTG cable.<br/>
* Press and hold the on-board WiFi button.<br/>
* Plug in the usb power.<br/>
* Keep holding the WiFi button for about 5 seconds. Do not release until the yellow LED for WiFi is off.<br/>
* DO NOT press the WiFi button longer than 20s or it will upgrade the bootloader.<br/>
* The WiFi LED blinks fast for about 3 minutes.<br/>
* The device will automatically reboot after firmware update is complete.<br/>


