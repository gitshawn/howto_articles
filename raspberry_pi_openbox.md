# Raspberry pi delicious, fast and usable - Work In Progress
### Featuring openbox gui
### Tested on a Raspberry pi 4b 4gb

- Install and boot PiOS Lite
- Install xorg (X11 GUI), openbox (X Window Manager), obconf (GUI App to config openbox)
```
sudo apt-get install \
--no-install-recommends \
xserver-xorg \
x11-xserver-utils \
xinit \
openbox \
obconf
```
- Install openbox components
```
sudo apt-get install \
--no-install-recommends \
tint2
```
- Install apps
```
sudo apt-get install \
--no-install-recommends \
chromium-browser
```

- Turn off unwanted things in PiOS
```
sudo systemctl disable dhcpcd
sudo /etc/init.d/dhcpcd stop
```
