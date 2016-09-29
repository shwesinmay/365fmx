# F.C.E.-365-Firmware-Manager
F.C.E.-365-Firmware-Manager - iOS Firmware Tools
iOS Firmware Manager Tool

The application comes as a faster access route for the old CLI applications like xpwntool and libimobiledevice project. The application's main purpose is to bring access on CLI applications for firmware DMG Encryption / Decryption, ASR patching and restoring for persons that doesn't understand CLI applications.

This application is currently running on Windows only and requires .NET Framework installed on your computer to be able to run. Unlike other Firmware restore / Modify tools, F.C.E. 365 Firmware Manager does not need iTunes to be installed.

Basically, the app uses xpwntool and especially dmg.exe to Decrypt the ROOT FS DMG file inside the .IPSW Firmware using appropriate Firmware Keys, then using the same keys it encrypts back your modified ROOT File System DMG. The same thing applies to Ramdisk DMGs inside the IPSW Firmware. The application uses hfsplus to decrypt the ramdisk and allows you to create the patches for ASR, iBSS, iBEC and so on.

F.C.E. 365 Firmware Manager makes use of libimobiledevice, especially of idevicerestore CLI to restore an iPSW for your iDevice. The device selection is made by UDID and the restore options are: Erase Restore, Update Restore, Custom Restore, Restore Latest Available. Due to libimobiledevice integration, this app does not require iTunes to restore the iPSW. SHSH Blobs are also fetched automatically by idevicerestore.

This app includes a tool for getting the phone out of Recovery Mode with one click. It also makes use of ideviceinfo to query all information about your device whenever you need it.

All the sources codes for xpwn, libimobiledevice and usbmuxd are provided! Also the binaries used are provided separately in the "Binaries" folder as on the Data folder.

The iPhone Wiki Page: https://www.theiphonewiki.com/wiki/Firmware_Manager

