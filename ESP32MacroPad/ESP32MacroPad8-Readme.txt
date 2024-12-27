Compiled with ESP32Arduino 2.0.17 and TFTeSPI 2.5.43 and ESP32 BLE Keyboard library: 
https://github.com/Cemu0/ESP32-BLE-Keyboard/tree/addSpecialKeySync which includes CapsNumScroll lock indicators
ESP32-WROOM CYB 3.5" LCD ST7796 480x320 LCD:
https://www.communica.co.za/products/bdd-esp32-lvgl-wifi-bt-3-5in-lcd?variant=50314510205228
-----------------------------------------------------------------------------------------------------------------------------------------------------
"I:\\Data\\Win10-3\\Arduino/ESP32MacroPad8.ino.elf"
"C:\\Users\\Tobias\\AppData\\Local\\Arduino15\\packages\\esp32\\tools\\esptool_py\\4.5.1/esptool.exe" --chip esp32 elf2image --flash_mode dio --flash_freq 80m --flash_size 4MB --elf-sha256-offset 0xb0 -o "I:\\Data\\Win10-3\\Arduino/ESP32MacroPad8.ino.bin" "I:\\Data\\Win10-3\\Arduino/ESP32MacroPad8.ino.elf"
esptool.py v4.5.1
Creating esp32 image...
Merged 27 ELF sections
Successfully created esp32 image.
"C:\\Users\\Tobias\\AppData\\Local\\Arduino15\\packages\\esp32\\hardware\\esp32\\2.0.17\\tools\\gen_esp32part.exe" -q "I:\\Data\\Win10-3\\Arduino/partitions.csv" "I:\\Data\\Win10-3\\Arduino/ESP32MacroPad8.ino.partitions.bin"
cmd /c if exist "I:\\Data\\Win10-3\\Arduino\\libraries\\Insights" "C:\\Users\\Tobias\\AppData\\Local\\Arduino15\\packages\\esp32\\hardware\\esp32\\2.0.17\\tools\\gen_insights_package.exe" "I:\\Data\\Win10-3\\Arduino" ESP32MacroPad8.ino "C:\\Users\\Tobias\\Documents\\Arduino\\ESP32MacroPad8"
Multiple libraries were found for "SD.h"
 Used: C:\Users\Tobias\AppData\Local\Arduino15\packages\esp32\hardware\esp32\2.0.17\libraries\SD
 Not used: C:\Program Files (x86)\Arduino\libraries\SD
 Not used: C:\Users\Tobias\Documents\Arduino\libraries\SD
Using library SPI at version 2.0.0 in folder: C:\Users\Tobias\AppData\Local\Arduino15\packages\esp32\hardware\esp32\2.0.17\libraries\SPI 
Using library TFT_eSPI at version 2.5.43 in folder: C:\Users\Tobias\Documents\Arduino\libraries\TFT_eSPI 
Using library FS at version 2.0.0 in folder: C:\Users\Tobias\AppData\Local\Arduino15\packages\esp32\hardware\esp32\2.0.17\libraries\FS 
Using library SPIFFS at version 2.0.0 in folder: C:\Users\Tobias\AppData\Local\Arduino15\packages\esp32\hardware\esp32\2.0.17\libraries\SPIFFS 
Using library SD at version 2.0.0 in folder: C:\Users\Tobias\AppData\Local\Arduino15\packages\esp32\hardware\esp32\2.0.17\libraries\SD 
Using library ESP32-BLE-Keyboard at version 0.3.2 in folder: C:\Users\Tobias\Documents\Arduino\libraries\ESP32-BLE-Keyboard 
Using library BLE at version 2.0.0 in folder: C:\Users\Tobias\AppData\Local\Arduino15\packages\esp32\hardware\esp32\2.0.17\libraries\BLE 
"C:\\Users\\Tobias\\AppData\\Local\\Arduino15\\packages\\esp32\\tools\\xtensa-esp32-elf-gcc\\esp-2021r2-patch5-8.4.0/bin/xtensa-esp32-elf-size" -A "I:\\Data\\Win10-3\\Arduino/ESP32MacroPad8.ino.elf"
Sketch uses 1318925 bytes (62%) of program storage space. Maximum is 2097152 bytes.
Global variables use 65640 bytes (20%) of dynamic memory, leaving 262040 bytes for local variables. Maximum is 327680 bytes.
esptool.py v4.5.1
Serial port COM10
Connecting....
Chip is ESP32-D0WD-V3 (revision v3.1)
Features: WiFi, BT, Dual Core, 240MHz, VRef calibration in efuse, Coding Scheme None
Crystal is 40MHz
MAC: f8:b3:b7:29:b8:74
Uploading stub...
Running stub...
Stub running...
Configuring flash size...
Flash will be erased from 0x00001000 to 0x00005fff...
Flash will be erased from 0x00008000 to 0x00008fff...
Flash will be erased from 0x0000e000 to 0x0000ffff...
Flash will be erased from 0x00010000 to 0x00153fff...
Compressed 17568 bytes to 12205...
Writing at 0x00001000... (100 %)
Wrote 17568 bytes (12205 compressed) at 0x00001000 in 1.3 seconds (effective 105.2 kbit/s)...
Hash of data verified.
Compressed 3072 bytes to 134...
Writing at 0x00008000... (100 %)
Wrote 3072 bytes (134 compressed) at 0x00008000 in 0.1 seconds (effective 393.2 kbit/s)...
Hash of data verified.
Compressed 8192 bytes to 47...
Writing at 0x0000e000... (100 %)
Wrote 8192 bytes (47 compressed) at 0x0000e000 in 0.1 seconds (effective 699.1 kbit/s)...
Hash of data verified.
Compressed 1325504 bytes to 834045...
Writing at 0x00010000... (1 %)
.....
Writing at 0x0014e48f... (100 %)
Wrote 1325504 bytes (834045 compressed) at 0x00010000 in 73.8 seconds (effective 143.6 kbit/s)...
Hash of data verified.

Leaving...
Hard resetting via RTS pin...
------------------------------------------------------------------------------------------------------------------------------------------------------

To install new version of ESP32 Arduino first delete it from boards manager, then delete the folder 
C:\Users\Name\AppData\Local\Arduino15\packages\esp32 then close and reopen Arduino IDE and then add the new ESP32 Dev Board again.

NB: Use Partition scheme No OTA 2MB APP/2MB SPIFFS 
 
Note: The [Cfg]->[m] Mouse page is not functional.
Note: Only Reset 0 is functional i.e. *r0* - *r1* and *r2* willl be used for deep sleep modes in the future

New changes:
All is new