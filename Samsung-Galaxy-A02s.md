# Samsung A02s (SM-A025F, SM-A025G, SM-A025M)

## Custom Recoveries/Kernels/Vendors :

TWRP (Unofficial) : [Click here](https://forum.xda-developers.com/t/recovery-unofficial-twrp-for-galaxy-a02s-snapdragon.4294377/)

OrangeFox (Unofficial)**(Discontinued)***: [Click here](https://forum.xda-developers.com/t/recovery-unofficial-twrp-for-galaxy-a02s-snapdragon.4294377/)

Custom Vendor** : [Telegram](https://t.me/samsung_galaxy_m01_a01_m11_a11)

***VERY UNSTABLE AND DOESN'T WORK! USE TWRP!**

**The vendor can be used to run arm64 GSIs and can also run Secure GSIs without any issue.
But do note that it is in beta and is very unstable!

## NOTES (VERY IMPORTANT!) :

##### About choosing the right GSI image :

Use binder GSI images! Binder GSI images will either be marked as **a64** or **arm32_binder64**. If you're using custom vendor, use arm64 GSIs only!

Some images might have **A/B(ab)** or **A-only** variants. Use **A/B(ab)** ones.

Only **non-secure** GSI images works on the stock vendor of the device.

##### Flashing a GSI image :
Either flash it as system image on TWRP (make sure it's a .img file).

or

Use fastboot to flash the image by using the following command (Must have TWRP) :

`fastboot flash system <your gsi img>`

Note that you shouldn't erase data using fastboot as this will **brick the partition**. Use the **Format Data** option in TWRP to do it.

##### Erasing the product partition

First, do `fastboot erase product` and then, flash the [product_gsi.img](https://forum.xda-developers.com/attachments/product_gsi-img.5371179/) by doing `fastboot flash product product_gsi.img`.

##### Other important things :

In some GSI images, there will be an option to enable **Device Spoof Properties** in the **phh Treble Options** in **Settings**. **DO NOT TURN THAT ON!** Even if you did and you restarted your device, you'll have aproximately 30 secs to **turn it back off and restart to apply the changes** before the system crashes! (On Stock Vendor & Secure-on-demand GSIs only)

**Do not use Universal SafetyNet Fix or any other module or hack that does the same thing as above! This will also cause the same issue.** (On Stock Vendor & Secure-on-demand GSIs only)

Do not enable **Use alternate audio policy** in the **phh Treble Options**. This will result in the volume buttons not working! Disable it and restart for it to work again.

If you want to be able to edit system files/make system files R/W, use **VNDKLITE** GSI images.

If you're using the custom vendor above, make sure to use the Bootloop Fix .zip to be able to boot any arm64 GSI properly!

## Installing Magisk on GSI images.

- Download the Magisk APK from the following [repo](https://github.com/topjohnwu/Magisk) in releases.
  
- In TWRP, Go to Install and select the APK and flash it.
  

Note that this method only works with non-superuser GSIs. See [this](https://github.com/phhusson/treble_experimentations/wiki/Frequently-Asked-Questions-%28FAQ%29#naming-conventions-that-some-gsi-buildermaintainer-uses) to be able to identify which image is non-superuser.


***


## List of known-working GSIs (On Stock Vendor) :

### [LeOS](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=17%20Jan-,LeOS%2020%20%26%20T,-Harvey186)
Variants : VNDK-a64-bvN/bvS , VNDKLITE-a64-bvN/bvS

### [Lineage OS 20 TD-Based](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=18%20Feb-,LineageOS%0ATD%2Dbased,-AndyYan)

Variants : a64_bvN/bvS , a64_bvN/bvS-vndklite, a64_bgN , a64_bgN-vndklite

### [Lineage 19.1](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=12%20Jan-,LineageOS%2019.1,-AndyYan)

Variants : a64_bvN/bvS , a64_bvN/bvS-vndklite , a64_bgN , a64_bgN-vndklite

### [AOSP 13](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=31%20Jan-,AOSP,-TrebleDroid%20Builders)

Variants : arm32_binder64-ab-vanilla , arm32_binder64-ab-vndklite-vanilla

### [AOSP 12.1](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=09%20Nov-,AOSP%2012.1,-Phhusson)

Variants : arm32_binder64-ab-vanilla/gogapps , arm32_binder64-ab-vndklite-vanilla/gogapps

**More GSI ROMs are being tested to see if they work! So use these ones for the time being!**

## List of known-working GSIs (On Custom Vendor) :

Almost any arm64 and secure GSIs can work on it! But, you can't run a64/arm32_binder64 GSIs on it.