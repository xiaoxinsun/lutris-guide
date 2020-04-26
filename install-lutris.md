### Install WINE

Ref: https://gaming.stackexchange.com/questions/341111/is-there-a-painless-way-to-run-starcraft-2-on-linux

```
# optional
sudo apt purge wine
```

### Install WINE stable per: https://wiki.winehq.org/Ubuntu
```
sudo dpkg --add-architecture i386 
wget -O - https://dl.winehq.org/wine-builds/winehq.key | sudo apt-key add -
sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ focal main'
sudo apt install --install-recommends winehq-stable
```

### Install Winetricks

note: may need additional steps that are not recorded below
```
wget https://raw.githubusercontent.com/Winetricks/winetricks/master/src/winetricks
winetricks d9vk_master
```

### install mesa vulkan driver
```
sudo apt update
sudo apt install mesa-vulkan-drivers libvulkan1
```

REBOOT

### Install lutris
Ref: https://lutris.net/downloads/
```
sudo add-apt-repository ppa:lutris-team/lutris
sudo apt-get update
sudo apt-get install lutris
```

### Launch Battlenet installer

Visit: https://lutris.net/games/starcraft/ and install via lutris