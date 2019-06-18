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

## Testing PVGeo and pyvista (ex vtki) - 2019-05

https://github.com/jessepisel/5minutesofpython/blob/master/Well%20log%20plots/PyVista.ipynb

adding to my ELA env:

```bash
cd ~/src/ela
cd pyvista
pip install appdirs nbval imageio-ffmpeg

python setup.py develop

pip install panel
pip install PVGeo
```
