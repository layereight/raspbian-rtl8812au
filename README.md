# raspbian-rtl8812au

* an Ansible role for compiling the rtl8812au wifi driver for raspbian on the Raspberry Pi
* has been tested with Raspbian on a 
[Raspberry Pi 2 Model B](https://www.raspberrypi.org/products/raspberry-pi-2-model-b/) and 
[Raspberry Pi Zero](https://www.raspberrypi.org/products/pi-zero/)
  * Raspbian Jessie release 2016-05-27 using kernel version 4.4.11-v7+
  * Raspbian Jessie release 2016-09-23 using kernel version 4.4.21-v7+
  * Raspbian Jessie release 2017-01-11 using kernel version 4.4.34-v7+
  * Raspbian Jessie release 2017-04-10 using kernel version 4.4.50-v7+
  * Raspbian Stretch release 2017-09-07 using kernel version 4.9.41-v7+
  * Raspbian Stretch release 2017-11-29 using kernel version 4.9.59-v7+

## Requirements

* Raspberry Pi with Raspbian OS
* network access to the Raspberry Pi and [sshd enabled](https://layereight.de/raspberry-pi/2017/02/28/ssh-headless-Raspberry-Pi.html)
* a user with sudo permissions

## Install the role via Ansible Galaxy

Typical run:
```sh
$ ansible-galaxy install layereight.raspbian-rtl8812au
```

If you want to install a specific version in a collection with other roles using a role file:
```sh
$ ansible-galaxy install -r roles.yml
```
*roles.yml*
```YAML
- name: layereight.raspbian-rtl8812au
  src: layereight.raspbian-rtl8812au
  version: "1.4"
```
* also see the [Ansible Galaxy documentation](http://docs.ansible.com/ansible/galaxy.html) and the 
[Ansible Galaxy introduction](https://galaxy.ansible.com/intro)

## Role Variables

No variables needed.

## Example Playbook

Typical playbook run:
```sh
$ ansible-playbook -i inventory rtl8812au.yml
```

*inventory*
```INI
[raspberrypi]
mypi ansible_host=192.168.0.101 ansible_user=pi ansible_ssh_pass=raspberry 
```

*rtl8812au.yml*
```YAML
- hosts: raspberrypi
  
  roles:
    - raspbian-rtl8812au
```

## Read on

* [https://github.com/notro/rpi-source/wiki](https://github.com/notro/rpi-source/wiki)
* [https://github.com/gnab/rtl8812au](https://github.com/gnab/rtl8812au)
* [Compiling the rtl8812au Wifi Driver for Raspbian](https://layereight.de/raspberry-pi/2016/08/25/raspbian-rtl8812au.html)
