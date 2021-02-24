# INSTALLATION GUIDE

1. Make a recovery USB using [**gibMacOS**](https://github.com/corpnewt/gibMacOS)
2. Copy **OC** folder and **Boot** folder to EFI partition of your USB.
3. Boot to Mac Recovery using usb you have just made
4. Turn on Wifi and install macOS on your SSD.
5. Boot to macOS you've installed
6. Using [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) or **OpenCore Configurator** to generate new SMBIOS
7. Copy **OC** folder and **Boot** folder from EFI partition of your USB to EFI partition of your SSD.
8. Restart and Enjoy your new hackintosh

***Notes:*** 
    
- *Change OpenCanopy background*
    1. You need a really big image! It seems this follows the same rules as any retina image, so you need an image double your resolution (3840x2160)
    2. Change the image to *PNG format*, rename it to *ModernBackground.png*
    3. Get [*chris1111/Icnspack-Builder*](https://github.com/chris1111/Icnspack-Builder) and install then launch the app.
    4. Click run. Drop your image on Icnspack-Builder. Click ready. Click save and save it somewhere.
    5. You should now have a resources.zip folder. Unzip that thing!
    6. Inside the folder should be Background.icns, put that into EFI/OC/Resources/Image
    7. Reboot and make sure it works
    
- *Turn on HiDPI for FullHD screen*
	1. Turn on HiDPI by Terminal
```
sudo defaults write /Library/Preferences/com.apple.windowserver DisplayResolutionEnabled -bool YES;
sudo defaults delete /Library/Preferences/com.apple.windowserver DisplayResolutionDisabled;
```	
	2. Extract folder DisplayVendorID-6af from /Tools/DisplayVendorID-6af.zip and copy it to /Library/Displays/Contents/Resources/Overrides
	3. Restart and enjoy


- If your pc has different specs, try to read [**OpenCore guide**](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf) or [**Dortania guide**](https://dortania.github.io/OpenCore-Desktop-Guide/installer-guide/) for more details

## Need help. Contact me
[![Telegram](https://img.shields.io/badge/Chat_on-Telegram-blue.svg)](https://t.me/tunglamvghy)
[![Messenger](https://img.shields.io/badge/Chat_on-Messenger-0078FF)](https://m.me/k38b.lamtung)
***Due to COVID-19, now I have free time. So if you want me to create your own EFI with a little payment, contact me via Telegram.***

## [Donate me](https://paypal.me/vtlam98)
If you want to donate, send me via [**PayPal**](https://paypal.me/vtlam98)
