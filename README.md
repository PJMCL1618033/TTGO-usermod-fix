Install the TTGO-T-Dispaly usermod for WLED 0.15 on the ESP32 TTGO T-Display V1.1
================================================================================
SSID: WLED-AP
Password: wled1234
http://4.3.2.1
http://192.168.xxx.xxx


I was able to get this mod working by following the information from this post;
Usermods TTGO-T-Display does not compile  #4375
https://github.com/wled/WLED/issues/4375

The group of files I combined in the .7z provides aneasy way the consistently compile & upload. 
I really like the convenience of this usermod displaying the IP and other information. 

For me, using the normal install guide for this usermod always fails since WLED 0.13.
The TTGO-usermod-fix-main.zip file will setup VSC in a few step for consistsnt installation of this usermod.

1. Start with a known working module by installing the factory test program from the TTGO hardware test.7z. 
	Use NodeMCU-PyFlasher.exe to load it


Compiling on Visual Studio Code
1. Download and uzip WLED-main.zip file to desktop
2. Download and uzip copy2WLED-folder.7z to desdktop
3. From "copy2WLED-folder" drag wled00 & .pio folders to WLED-main folder. Yes for overwrite
4. From "copy2WLED-folder" drag platformio.ini file to WLED-main folder. Yes for overwrite
5. Setup Visual Studio Code following this guide:    https://kno.wled.ge/advanced/compiling-wled/
6. Connect TTGo module to a USB port   
7. Run Visual Studio Code program. 
8. Open WLED-main folder into Visual Studio Code (Ctrl+K Ctrl+O)
9. Wait for VSC to finih configuring  WLED project.
10. Click on PlatformIO 👽 aien and expand the >PROJECT TASKS tab
11. Click on the >esp32dev task
12. Click on the >esp32dev task again and click on Updoad
13. Project will compile and upload to TTG0 and reset the module.

CONNECTING 
1.  Wait for TTGO to display an IP:4.3.2.1 
2. From a Smart Phone use WIFI to connect to WLED-AP and sign in
3. From WLED config goto WiFi Setp 
4. Replace SSID and Network password with your system credentials
5. New IP for your network will display on TTGO screen

Pin 12 is the  DATA out to the WS2812 leds.




