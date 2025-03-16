TTGo usermod WLED Install
================================
SSID:     WLED-AP
Password: wled1234
http://4.3.2.1


http://192.168.xxx.xxx


Compiling Procedure
1. Download and uzip WLED-main.zip project to desktop
2. Download and uzip copy2WLED-folder.7z to desdktop
3. From "copy2WLED-folder" drag wled00 & .pio folders to WLED-main folder. Yes for overwrite
4. From "copy2WLED-folder" drag platformio.ini file to WLED-main folder. Yes for overwrite
5. Setup Visual Studio Code following this guide:
   https://kno.wled.ge/advanced/compiling-wled/
   
6. Connect TTGo module to a USB port   
7. Run Visual Studio Code program. 
8. Open WLED-main folder into Visual Studio Code (Ctrl+K Ctrl+O)
9. Wait for VSC to finih configuring  WLED project.
10. Click on PlatformIO 👽 aien and expand the >PROJECT TASKS tab
11. Click on the >esp32dev task
12. Click on the >esp32dev task again and click on Updoad
13. Project will compile and upload to TTG0 and reset the module.


CONNECTING TO TTGO from WEB
1.  Wait for TTGO display to display an IP:4.3.2.1 
2. From a Smart Phone use WIFI to connect to WLED-AP and then sign in
3. From WLED congig goto WiFi Setp 
4. Replace SSID and Network password with your system credentials
5. New IP for your network will display on TTGO screen
