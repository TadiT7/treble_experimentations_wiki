## I did it with a Xiaomi Redmi 9A (dandelion)


Requirements

* Stock Recovery
* Bootloader Unlocked
* [vbmeta.img](https://forum.xda-developers.com/attachments/vbmeta-img.5257631/) (you can also use the one that comes with your MIUI IMAGE)
* PC with Android-Tools (ADB/fastboot and proper drivers installed)
* Patience <3

## Step 1 - Choosing the correct image.

 choose a GSI image that matches your Android version and the CPU Architecture and Partition of the device. 

To discover what image should you use, this app makes it easier. 
https://play.google.com/store/apps/details?id=tk.hack5.treblecheck&hl=&gl=US

You can easily download it from here too 
https://www.apkmirror.com/apk/hackintosh-five/treble-info/treble-info-5-0-6-release/treble-info-5-0-6-android-apk-download/

Its safe to use.

Once in the app , the app recommends you which IMAGE you should download, gives you CPU ARCH info and tells you if phone is Aonly or A/B

In my case its A ONLY , but the app recommends me to download an A/B Image, specifically a
 " **system-arm32_binder64-ab-vanilla.img.xz**  " image.

Since my last MIUI image installed was " **dandelion_global_images_V12.5.4.0.RCDMIXM_20220421.0000.00_11.0_global** " **its based on Android 11**

I HAVE to download an Android 11 image, so i went with the latest android 11 that phhusson released.

AOSP 11.0 v313 -- https://github.com/phhusson/treble_experimentations/releases/tag/v313

(But if you are on Android 10, you have to download an android 10 image, if you're on 12 , you have to download an Android 12 image and so on,
you can only choose the same Android version or 1 that is above yours , bare in mind we might not be able to return to previous Android versions, so stick with your current version)


I downloaded and used " **system-roar-arm32_binder64-ab-vanilla.img.xz** " Because our system uses arm32_binder64, and ab will work for us. 

Vanilla variant comes without gapps and has Root/SU, but you can download "system-roar-arm32_binder64-ab-gapps.img.xz " 
the gapps variant. (I don't know if it has root)


system-roar-arm32_binder64-ab-vndklite-vanilla.img.xz  -- the vndklite variant should also work for us, but im not sure, this optimizes system memory, cpu usage and storage. (haven't tried it yet)

## Step 2 - You have your Image time to flash it.

Unpack your .img.xz , inside you will find your .img file , rename it to system.img

Move this system.img and your vbmeta.img to your adb folder if necessary.

Now reboot into Fastboot Mode (turn phone off, hold power and vol - )

and use these commands:

     fastboot devices
     fastboot --disable-verification --disable-verity flash vbmeta vbmeta.img
     fastboot reboot fastboot

We've now entered into fastbootd mode
and we continue with these commands:

    fastboot getvar is-userspace 
( it should reply with "is-userspace: yes" , this is good, it means we're good to go)

Continue with these commands:

    fastboot erase system
    fastboot flash system system.img
    fastboot reboot recovery

Once inside the default recovery, choose to wipe data, and now reboot to system. 

Allow your phone to boot, an image with donald ducks should suprise you, eventually it should boot into home in few secs.
Congratulations you got rid of MIUI without any recovery, and  you got a nice debloated ROM.

### Features? = 

Well its 352.40 mb size, Its debloated ! NO MORE GOOGLE, OR XIAOMI in it, at least not forced in our faces.
Since its so small , it should be very good on the battery and beccause of this performance of the phone during usage of apps should be optimal too, the best performance these 2gb ram , this cpu can offer.
It comes rooted by default.

