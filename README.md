# raspbian-rtl8812au

* an Ansible role for compiling the rtl8812au wifi driver for raspbian on the Raspberry Pi
* has been tested with Raspbian on a 
[Raspberry Pi 2 Model B](https://www.raspberrypi.org/products/raspberry-pi-2-model-b/) and 
[Raspberry Pi Zero](https://www.raspberrypi.org/products/pi-zero/)
  * Raspbian Jessie release 2016-05-27 using kernel version 4.4.11-v7+
  * Raspbian Jessie release 2016-09-23 using kernel version 4.4.21-v7+
  * Raspbian Jessie release 2017-01-11 using kernel version 4.4.34-v7+
* some tasks require sudo permissions

## Read on

* [https://github.com/notro/rpi-source/wiki](https://github.com/notro/rpi-source/wiki)
* [https://github.com/gnab/rtl8812au](https://github.com/gnab/rtl8812au)
* [Compiling the rtl8812au Wifi Driver for Raspbian](https://layereight.de/raspberry-pi/2016/08/25/raspbian-rtl8812au.html)

## Install the role via Ansible Galaxy

* execute `ansible-galaxy install -r requirements.yml`
* contents of requirements.yml:
```
  - name: raspbian-rtl8812au
    src: https://github.com/layereight/raspbian-rtl8812au
    version: "1.3"
```
* also see the [Ansible Galaxy documentation](http://docs.ansible.com/ansible/galaxy.html)
