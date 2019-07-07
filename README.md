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
4. Edit **country** to your two letter ISO Code.
If you do not know yours, check [countrycode.org](https://countrycode.org/) or keep the default of US

5. Edit the Wifi SSID and PSK to your Wifi Information.
```
ssid="YOUR-SSID"
psk="wpa_passphrase"
```
**Note**: If using clear text password make sure you keep the quotes. If you use a hash of the password, you do not need to have quotes.

6. Save the file and copy the file to the root directory on the microSD card that says "Boot".
7. How to enable SSH Server on boot.
```
In the root directory of the mircoSD card, you need to create a empty ssh file.
Linux: touch ssh
Windows: Right click, goto New, select Text File, set filename to ssh and press enter to save.
```
<p><strong>Note</strong>: Important that you have no <strong>txt</strong> extension, when create the file in windows or it will not enable ssh server.</p>
<p><strong>Note</strong>:If you do not see the <strong>txt</strong> extension in Windows Explorer, click View, check <strong>File Name Extensions</strong> by default this is not enable on windows.</p>
<p>You can connect to the Raspberry Pi by typing ssh <strong>pi@raspberrypi.local</strong> or <strong>ssh pi@(ip address)</strong> at the command prompt or terminal window and default password is <strong>raspberry</strong></p>

## Authors

**Shane Saunders** - *Initial work* - [asparatu](https://github.com/asparatu)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
