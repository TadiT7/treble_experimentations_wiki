Set up a **Linux machine** – it may be the newest Ubuntu or Mint. If you aren't planning to run it alongside Windows, use a virtual machine, for example VirtualBox.

Install **apktool** by following its guide.
If there's a `framework-res__auto_generated_rro.apk`, `FrameworksResCommon.apk` (or something like that) overlay on your device in `/vendor/overlay` directory, copy it to your PC. If there's nothing like that (try searching for everything with framework and .apk in the name), install your stock system (or extract it on PC) and copy the `system/framework/framework-res.apk` file.
Whatever you found, **decompile** it by apktool.

Install **git** if you don't have it by:
`sudo apt install git`

On your desktop, open up the terminal, write:
`git clone https://github.com/phhusson/vendor_hardware_overlay.git`

Find your brand or create its directory, create a directory with your device's official name inside it. Copy some other device's `Android.mk` and replace in it:
`LOCAL_PACKAGE_NAME := treble-overlay-brand-device`

On your device, in **adb** or **Termux** app use this command:
`getprop ro.vendor.build.fingerprint`

On PC, copy `AndroidManifest.xml` and replace in it:

`package="me.phh.treble.overlay.brand.device"`

`android:requiredSystemPropertyValue="+brand/device*"`

Where brand and device for property value is what you got from that `getprop` command.

Then inside your device's directory, create a `res` folder and copy inside the `xml` folder (if exists) from apk **decompiled** by apktool. Then inside the `res`, also copy the `values` folder. Inside it, delete every file which isn't called `arrays`, `bools`, `integers`, `strings` (.xml).

Install **xmlstarlet** if you don't have it by:
`sudo apt install xmlstarlet`
Then go into `vendor_hardware_overlay/tests`, open terminal and run:
`bash tests.sh`

As a result, you'll get a recommended priority level which you should replace in your `AndroidManifest.xml`.
Inside the `overlay.mk` of main directory add your `LOCAL_PACKAGE_NAME`, in the alphabetic order.

Then if you want (but you should), go into `vendor_hardware_overlay/build/` and run:
`bash build.sh`
It'll build you an overlay which you should put in `/system/overlay/` on your device.

On GitHub, create an account and fork the **original repo** by phhusson.
Open up terminal in `vendor_hardware_overlay`, then type:

`git add --all`

`git commit -m "Add overlay for yourdevicenamehere"`

`git remote add myrepo https://github.com/yourusername/vendor_hardware_overlay.git`

`git push myrepo master`


Then use **pull request** function on GitHub and **apply to tips and guidance** by people commenting :)

If you do extra changes, repeat:

`git commit -m "Your change description"`

`git push myrepo master`