# Ubuntu unkown display

In my situation xrandr output something like **`default connected primary`** instead of your connect interface

This may be nvidia drivers problem, so you can try reinstall drivers.

### Remove nvidia drivers
`sudo apt remove --autoremove 'nvidia-*'`

### Add repostory
`sudo add-apt-repository ppa:graphics-drivers/ppa`

### Install drivers version
`sudo apt install nvidia-driver-${VERSION}`

### Remove headers that not match driver version
`sudo apt remove 'linux-headers-${VERSION}*'`


### After that you need reboot
`sudo reboot`

## All commands
```sh
sudo apt remove --autoremove 'nvidia-*'
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt install nvidia-driver-${VERSION}
sudo apt remove 'linux-headers-${VERSION}*'
sudo reboot
```
