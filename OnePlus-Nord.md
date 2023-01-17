Hello folks,

i could have gsi image flashed, 
what i did:

~~~
install OOS10 stock
enable oem
adb reboot fastboot
fastboot flashing unlock
fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img
fastboot flash recovery OrangeFox-R11.1_2_FBEv1-Unofficial-avicii.img
fastboot flash system system-squeak-arm64-ab-vndklite-floss.img
~~~

Adding some tests,

A10 image, arm64-ab-vanilla v222
~~~
camera: works
lte: works
wifi: works
bt: mute, no way to have it working
can patch for signature spoofing (nanodroid patcher)
can install magisk
~~~

A12.1 image, arm64-ab-vanilla v416
~~~
camera: works
lte: works
wifi: works
bt: works
cannot install magisk 25.2, no signature spoofing
~~~

A12.1 image, arm64-an-floss-vndklike v416
~~~
All ok !
Best image right now.
~~~

Notes: do not install phh over stock-updated OOS12,
you will get some error messages a "phhtreble app stopped to work".

If you find this help useful, please send an email to 
angelo AT kernel-space.org, a "thanks" is welcome.
