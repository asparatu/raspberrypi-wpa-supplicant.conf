# Raspberry Pi Wifi Configuration File
Help you to setup a wpa supplicant configuration file for Raspbian Stretch or later on new headless Rasbian installation.

## Getting Started
These will be step-by-step instruction on how to create the configuration file on any OS and Rasbian installation.

## Prerequisites
**Git** or **Git for Windows** needs to be install on the pc. You can download a copy from [Git Official Website](https://git-scm.com/downloads).

## How to use
1. Run the following command in command prompt or terminal window:
```
git clone https://github.com/asparatu/raspberrypi-wpa-supplicant.conf.git
```
2. Move into the folder
```
cd raspberrypi-wpa-supplicant.conf
```
3. Edit the configuration file
```
Linux: nano wpa_supplicant.conf
Windows: notepad wpa_supplicant.conf
```
4. Set your country in configuration
```
Edit country to your two letter ISO Code.
```
If you do not know yours, check [countrycode.org](https://countrycode.org/) or keep the default of US
5. Edit SSID and PSK
```
ssid="YOUR-SSID"
psk="wpa_passphrase"
```
Change these to your WiFi settings, **Note**: If using clear text password make sure you keep the quotes.

6 Save the file and copy it the root of the microSD drive.
```
The drive  label should say "boot"
```
7. Enable SSH
```
Linux: touch ssh
Windows: Right click in boot root, goto New, select Text File, Delete name and Extension, rename ssh and save.
```
Insert the microSD card and plug in the Raspberry Pi. It will setup the Wifi Connection.
You can connect to the raspberrypi.local or ip address.

**Note**: You can use this on non-headless Raspberry Pi installation.

## Authors

* **Shane Saunders** - *Initial work* - [asparatu](https://github.com/asparatu)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
