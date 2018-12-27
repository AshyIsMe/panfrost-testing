# Panfrost on rockpro64
Building and running panfrost on the rockpro64 on ayufan's ubuntu bionic build.

Build as per instructions here: https://panfrost.freedesktop.org/building-panfrost-mesa.html

## Ansible automated steps

The ansible playbook playbook-ayufan-ubuntu.yml will build the panfrost mesa repo on a rockpro64 running ayufan's bionic lxde image.




## Manual Steps

1. Upgrade to cosmic

Followed these steps: [https://linuxconfig.org/how-to-upgrade-ubuntu-to-18-10-cosmic-cuttlefish#h9-how-to-upgrade-ubuntu-the-debian-way]


1. Now install prereqs

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
weston \
xwayland \
libwayland-dev \
wayland-protocols \
libwayland-egl-backend-dev \
libxrandr-dev


```
