**Device:** Pixel 4 XL

**Summary:** I tested the quack vanilla versions until v213. Almost everything works (wlan, mobile connection, camera etc) and the rom is very stable on this phone. Nevertheless the wlan connection isn't so stable even with full signal strength. 
I can't say anything about bugs in the gapps version for this phone because i refuse to use Builds with Gapps.


**Steps to install:**

    Step 1: Download the quack vanilla build and the vbmeta from phh

    Step 2: Boot the phone into fastboot mode (over hardware buttons or adb)
    
    Step 3: Flash the vbmeta.img. 
            Command: flash vbmeta vbmeta.img

    Step 4: Boot into fastbootd mode.
            Command: fastboot reboot fastboot

    Step 5: Erase the current system.
            Command: fastboot erase system

    Step 6: Flash the build of phh quack.
            Command: flash system "Name of the build".img

   Step 7: Erase userdata.
           Command: fastboot -w

   Step 8: Reboot the phone
           Command: fastboot reboot



    flash this image with the fastboot utility:


**Hardware support:**

* Camera 	              Works
2. Speaker / Mic 	      Works
Bluetooth 	              Not working
WiFi 	                      Works (but completly stable)
SIM / Mobile Data / Voice     Works
VoLTE 	                      Not tested 
Fingerprint 	              Not tested
NFC 	                      Not working
Offline Charging 	      Not tested
NFC                           Not working
Storage connection to PC      Works