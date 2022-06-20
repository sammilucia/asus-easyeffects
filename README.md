# ASUS G14 EasyEffects Presets for Linux

*Note: These may work well on G15 and other ASUS models as well*

## Overview

When you run Linux on ASUS notebooks, you lose support for Dolby Atmos profiles. The inbuit speakers sound "okay" but not as good as in Windows.

This project is an attempt to fix and improve on the Dolby Atmos effects for common use cases, and to adjust the EQ curve to compensate for the limitations of the G14's speakers.

## Usage

These profiles are currently designed to be used with "Over-Amplification" enabled. There is some gentle volume auto-leveling, however it's not designed to get everything to "full volume". Otherwise system sounds and sudden sounds would get distorted.

In general the autogain will try to target -18dB, which should be plenty of room to have good manual control of the volume as well, while keeping things generally within a sensible volume range.

## Use cases

### 1. Talking + Podcasts

If you listen to a lot of YouTube/BitChute/etc., audiobooks, and podcasts, especially while doing other things, this preset cleans up a lot of common problems which I find distracting like:
-  Background noise
-  Room noise / reverberation
-  Strong or piercing sibilants ('S' sounds)
-  Stereo information (most of the stereo image is removed, because for speaking, it's generally useless and can be distracting)

### 2. Movie

This preset adds some gentle EQ at 1kHz and 2.8kHz to improve intelligibility of speech, and increases stereo width using mid-side (M/S) processing, while still leaving the sound pretty dynamic. Loud bits should still be loud, and quiet bits should still be quiet—albiet probably a little more audible for the very quiet scenes.

### 3. Music

This preset is designed to give a fairly flat frequency response across the spectrum, to represent the music as the artist intended. It does *not* attempt to apply a "Loudness curve" ("V-shaped curve") that a lot of people like. I am an audio engineer, so prefer listening to "flat" speakers. There is also some mild notch EQ to address some problem areas of the G14's speakers.

I decided to not widen the stereo image for this preset, because I find a wide stereo image can be distracting when I'm trying to work. So this is designed for as accurate representation of music as possible without much flourish.

### 4. Headphones

This preset does not attempt to add any EQ, leveling, exciter, or warmth, because we will all have different headphones. It does however add a sensible amount of stereo crosstalk between the L + R channels (because headphones are not actually "stereo", they are "binaural", so this attempts to fix this to give more of an impression of *speakers*).

I will probably revisit this preset at some point when I try to write some music and find out if this preset translates to speakers (or completely fails).

### 5. Speakers

This is a basic preset which attempts to address deficiencies in the G14's speakers, without any specific use case in mind. Think of this like a "general use" preset that you can possibly use for everything if you can't be bothered.

### 6. Speakers (Wide)

The same as "Speakers" but with some M/S processing to increase stereo width.

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
