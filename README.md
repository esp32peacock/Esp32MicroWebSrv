# Esp32MicroWebSrv

.bin for ESP32 to test MicroWebSrv in AP mode 

# If want to use in STA mode
please change this line to

srv = MicroWebSrv(port=80, bindIP='0.0.0.0', webPath='www/')

# Common use

SSID Esp32Peacock
192.168.4.1

add /get?test1=value1&test2=value2 to test GET method

use microPython V 1.9.4 to Solve ampdu ignore deleting tx error

http://micropython.org/resources/firmware/esp32-idf3-20180511-v1.9.4.bin

# How to flash
- Erase Flash
python esptool.py -p com5 erase_flash
- Write bin
python esptool.py -p com5 -b 115200 write_flash -z  0x0000 flash_Esp32MicroWebSrv.bin


# How to save bin from ESP
python esptool.py -p com5 -b 115200 read_flash 0 0x400000 Your.bin


https://microwebsrv.hc2.fr/

https://github.com/jczic/MicroWebSrv

