# BsxM1
A set of PNG files wrapped in Apple .icns file format suitable for using as a theme for OpenCanopy which is part of OpenCore.

<img src="https://github.com/blackosx/BsxM1/blob/main/preview_ui.jpg" alt="theme_preview" border="0">

<img src="https://github.com/blackosx/BsxM1/blob/main/preview_password.jpg" alt="theme_preview" border="0">

**Requirements**<br>
[OpenCore](https://github.com/acidanthera/OpenCorePkg) with OpenCanopy installed and configured.

**Initial Setup of OpenCanopy**<br>
Please refer to [OpenCore beauty treatment](https://dortania.github.io/OpenCore-Post-Install/cosmetic/gui.html#setting-up-opencore-s-gui) at dortania.

**Compatible with OpenCore Version**<br>
0.7.0<br>
*Note: Since OpenCore 0.7.0, the EFI/OC/Resources/Image/ directory will contain a Vendor directory which in turn will contain subsequent theme dirs.*


**Using this theme**<br>
This repository contains a Blackosx directory with a sub-directory BsxM1 which contains all necessary ICNS files for the theme.

If you don't have a EFI/OC/Resources/Image/Blackosx directory in EFI/OC/Resources/Image/<br>
- then add the Blackosx directory to EFI/OC/Resources/Image/ directory in your systems EFI System Partition.

If you already have EFI/OC/Resources/Image/Blackosx/<br>
- then just add the BsxM1 directory

Either way, for this theme you will want to end up having
EFI/OC/Resources/Image/Blackosx/BsxM1

You can switch the icon set used by OpenCanopy by changing the 'PickerVariant' key in OpenCore's config.plist to match the vendor and theme name of the icon set you want to display. So to instruct OpenCanopy to use this icon set you want to set the PickerVariant key to Blackosx\BsxM1

```
                <key>PickerVariant</key>
                <string>Blackosx\BsxM1</string>
```

**Recommended Config changes**<br>
For the best experience using this theme you will want the text to display in white. This can be achieved by setting NVRAM->Add->4D1EDE05-38C7-4A6A-9CC6-4BCCA8B38C14->DefaultBackgroundColor to any colour other than Apple Grey, #BFBFBF or as used on config.plist, v7+/AA==

```
        <key>NVRAM</key>
        <dict>
            <key>Add</key>
            <dict>
                <key>4D1EDE05-38C7-4A6A-9CC6-4BCCA8B38C14</key>
                <dict>
                    <key>DefaultBackgroundColor</key>
                    <data>AAAAAA==</data>
```

**Credits**<br>
The design of this theme is based on the original Apple image for their M1 chip
