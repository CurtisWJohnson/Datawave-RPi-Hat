# Datawave-RPi-Hat

Requirements
- Datawave Raspberry Pi Hat
- Raspberry Pi
- eepromutils (https://github.com/raspberrypi/hats.git)

From the command line on the Raspberry Pi

Download appropriate files
```Code
git clone https://github.com/CurtisWJohnson/Datawave-RPi-Hat.git
cd Datawave-RPi-Hat
```

Compile the .eep file.
```Code
sudo ./eepmake Datawave-rpi.txt Datawave-rpi.eep Datawave-rpi.dtb
```
Flash the .eep file to the EEPROM on the Pi. **Needs to be done while holding pin 26 on the Pi low**
```Code
sudo ./eepflash.sh -w -f=Datawave-rpi.eep -t=24c32
```
Reboot the Pi
```Code
sudo reboot
```
