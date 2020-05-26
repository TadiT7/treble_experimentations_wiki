# Samsung Galaxy A8 2018 - SM-A530F/W
Oreo Vendor:
https://forum.xda-developers.com/galaxy-a8-2018/samsung-galaxy-a8-2018-roms-kernels-recoveries--other-development/vendor-samsung-galaxy-a8-a8-2018-t3899455
 ## Hardware Support
 * Camera: 
Doesn't works 

 * Speaker / Microphone
Speaker, Microphone works
 * Bluetooth
works
 * Wifi
Works
 * SIM / Mobile Data / ingoing voice calls / outgoing voice calls
works
 * VoLTE
Doesn't work
* All sensors
works
 * NFC
works
 * Fingerprint Reader
works
 * 3.5mm audio jack
 ***
Pie Vendor:
https://forum.xda-developers.com/galaxy-a8-2018/samsung-galaxy-a8-2018-roms-kernels-recoveries--other-development/pie-vendor-galaxy-a8-a8-2018-t3931071

 ## Hardware Support
 * Camera: 
Works

 * Speaker / Microphone
Speaker, Microphone works
 * Bluetooth
Works
 * Wifi
Works
 * SIM / Mobile Data / ingoing voice calls / outgoing voice calls
Works 
 * VoLTE
Doesn't work (Samsung's VoLTE implementation is proprietary)
* All sensors
works
 * NFC
works
 * Fingerprint Reader
Works (On Q, the fingerprint workaround needs to be enabled via Treble App in Settings.)
 * 3.5mm audio jack
 ***
## Additional Notes
*(This isn't the case on GSI versions from Q) On Pie vendor, GSI boots only after reverting this [commit] (https://github.com/phhusson/device_phh_treble/commit/e064c6f3107ad92f8b19891a93104d80e8482935)


 ***
Android 10 GSI:
I tested a lot of pie and 10 GSI with vendor patching for pie. I had multiples issues like Whatsapp managing badly the camera, and SIMcard disappearing, sometimes freeze and reboot after a time.
Right now I use CAOS (2020.05.13) and these bugs disappeared. Many other GSIs have Whatsapp getting good FPS with camera.
A thing that always failed and still : charging wile power off. Charging is ok but you will not be able to boot except force shutdown (less volume and power for 5 - 10s)
A little list of my usage : 
 ## Hardware Support
 * Camera: 
Works
 * Speaker / Microphone
Speaker, Microphone works
 * Bluetooth
Not tested
 * Wifi
Works
 * SIM / Mobile Data / ingoing voice calls / outgoing voice calls
Works 
 * VoLTE
Not tested
* All sensors
I tested gyroscope - OK
 * NFC
Not tested
 * Fingerprint Reader
Not tested
 * 3.5mm audio jack
Works

 ## Tested By:
* @afalce - 2020-05-23
* @prashantp01 - 2019-05-12
* @prashantp01 - 2019-04-12
* @prashantp01 - 2019-03-12
* @prashantp01 - 2019-02-12
