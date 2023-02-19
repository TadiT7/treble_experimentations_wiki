## I did it with a Xiaomi Redmi 9A (dandelion)


Requirements

* Stock Recovery
* Bootloader Unlocked
* [vbmeta.img](https://forum.xda-developers.com/attachments/vbmeta-img.5257631/) (you can also use the one that comes with your MIUI IMAGE)
* PC with Android-Tools (ADB/fastboot and proper drivers installed)
* Patience <3

## Step 1 - Choosing the correct image.

Choose a GSI image that matches your Android version and the CPU Architecture and Partition of the device. 

To discover what image you should use, this app makes it easier. 
https://play.google.com/store/apps/details?id=tk.hack5.treblecheck&hl=&gl=US

You can easily download it from here too 
https://www.apkmirror.com/apk/hackintosh-five/treble-info/treble-info-5-0-6-release/treble-info-5-0-6-android-apk-download/

Its safe to use.

Once in the app , the app recommends you which IMAGE you should download, gives you CPU ARCH info and tells you if phone is Aonly or A/B

In my case its A ONLY , but the app recommends me to download an A/B Image, specifically a

 " **system-arm32_binder64-ab-vanilla.img.xz**  " image. (These arm32_binder64 images are also called A64 images)

Since my last MIUI image installed was "**dandelion_global_images_V12.5.4.0.RCDMIXM_20220421.0000.00_11.0_global**" **its based on Android 11**

I HAVE to download an Android 11 image, so i went for a Lineage OS R 18.1 with the latest android 11 available. (since 18.1 is based on Android 11R , it booted)

LiR 2022.03.25 -- https://sourceforge.net/projects/treblerom/files/LiR/2022.03.25/lir-v316-220325-a64-bvZ.img.xz/download

(But if you are on Android 10, you have to download an android 10 image, if you're on 12 , you have to download an Android 12 image and so on,
you can only choose the same Android version or 1 that is above yours , bare in mind we might not be able to return to previous Android versions, so stick with your current version)


I downloaded and used " **[lir-v316-220325-a64-bvZ.img.xz](https://sourceforge.net/projects/treblerom/files/LiR/2022.03.25/lir-v316-220325-a64-bvZ.img.xz/download)** " Because our CPU supports arm32_binder64, and ab works for us. 

b = A/B , v = Vanilla , Z = Has Dynamical SuperUser ( Root can be disabled/enabled while using the phone )
Vanilla variant comes without gapps and has Root/SU.

But you can download and install any other as long as its compatible with the cpu and the partition format.
Feel free to try other Images and report.


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

Give it time. Allow your phone to boot, patience, an image with LinageOS Logo should suprise you, eventually it should boot into start menu in a few secs.
Congratulations you got rid of MIUI without any recovery, and  you got a nice debloated ROM (The best ROM or one of the BEST ROMS i should say)

(Detail, once you've disabled dm-verity with fastboot --disable-verification --disable-verity flash vbmeta vbmeta.img command
You don't have to do it again for any of these ROMS, but in case you have dm-verity corruption/error, you can do this)

### Features? = 

Well its 1.5GB size, Its debloated ! NO MORE GOOGLE, OR XIAOMI in it, at least not forced in our faces.
Since its smaller, it should be very good on the battery and because of this, performance of the phone during usage of apps should be optimal too, the best performance these 2gb ram , this cpu can offer. Its LOS + PHH-Treble combined, i mean its good.
It comes rooted by default. You won't really hard-brick ur device, or have to return to MIUI ever again, you can always use these images, and try new ones, and easily flash them through fastbootd as we did before.

What Works / Doesn't work / Hardware Info


> Component             |   | Comment
> -- | -- | --
> Camera                    | √ |  
> Audio                     | √/× | (headphone jack doesn't work, but can be fixed with a simple code on termux)
> Bluetooth                 | √ |  
> Display                   | √ | (brightness slider doesn't work / can also be fixed via termux)
> WiFi / Hotspot            | √ |  
> GPS                       | √ |  
> SIM / Mobile Data / Voice | × | (RIL dead in GSI Phh of A11 and A12, only works in Eremitein's GSI's. )
> VoLTE                     | ? | (Untested)
> Fingerprint               | √ |  
> Offline Charging          | × |  

In this LiR Image, RIL/SIM works perfectly, you have internet and calls 100% BUT
"RIL/SIM Card is dead in many A11 and A12 images,  so we have to search for images that have RIL/SIM working, or make it work ourselves"
*gulp*

IM NOT SURE YET IF WE SHOULD USE A or A/B , since our device is A-Only i suggest trying with A-Only first if it doesn't work or it's not available , try with A/B, (So far the A/B Image used in this guide works perfectly)

" Other Lists of Generic GSI's " 

* https://github.com/phhusson/treble_experimentations/releases
* https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list

"Other working GSI's" 

* Tested [CrDroid v313 by eremitein](https://sourceforge.net/projects/treblerom/files/crDRom11/2021.09.21/)
* Tested [Bless v306 by eremitein](https://sourceforge.net/projects/treblerom/files/BLESS11/2021.05.02/)
* Tested [Pixel Experience 10 by ExpressLuke](https://sourceforge.net/projects/expressluke-gsis/files/PixelExperience/Ten/A64/AB/)
* Every  [eremitein](https://sourceforge.net/projects/treblerom/files/) builds

More INFO can be found here:

https://github-wiki-see.page/m/phhusson/treble_experimentations/wiki/Frequently-Asked-Questions-(FAQ)
