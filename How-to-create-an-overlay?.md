## First of all
This guide is made for devices providing Treble with **stock vendor**. For devices with only unofficial implementation, cooperate directly with the unofficial vendor provider.

Set up a **Linux machine** – it may be the newest Ubuntu or Mint. If you aren't planning to run it alongside Windows, use a virtual machine, for example VirtualBox, or build with Jenkins.

## Make overlay

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

## Build with your own PC

Install **xmlstarlet** if you don't have it by:
`sudo apt install xmlstarlet`
Then go into `vendor_hardware_overlay/tests`, open terminal and run:
`bash tests.sh`

As a result, you'll get a recommended priority level which you should replace in your `AndroidManifest.xml`.
Inside the `overlay.mk` of main directory add your `LOCAL_PACKAGE_NAME`, in the alphabetic order.

Then if you want (but you should), go into `vendor_hardware_overlay/build/` and run:
`bash build.sh`
It'll build you an overlay which you should put in `/system/product/overlay/` on your device.

## Build with Jenkins

Before building, you should push your commit into Github first.

Install **xmlstarlet** on your remote server if you don't have it by:
`sudo apt install xmlstarlet`

Set a new job in Jenkins (Freestyle project is OK)

Navigate to `General` section, click `ADVANCED...`, then make `Use custom workspace` checked.

Then set a path (what you like, e.g: `/tmp/overlay`) into `Directory` field.

Navigate to `Build` section, click `ADD BUILD STEP`, then select `Execute shell`.

Copy following codes into `Command` field:

```shell
#!/bin/bash

git clone https://github.com/yourusername/vendor_hardware_overlay.git
cd vendor_hardware_overlay
git checkout master
cd build
chmod u+x ./build.sh
./build.sh
cd ../tests
chmod u+x tests.sh
./tests.sh
```

After that, navigate to `Post-build Actions`, click `ADD POST-BUILD ACTION`, then select `Archive the artifacts`.

Input `vendor_hardware_overlay/build/*.apk` into `Files to archive` field.

Click `ADD POST-BUILD ACTION` again, then select `Delete workspace when build is done`.

Finally, Click `Save`, and click `Build Now`.

(Don't forget to view `Console Output`, it will show errors here.)

If build succeeded, you can see there's a link named `Last Successful Artifacts`.

Then click `(all files in zip)` to download your overlay files.

## Push to Github

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

If you create a messy pile of commits or your git "stops working", copy your changes somewhere else, clone **original** (phhusson) repo again, paste your changes into the newly downloaded one and force push them by:
`git add --all`

`git commit -m "Add overlay for yourdevicenamehere"`

`git remote add myrepo https://github.com/yourusername/vendor_hardware_overlay.git`

and: `git push -f myrepo master`