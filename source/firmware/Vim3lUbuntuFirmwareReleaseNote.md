title: Khadas VIM3L Ubuntu Firmware Release Notes
---

## Linux 4.9 Images

{% note info Note %}

VIM3L Only support **Ubuntu 20.04** for Linux 4.9.

{% endnote %}

--------------------------------------------------------------------------------------------------
**V1.0.4-210330: (OTA Release)**

1. fix watchdog
2. add ubuntu splash support
3. improve loglevel setup
4. fix board dependencies
5. fix npu package conflict with jpeg package

--------------------------------------------------------------------------------------------------
**V1.0.3-210317: (OTA Release)**

1. fix board package dependencies issue
2. fix desktop package dependencies issue
3. add gsensor support

--------------------------------------------------------------------------------------------------
**V1.0.2-210130: (OTA Release)**

1. VIM3L: fix load dts overlays failure with android u-boot
2. add kernel options
3. fix tengine_libs_deb
4. fix h265 encode i420 format
5. add usb gadget setup
6. npu package add ovxinc headers


--------------------------------------------------------------------------------------------------
**V1.0.1-210119: (OTA Release)**

1. fix tengine libraries
2. add usb otg device overlays descriptions


--------------------------------------------------------------------------------------------------
**V0.9.7-20201126: (OTA Release)**

1. NPU version 6.4.3CB
2. fixed kplayer
3. fixed wiringpi for focal


--------------------------------------------------------------------------------------------------
**V0.9.5-20200828: (OTA Release)**

1. npu library 6.4.2.1
2. add more HDMI resolutions

--------------------------------------------------------------------------------------------------
**V0.9.3-20200814: (OTA Release)**

1. Add kodi (18.7) support
2. Add python3-wiringpi support
3. Add support for customized freq setup
4. Add hardware optimization
5. Add CPU Frequency Setting desktop application (Applications->CPU Frequency Setting)
6. Fix fan_setup.sh
7. Add customer kernel args support

--------------------------------------------------------------------------------------------------
**V20200530: (Base Release)**

1. Initial support for Ubuntu 20.04 Focal
2. Linux 4.9.224

## Mainline Kernel Images

{% note info Note %}

VIM3L Only support **Ubuntu 20.04** for Mainline Linux. 

{% endnote %}


--------------------------------------------------------------------------------------------------
**V0.9.1-20200602: (OTA Release)**

1. Linux 5.7.0

--------------------------------------------------------------------------------------------------
**V20200530:**

1. Initial support for Ubuntu 20.04 Focal
2. U-boot 2020.04
3. Linux 5.7-rc7

{% note warn For OTA Releases %}

You can check [How To Upgrade The System](/vim1/HowToUpgradeTheSystem.html) to upgrade the system to latest release.

{% endnote %}
