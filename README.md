#Runbook for Mumble 4Wire box on Raspberry Pi

This Runbook will setup a Headless Mumble on a Raspberry Pi with an Audioinjector soundcard hat

Preperations:
Put empty file named ’ssh' on image disc to enable ssh

Boot Raspberry Pi with mounted AudioInjector soundcard

Login to Raspberry Pi: ssh pi@xx.xx.xx.xx

Default Password: raspberry

Change password: passwd

add Raspberry Pi to hosts file

Run:  ansible-playbook playbook.yml -i hosts

-----------------------------------------------

ToDo: in playbook.yml

-Set mumble SoundCard setting in Mumble ($HOME/.config/Mumble/Mumble.conf & $HOME/.local/share/data/Mumble/Mumble/.mumble.sqlite)

-Create certificate for Mumble

-Settings in alsamixer: (/var/lib/alsa/asound.state)

hi-fi mixer ON in outputsection

Line-in Capture On

Set Input mux to Line in