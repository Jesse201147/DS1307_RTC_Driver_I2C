## Driver for DS1307 RTC use python3

Tested on:

- Raspberry Pi 4B
- ODROID-C4

## Install

```bash
# clone source code
git clone https://github.com/Jesse201147/DS1307_RTC_Driver_I2C.git
# install smbus
sudo apt install python-smbus
# run
cd DS1307_RTC_Driver_I2C
python3 ds1307 -h
```

## Deploy

```bash
# install pyinstaller
pip install pyinstaller
# Compile Source code
pyinstaller -F ds1307.py
# Copy executable file to /usr/bin
sudo cp ./dist/ds1307 /usr/bin/
# Test
ds1307 -h
```