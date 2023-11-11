<img src="https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Logos/OpenCore_with_text_Small.png" width="200" height="48"/>

# Hackintosh-OpenCore-EFI-DELL-Optiplex-3050

Welcome to the Hackintosh-OpenCore-EFI-DELL-Optiplex-3050 repository! This repository provides a pre-made EFI setup for the OpenCore bootloader specifically designed for the Dell Optiplex 3050.

<img src="https://media.discordapp.net/attachments/321319496990326784/989091420201693225/Zrzut_ekranu_2022-06-22_o_10.55.57.png">

## Current Version - OpenCore 0.9.6 DEBUG

This repository includes a "Plug-and-Play" EFI configuration for the OpenCore bootloader, as well as all the necessary files to install and run macOS on your Dell Optiplex 3050. For the latest version, please visit the [OpenCore 0.9.6 release](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.5).

## Sonoma NOTE:

Please be aware that Apple has not removed any of the kexts for Kaby Lake's iGPUs as of the Release Candidate stage of Sonoma. To run Sonoma, you should change your SMBIOS to `iMac19,1`.

Refer to the "SMBIOS" section below, as using this SMBIOS is necessary for proper iServices functionality. The situation may change in the future, depending on Apple's actions. Thanks to Intel, it appears that spoofing from Kaby Lake to Coffee Lake (KBL -> CFL) is possible so will come in handy if needed.

**P.S.**: An updated reference image is needed, so if someone achieves success, please consider contributing. This repository started as a result of boredom in class and now that I've graduated, it's become a bit of a guessing game.

### SMBIOS:

The included SMBIOS in this repository is not associated with a purchased Apple device. For your own sake, it's not recommended to use it.

To generate your own SMBIOS, you can use the following tool:
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

You just need a invalid or unused SMBIOS to copy-paste the required info, especially if you intend to use iServices.

## Credits:

- [Lilu](https://github.com/acidanthera/Lilu/)
- [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
- [HibernationFixup](https://github.com/acidanthera/HibernationFixup)
- [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
- [USBInjectAll](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads)
- [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- [OpenCanopy's resources](https://github.com/acidanthera/OcBinaryData)

 
