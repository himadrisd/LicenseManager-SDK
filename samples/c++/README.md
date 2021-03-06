- [Cross compilation](#cross-compilation)
  - [Raspberry Pi](#cross-compilation-rpi)
    - [Installing the toolchain](#cross-compilation-rpi-install)
      - [Windows](#cross-compilation-rpi-install-windows)
      - [Ubuntu](#cross-compilation-rpi-install-ubuntu)
      

There are 1 C++ sample: [Activation](activation). Check [here](README/README.md) on how to build and use them.

The C++ samples are common to all platforms: **Android**, **Windows**, **iOS**, **Raspberry Pi (3 or 4)**, **Linux**...

For **Android**, you don't need to use these samples. All our products contain Java code for Android to automate the license activation process.

<a name="cross-compilation"></a>
# Cross compilation #

Every sample contain a single C++ source file and is easy to cross compile. 

<a name="cross-compilation-rpi"></a>
## Raspberry Pi (Raspbian OS) ##

This section explain how to install Raspberry Pi 4 (Raspbian OS) toolchain to cross compile the samples. These instructions can be easily adapted to another target platform (e.g Android).

<a name="cross-compilation-rpi-install"></a>
### Installing the toolchain ###

<a name="cross-compilation-rpi-install-windows"></a>
#### Windows ####
The toolchain for Raspberry Pi 4 could be found at [http://sysprogs.com/getfile/566/raspberry-gcc8.3.0.exe](http://sysprogs.com/getfile/566/raspberry-gcc8.3.0.exe) and more toolchain versions are at [https://gnutoolchains.com/raspberry/](https://gnutoolchains.com/raspberry/).

If you haven't changed the installation dir then, it should be installed at **C:\SysGCC**. To add the toolchain to the **%PATH**:
```
set PATH=%PATH%;C:\SysGCC\raspberry\bin
```

<a name="cross-compilation-rpi-install-ubuntu"></a>
#### Ubuntu ####
```
sudo apt-get update
sudo apt-get install crossbuild-essential-armhf
```
