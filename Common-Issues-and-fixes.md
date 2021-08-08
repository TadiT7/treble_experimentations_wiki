> ***This sub-page is highly dependant on user contributions based on their experiences***

> ***This sub page gives many fixes within phh settings which can be located in settings***

**1. can't listen to anything on phone calls**

`Possible solutions:`

`1. Try disabling a2dp overload from phh settings in settings and reboot `

**2. Maximum brightness is too low**

`Possible solutions:`

`1. Enable alternate backlight scale and linear in phh settings`

**3. Wired headphones not getting detected**

`Possible solutions:`

`1. Enable alternative headphones detection in phh settings and reboot`  
`2. adb shell setprop persist.sys.overlay.devinputjack true`

**4. Fingerprint sensor not getting detected**

`Possible solutions:`

`1. adb shell setprop persist.sys.phh.fingerprint.nocleanup true`

**5. High refresh rate not working**

`Possible solutions`

`1. Check force refresh rate option in phh settings`  

(Method 2 tested only on some oppo/realme/oneplus, do with caution)  
`2. adb shell -c service call SurfaceFlinger 1035 i32 0`