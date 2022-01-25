# World Filpper Asset Extractor

#### DISCLAIMER: All the rights of extracted assets belong to cygames/citail and/or its affiliates. I do not encourage you to use any of extracted assets in inappropriate purpose. If you use any assets extracted by this tool, you do so at your sole risk.

<p align="center">
 <img src="https://user-images.githubusercontent.com/19164553/150029824-aace84ff-766d-4555-ba72-794d610761b5.gif" alt="theoSpecial" />
</p>

Asset Extraction tool for World Flipper.

This tool extracts the assets from world flipper application installed on your device / emulator using ADB and FFDEC, rename digested file paths with original file path, restore corrupted png and mp3 data, export irregular (amf, orderedmap, etc) files in regular data format such as json.

Currently only supports Global / Japan variants. 

## Installation

Check out the [release page of this repo](https://github.com/ScripterSugar/wdfp-extractor/releases).

## Requirements

Currently only supports Windows (recommended 10 or higher)

Requires [Java 8 or later](https://www.java.com/en/download/) to run FFDEC.

if you're willing to extract assets from real device, your device must be rooted.

## Recommended environments

The tool only tested for limited use cases, thus might has various bugs / crahses among other enviornments. Basically this tool works best with modified, non-production adbd, which supports adb running as root permission and grants full access to data directory.

### Emulator
- Nox player (version 7.0.x) - **Recommended (Global)**

### Real device
- Pixel 2 (Android 11), Pixel 4 XL (Android 12)

## Usage
![wdfp](https://user-images.githubusercontent.com/19164553/149924519-91e016e3-5ac7-4d97-a8f3-c7c833f79e76.gif)

Simply just connect your device, select the directory you want to save your assets, and click on the Extract Data button.

**Do not close the app even if it hangs. The process might hangs a lot and few tasks require more than dozens of minutes. Be patient while extraction is in progress**

## Supported Assets
- APK
- Decompiled SWF
- Master table
- Character image assets
- Character image atlases/frame/parts/timeline (exported as json format)
- Miscellaneous image assets.
- Audio files including BGM, Character voice lines, S/E and more.
- Cropped sprites based on atlases and sprite sheet
- Animated images generated from sprites (Character images only)

## Planned feature
- Support extraction of ability texts
- Data viewer

## Contributing

I won't actively manage this repository as far as it works for me, so if you're having trouble using the tool on your side, in most cases you'll have to fix the problem yourself. You can still issue the tickets, but do not expect me to actively fix it. Please feel free to open any PR.

If you want more asset coverage added to tool, please provide the details about assets you want to export, including file formats, asset path, format of data, etc.

The application built from the [electron-react-boilerplate](https://github.com/electron-react-boilerplate/electron-react-boilerplate). Refer to the repository to check how to install dependencies and start development on your local machine.




