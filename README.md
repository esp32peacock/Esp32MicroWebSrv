# Esp32MicroWebSrv

.bin for ESP32 to test MicroWebSrv in AP mode 

SSID Esp32Peacock
192.168.4.1

# How to flash
- Erase Flash
python esptools.py -p com 5 erash_flash
- Write bin
python esptools.py -p com5 -b 115200 write_flash -z  0x0000 Esp32MicroWebSrv.bin


https://microwebsrv.hc2.fr/

https://github.com/jczic/MicroWebSrv
