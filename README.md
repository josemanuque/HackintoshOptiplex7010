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
- No kernel panics.
- USB 2.0 *
- Sleep is partially working.
- Light, clean and stable instalation

Issues:
- USB 3.0 is not working (XHC is not being recognized by macOS).
- Sleep has given issues 2 times, USB devices get disconnected and fan starts spinning.
- During installation no USB 2.0/3.0 is being read except for the flash drive. (Solved connecting the Flash drive, mouse and keyboard to a hub) Issue gets fixed after installation.
- No audio
- No Power Management SSDT (SSDT-PM.aml)
- OpenCore GUI not included atm.

