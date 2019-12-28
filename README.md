# Esp32MicroWebSrv

.bin for ESP32 to test MicroWebSrv in AP mode 

# Common use

SSID Esp32Peacock
192.168.4.1

add /get?test1=value1&test2=value2 to test GET method

use Old Version <MicroPython V 1.11 to Solve ampdu ignore deleting tx error

http://micropython.org/resources/firmware/esp32spiram-idf3-20190529-v1.11.bin

# How to flash
- Erase Flash
python esptool.py -p com5 erase_flash
- Write bin
python esptool.py -p com5 -b 115200 write_flash -z  0x0000 flash_Esp32MicroWebSrv.bin

# How to debug ESP32 MicroPython

use UPyCraft

# Original

https://microwebsrv.hc2.fr/

https://github.com/jczic/MicroWebSrv


# How to save bin from ESP
python esptool.py -p com5 -b 115200 read_flash 0 0x400000 Your.bin



