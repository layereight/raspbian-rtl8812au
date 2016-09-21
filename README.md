# raspbian-rtl8812au

* an Ansible role for compiling the rtl8812au wifi driver for raspbian on the Raspberry Pi
* has been tested with a raspbian jessie lite (version 2016-05-27) on a 
[Raspberry Pi 2 Model B](https://www.raspberrypi.org/products/raspberry-pi-2-model-b/)
* should be run with sudo permissions

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
    version: "1.2"
```
* also see the [Ansible Galaxy documentation](http://docs.ansible.com/ansible/galaxy.html)
