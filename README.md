# ASUS G14 EasyEffects Presets for Linux

*Note: These may work well on G15 and other ASUS models as well*

## Overview

When you run Linux on ASUS notebooks, you lose support for Dolby Atmos profiles. The inbuit speakers sound "okay" but not as good as in Windows.

This project is an attempt to fix and improve on the Dolby Atmos effects for common use cases, and to adjust the EQ curve to compensate for the limitations of the G14's speakers.

## Usage

These profiles are currently designed to be used with "Over-Amplification" enabled. There is some gentle volume auto-leveling, however it's not designed to get everything to "full volume". Otherwise system sounds and sudden sounds would get distorted.

In general the autogain will try to target -18dB, which should be plenty of room to have good manual control of the volume as well, while keeping things generally within a sensible volume range.

## Installation

1. Install [EasyEffects](https://github.com/wwmm/easyeffects) 
2. Copy the `easyeffects` folder to `~/.config`.
3. Open EasyEffects and select a profile
4. (Optional) enable "Over-Amplification" in Gnome Tweaks

## Project Goals

The goals of this project are several, based on my personal listening preferences and scenarios:

1. Keep the dynamic range and quality of music and movies intact (don't squash the hell out of them)
2. Control harsh and unpleasant qualities like lower quality notebooks DACs and hard sibilants (by adding some 2nd order harmonics)
3. Need to change presets as little as possible, i.e. sensible and useful use cases

## Notes

So far I haven't used or captured impulse responses from Dolby Atmos from Windows, simply because I haven't felt I've needed to. I've been pretty happy with the results and am actually finding the profiles more useful than Dolby Atmos.

But tell me what you think, and I'll continue to test and improve these over time 😊.
