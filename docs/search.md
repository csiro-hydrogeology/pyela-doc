## Testing PVGeo and vtki

```bash
pip install PVGeo
```

While still trying to run the mayavi based stuff that does OK on windows but not on Linux, decided to make sure I have proper nvidia drivers 

Unsuccessful trial [using these instructions](https://linuxconfig.org/how-to-install-the-latest-nvidia-drivers-on-debian-9-stretch-linux)
uninstalled everything nvidia-* then found [deb wiki NvidiaGraphicsDrivers](https://wiki.debian.org/NvidiaGraphicsDrivers) and [this](https://wiki.debian.org/Bumblebee#Installation)

```text
update-alternatives: error: alternative /usr/lib/nvidia/bumblebee for glx not registered; not setting
rmmod: ERROR: Module nouveau is in use
```
