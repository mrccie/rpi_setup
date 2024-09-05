# rpi_setup
Basic Rasperry Pi Standup Guide

## Purpose
This repository will serve as a place that other Raspberry Pi projects can point at in place of creating their own "Set up your Raspberry Pi" section.  This guide will walk through the basic foundation to get a system up and running, after which additional customization can occur.

## Target System(s)
This guide has been developed for Raspberry Pi Zero/Zero 2/3/4/5... basically any single-board computer produced by the Raspberry Pi folks.

## Setup Steps
The basic setup steps that are covered include:
- Creating a Bootable MicroSD Card
- (Optional, but Recommended) Customizing Your Raspbian OS Before Install

## Necessary Hardware
- Raspberry Pi (Zero/Zero 2/3/4/5)
- MicroSD card (8GB minimum, 16GB or larger recommended)
- A method to connect your microSD card to a computer (typically a USB dongle or, for laptops with SD card readers, a microSD-to-SD adapter)

## Good Links
- Toms has a [good guide](https://www.tomshardware.com/reviews/raspberry-pi-headless-setup-how-to,6028.html) that includes a section to enable options without using the OS editing options

## Stand Up the Pi

### Creating a Bootable MicroSD Card

1. Connect your microSD card to your computer
2. Go to the [Raspberry Pi software page](https://www.raspberrypi.com/software/) and download the appropriate Raspberry Pi Imager for your computer
3. Install and Run the Raspberry Pi imager (it's easy to install - just click "Install"!)
4. In the first window, select the Raspberry Pi device you want to set up, the operating system to install, and the storage device (microSD card) to install to. __Read the next section before hitting Next__

![image](https://github.com/user-attachments/assets/c9ab3c21-3878-4769-bbf7-ddf0eecfd9d8)
_In this example, I selected to create an image for a Raspberry Pi 4, load Raspbian (the vendor-preferred OS), and I selected my microSD card (the only visible option)_

### (Optional but Recommended) Customizing Your Raspbian OS Before Install
The easiest way to customize Raspbian is to modify the installation script that the Raspberry Pi Imager will use.  You can always customize after setup, but then you have to modify system files rather than using a simple GUI.  This guide only discusses this method of customization so... do it this way or get ready to use a search engine.

1. When presented with this screen, click "EDIT SETTINGS"
![image](https://github.com/user-attachments/assets/4b36b99d-48a4-4b5c-8ef4-124746d13a22)

2. On the "GENERAL" tab, fill out the settings you want then go to Services.  For reference, this is what mine look like for this build:
![image](https://github.com/user-attachments/assets/a3163474-68dd-497f-a38b-0cc7b1d527b7)
_Note: The Raspberry Pi Imager will remember your last-used settings, so you may not want to configure WiFi if you share a computer with someone who should not know your WiFi password_

3. If you will be using SSH to connect to your Pi, enable SSH in the SERVICES tab.   For reference, this is what my tab looks like:
   ![image](https://github.com/user-attachments/assets/4fd0b016-16db-4448-98e5-1c1756e2448a)

4. The OPTIONS tab gives you a few options.   For reference, this is what my tab looks like:
   ![image](https://github.com/user-attachments/assets/4fd0b016-16db-4448-98e5-1c1756e2448a)

5. Click SAVE, then click "YES" when asked "Would you like to apply OS customization settings?".  Click "YES" again to acknowledge that your microSD card will be erased to install the operating system.  Then wait a few minutes while the card is overwritten.  Eventually you will be told you can remove the SD card from the reader, signaling that you are done.





