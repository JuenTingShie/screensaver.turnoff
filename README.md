[![GitHub release](https://img.shields.io/github/release/dagwieers/screensaver.turnoff.svg)](https://github.com/dagwieers/screensaver.turnoff/releases)
[![Build Status](https://travis-ci.org/dagwieers/screensaver.turnoff.svg?branch=master)](https://travis-ci.org/dagwieers/screensaver.turnoff)
[![Codecov status](https://img.shields.io/codecov/c/github/dagwieers/screensaver.turnoff/master)](https://codecov.io/gh/dagwieers/screensaver.turnoff/branch/master)
[![License: GPLv3](https://img.shields.io/badge/License-GPLv3-yellow.svg)](https://opensource.org/licenses/GPL-3.0)
[![Contributors](https://img.shields.io/github/contributors/dagwieers/screensaver.turnoff.svg)](https://github.com/dagwieers/screensaver.turnoff/graphs/contributors)

# Kodi screensaver that turns your screen off to save power

This Kodi screensaver turns your TV, projector or monitor off, so it can actually "save your screen".


## How does it work ?

It supports the following methods:

- **CEC (built-in)**
  - The screensaver forces the display to go into Standby using internal CEC controls.

- **No Signal on Raspberry Pi (using vcgencmd)**
  - The screensaver causes 'no signal' using the vcgencmd utility. This only works on Raspberry Pi.

- **DPMS (built-in)**
  - The screensaver immediately forces the display off using internal DPMS (Energy Star) controls.

- **DPMS (using xset)**
  - The screensaver immediately forces the display off using the `xset` utility to set DPMS off state.

- **DPMS (using vbetool)**
  - The screensaver immediately forces the display off using the `vbetool` utility to set DPMS off state.

- **DPMS (using xrandr)**
  - The screensaver immediately forces the display off using the `xrandr` utility to set DPMS off state.

- **CEC on Android (kernel)**
  - The screensaver immediately forces the display off using kernel CEC controls and turns off device.

- **Backlight on Raspberry Pi (kernel)**
  - The screensaver turns off the backlight of the display. This only works on Raspberry Pi.

- **HDMI on Raspberry Pi (tvservice)**
  - The screensaver turns off the HDMI output using the 'tvservice' utility. This only works on Raspberry Pi, or possible other similar Broadcom chipsets.


Optionally it also can put your system to sleep or power it off.

Or log off your user or mute audio.

One can press the `HOME` key to deactivate the screensaver, depending on the method used and the state of the display it may turn your display back on.


## Related
A collection of related links:

- [Hardware hack for turning RPi on over CEC](https://forum.kodi.tv/showthread.php?tid=174315&pid=2651811#pid2651811)
