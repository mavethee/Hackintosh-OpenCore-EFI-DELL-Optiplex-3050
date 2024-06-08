<img src="https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Logos/OpenCore_with_text_Small.png" width="200" height="48"/>

# Hackintosh-OpenCore-EFI-DELL-Optiplex-3050

Welcome to the Hackintosh-OpenCore-EFI-DELL-Optiplex-3050 repository! This repository provides a pre-made EFI setup for the OpenCore bootloader specifically designed for the Dell Optiplex 3050.

## Current Version - [OpenCore 1.0.0 DEBUG](https://github.com/acidanthera/OpenCorePkg/releases/tag/1.0.0)

This repository includes a "Plug-and-Play" EFI configuration for the OpenCore bootloader, as well as all the necessary files to install and run macOS on your Dell Optiplex 3050.

## Installation:

1. First of all, ensure you're firmware and drivers are generally up to date. Next download the EFI by getting it from assets in `Releases` page or cloning whole repo.

2. It may still boot with EFI as it is just fine but please ensure to dump your own SSDTs for `EFI/OC/ACPI` with [SSDTTime](https://github.com/corpnewt/SSDTTime), remember that every configuration differ even if it's the same model!

3. (Optional) Remove `USBInjectAll.kext` from `EFI/OC/Kexts`, map your own USB config using USBToolBox's [tool](https://github.com/USBToolBox/tool) and its [kext](https://github.com/USBToolBox/kext) referring to this [usage manual](https://github.com/USBToolBox/tool?tab=readme-ov-file#usage)

4. Please be aware that Apple has not removed any of the kexts for Kaby Lake's iGPUs as of the Release Candidate stage of Sonoma. ~~To run Sonoma, you should change your SMBIOS to `iMac19,1`~~. `iMac19,1` is now set by default. The included SMBIOS in this repository is not associated with a purchased Apple device. For your own sake, **it's not recommended to use it**. Re-generate `iMac19,1` SMBIOS for your EFI using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS). You just need a invalid or unused SMBIOS to copy-paste the required info, especially if you intend to use iServices.The situation may change in the future, depending on Apple's actions. Thanks to Intel, it appears that spoofing from Kaby Lake to Coffee Lake (KBL -> CFL) is possible so will come in handy if needed.

**P.S.**: An updated reference image is needed, so if someone achieves success, please consider contributing. This repository started as a result of boredom in class and now that I've graduated, it's become a bit of a guessing game.

## Credits:

- [AppleALC](https://github.com/acidanthera/AppleALC)
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
- [Lilu](https://github.com/acidanthera/Lilu)
- [OpenCanopy's resources](https://github.com/acidanthera/OcBinaryData)
- [OpenCore's bootloader](https://github.com/acidanthera/OpenCorePkg)
- [ProperTree](https://github.com/corpnewt/ProperTree)
- [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
- [SSDTTime](https://github.com/corpnewt/SSDTTime)
- [HibernationFixup](https://github.com/acidanthera/HibernationFixup)
- [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
- [USBInjectAll](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads)
- [USBToolBox](https://github.com/USBToolBox)
- [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
 
