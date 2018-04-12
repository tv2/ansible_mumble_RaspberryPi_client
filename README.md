#Runbook for Mumble 4Wire box on Raspberry Pi

This Runbook will setup a Headless Mumble on a Raspberry Pi with an Audioinjector soundcard hat

Preperations:
* Put empty file named ’ssh' on image disc to enable ssh

* Boot Raspberry Pi with mounted AudioInjector soundcard

* Login to Raspberry Pi: ssh pi@xx.xx.xx.xx

    * Default Password: raspberry

* Change password: passwd

* add Raspberry Pi to hosts file 
    * copy hosts.example to hosts and edit

* Run:  ansible-playbook playbook.yml -i hosts

-----------------------------------------------

ToDo: in playbook.yml


* Create certificate for Mumble and add to Mumble.conf

* Setup GPI trig based on https://github.com/adafruit/Adafruit-Retrogame.git