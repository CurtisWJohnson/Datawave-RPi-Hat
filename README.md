# Datawave-RPi-Hat

Requirements
- Datawave Raspberry Pi Hat
- Raspberry Pi
- eepromutils (https://github.com/raspberrypi/hats.git)

From within Raspberry Pi
pi@raspberrypi: sudo ./eepmake Datawave-rpi.txt Datawave-rpi.eep Datawave-rpi.dtb
**Do the following while holding pin #26 on the Pi low**
pi@raspberrypi: sudo ./eepflash.sh -w -f=Datawave-rpi.eep -t=24c32
pi@raspberrypi: sudo reboot
