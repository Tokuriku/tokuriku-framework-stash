# HardwareScanner Framework API Document
#### Part of the Tokuriku-Framework-Stash GitHub Repository
https://github.com/Tokuriku/tokuriku-framework-stash

All the Methods in this Framework are dependent on the "**HardwareScanner**" Class and are **Type Methods**. This Framework is for **Xcode 6.3** and **Swift 1.2** or lower.

### Installation
To use this Framework:

1. Download the full Repository at https://github.com/Tokuriku/tokuriku-framework-stash
2. Take the Framework itself (the Lego block) in the **HardwareScanner** folder and insert it into your project.
3. Make sure the Framework is not only linked but **Embedded** also in the project's General tab.
4. Call the framework with `Import HardwareScanner` before using it in a Class.

### Usage
The main method you'll want to use is the public method:

    model() -> String

It outputs the model of the device used by the app in a String.

The possible models are:

- iPhone 1G
- iPhone 3G
- iPhone 3GS
- iPhone 4
- Verizon iPhone 4
- iPhone 4S
- iPhone 5 (GSM)
- iPhone 5 (GSM+CDMA)
- iPhone 5c (GSM)
- iPhone 5c (GSM+CDMA)
- iPhone 5s (GSM)
- iPhone 5s (GSM+CDMA)
- iPhone 6
- iPhone 6 Plus
- iPod Touch 1G
- iPod Touch 2G
- iPod Touch 3G
- iPod Touch 4G
- iPod Touch 5G
- iPad
- iPad 2 (WiFi)
- iPad 2 (GSM)
- iPad 2 (CDMA)
- iPad 2 (WiFi)
- iPad Mini (WiFi)
- Pad Mini (GSM)
- iPad Mini (GSM+CDMA)
- iPad 3 (WiFi)
- iPad 3 (GSM+CDMA)
- iPad 3 (GSM)
- iPad 4 (WiFi)
- iPad 4 (GSM)
- iPad 4 (GSM+CDMA)
- iPad Air (WiFi)
- iPad Air (Cellular)
- iPad Air
- iPad Mini 2G (WiFi)
- iPad Mini 2G (Cellular)
- iPad Mini 2G
- iPad Mini 3 (WiFi)
- iPad Mini 3 (Cellular)
- iPad Mini 3 (China)
- iPad Air 2 (WiFi)
- iPad Air 2 (Cellular)
- Apple TV 2G
- Apple TV 3
- Apple TV 3 (2013)
- Simulator
- Unknown Hardware

### Changelog
Current Version (1.1)
- Made the framework support Xcode 6.3 compiler

Version 1.0
- Full functionality