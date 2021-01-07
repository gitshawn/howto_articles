# Raspberry pi delicious, fast and usable - Work In Progress
### Featuring openbox gui
### Tested on a Raspberry pi 4b 4gb

- Install and boot Raspberry Pi OS Lite
- Update and upgrade Pi OS
```
sudo apt-get update &&
sudo apt-get upgrade
```
- Install xorg (X11 GUI), openbox (X Window Manager), obconf (GUI App to config openbox)
```
sudo apt-get install -y \
--no-install-recommends \
xserver-xorg \
x11-xserver-utils \
xinit \
openbox 
```
- Install openbox components
```
sudo apt-get install -y \
--no-install-recommends \
obconf \
tint2 \
network-manager \
compton \
feh \
lightdm \
light-locker \
xdotool

sudo apt-get install -y --no-install-recommends perl cpanminus make  libgtk2-perl &&
wget https://raw.githubusercontent.com/trizen/obmenu-generator/master/obmenu-generator && 
sudo mv obmenu-generator /usr/bin/ &&
sudo chmod +x /usr/bin/obmenu-generator &&
mkdir ~/.config/obmenu-generator/ &&
wget https://raw.githubusercontent.com/trizen/obmenu-generator/master/schema.pl &&
sudo mv schema.pl ~/.config/obmenu-generator/ &&
sudo cpanm Linux::DesktopFiles &&
sudo cpanm Data::Dump &&
sudo cpanm File::DesktopEntry

```
- Install apps
```
sudo apt-get install -y \
--no-install-recommends \
terminator \
chromium \
chromium-sandbox
```

- Turn off unwanted things in PiOS
```
sudo systemctl disable dhcpcd
sudo /etc/init.d/dhcpcd stop
```
