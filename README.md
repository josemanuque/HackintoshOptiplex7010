# macOS Big Sur on a Dell Optiplex 7010

OpenCore based installation of macOS 11.6.7 in a Dell Optiplex 7010. Used USB Flash Drive with recovery dmg.

Specs:

- Dell Optiplex 7010 USFF
- Intel Core i7-3770s
- Intel Graphics HD 4000 (iGPU)
- OpenCore 0.8.2 Release
- macOS Big Sur 11.6.7
- Running macOS installation on an external SSD using USB port


![Screen Shot 2022-07-13 at 9 50 53 PM](https://user-images.githubusercontent.com/80563786/178921706-0d654ef4-737e-41db-bfa0-daeb869bd7d8.png)


What works:
- macOS, latest version at the moment.
- Internal audio from speakers.
- Power Management.
- No kernel panics.
- USB 3.0
- USB 2.0 Partially
- Sleep is partially working.
- iServices (iCloud, iMessage, FaceTime)
- Light, clean and stable installation.

Issues:
- USB 2.0 is not working after boot. (If a device is plugged 
- Sleep has given issues 2 times, USB devices get disconnected and fan starts spinning.
- During installation no USB 2.0/3.0 is being read except for the flash drive. (Solved connecting the Flash drive, mouse and keyboard to a hub) Issue gets fixed after installation.
- OpenCore GUI not included atm.


# Version 1.0 Log
- Fixed USB 3.0 Issues with SSDT-HPET generated by SSDTTime and SSDT-XOSI from here https://github.com/dortania/Getting-Started-With-ACPI/tree/master/extra-files/compiled
- For SSDT-HPET choose default options in SSTTime.
- Used previous USBMap.kext generated with USBMap tool.
- Huge credit to GTG from the tonymacx86 forum for the Catalina Desktop guide in which this solution was found.


# Version 0.2b

Followed Dortania's OpenCore Post-Install Guide.
-Fixed Power Management using ssdtPRGen
-Audio for this machine uses ALC269, used layout 15 converted to <15000000> on data plist.


Credits
- Dortania
- OpenCore devs
- CorpNewt
- GTG from tonymacx86
