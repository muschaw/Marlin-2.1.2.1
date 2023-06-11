Lotmaxx Shark V2 SC-10


* Working LCD (Laser still not tested) - use the DWIN_SET from this repo
    * The screen now defaults to English
        * ABL (UBL) set to to 6 grid points (I can't get more to work with the screen code enabled)
    * Zoffset now shows 2 decimal points
    * Zoffset in all menus now moves in 0.05 and 0.01 despite the buttons saying 0.1/1.0 and 0.05/0.01, I can't fix it as I don't have access to the DWIN_SET source code, help anyone ?!
    * Laster mode does not switch on in the screen menus.
* Laser should be working (not tested)
* Replace M600 with G27 on fillamnet sensor trip (M600/M125 crashes with this LCD)
* Linear advance and input shaping enabled
* Arc and BEZIER_CURVE_SUPPORT disabled to save on RAM (if these are needed change the ABL-UBL grid to 5 points)
* Must run M502 & M500 after flashing and reboot (reboot not needed if not using the screen code)

This firmware is based on a "clean" 2.1.2.1 [Marlin](https://github.com/MarlinFirmware/)

The pinouts and LCD code came from these projects:   
* https://github.com/EfelerGibi/Marlin-Mod-For-Lotmaxx-Shark-v2 
* https://github.com/sm3dp/firmware_marlin2.0 
* https://github.com/spinixguy/sc-10-shark-v2-firmware
