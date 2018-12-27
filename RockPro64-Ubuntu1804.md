
# Panfrost on rockpro64
Building and running panfrost on the rockpro64 on ayufan's ubuntu bionic build.

Build as per instructions here: [https://panfrost.freedesktop.org/building-panfrost-mesa.html]

```
rock64@rockpro64:~$ uname -a
Linux rockpro64 4.4.132-1075-rockchip-ayufan-ga83beded8524 #1 SMP Thu Jul 26 08:22:22 UTC 2018 aarch64 aarch64 aarch64 GNU/Linux

rock64@rockpro64:~$ lsb_release -a
No LSB modules are available.
Distributor ID: Ubuntu
Description:    Ubuntu 18.04.1 LTS
Release:        18.04
Codename:       bionic

```


# Prerequisites

## Upgrade to cosmic

Followed these steps: [https://linuxconfig.org/how-to-upgrade-ubuntu-to-18-10-cosmic-cuttlefish#h9-how-to-upgrade-ubuntu-the-debian-way]


## Now install prereqs
```
sudo apt remove -y libmali-rk-midgard-t86x-r14p0   # Maybe???
sudo apt autoremove


sudo apt install -y \
python3-pip \
python3 \
python3-setuptools \
python3-mako \
meson \
zlib1g-dev \
libexpat1-dev \
libdrm-dev \
weston xwayland libwayland-dev wayland-protocols \
libwayland-egl-backend-dev \
libxrandr-dev


```
