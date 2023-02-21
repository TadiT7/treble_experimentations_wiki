# Samsung A02s (SM-A025F, SM-A025G, SM-A025M)

## Custom Recoveries Available :

TWRP (Unofficial) : [Click here](https://forum.xda-developers.com/t/recovery-unofficial-twrp-for-galaxy-a02s-snapdragon.4294377/)

OrangeFox (Unofficial)**(Discontinued)***: [Click here](https://forum.xda-developers.com/t/recovery-unofficial-twrp-for-galaxy-a02s-snapdragon.4294377/)

***VERY UNSTABLE AND DOESN'T WORK! USE TWRP!**

## NOTES (VERY IMPORTANT!) :

##### About choosing the right GSI image :

Use binder GSI images! Binder GSI images will either be marked as **a64** or **arm32_binder64**.

Some images might have **A/B(ab)** or **A-only** variants. Use **A/B(ab)** ones.

Only **non-secure** GSI images works on the device!

If the image is marked with **secure**, this means that it **doesn't support** the device!

If you flash a GSI image and it crashes after some seconds after booting up, this might mean that the **GSI image is secure**!

All GSI images made by **Nazim** are secure! So don't use them!

##### Other important things :

In GSI images made by **AndyYan**, there will be an option to enable **Device Spoof Properties** in the **phh Treble Options** in **Settings**. **DO NOT TURN THAT ON!** Even if you did and you restarted your device, you'll have aproximately 30 secs to **turn it back off and restart to apply the changes** before the system crashes!

**Do not use Universal SafetyNet Fix or any other module or hack that does the same thing as above! This will also cause the same issue.**

Do not enable **Use alternate audio policy** in the **phh Treble Options**. This will result in the volume buttons not working! Disable it and restart for it to work again.

If you want to be able to edit system files/make system files R/W, use **VNDKLITE** GSI images.

## Installing Magisk on GSI images.

- Download the Magisk APK from the following [repo](https://github.com/topjohnwu/Magisk) in releases.
  
- In TWRP, Go to Install and select the APK and flash it.
  

Note that this method only works with non-superuser GSIs. See [this](https://github.com/phhusson/treble_experimentations/wiki/Frequently-Asked-Questions-%28FAQ%29#naming-conventions-that-some-gsi-buildermaintainer-uses) to be able to identify which image is non-superuser.


***


## List of known-working GSIs :

### [LeOS](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=17%20Jan-,LeOS%2020%20%26%20T,-Harvey186)
Variants : VNDK-a64-bvN/bvS , VNDKLITE-a64-bvN/bvS

### [Lineage OS 20 TD-Based](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=18%20Feb-,LineageOS%0ATD%2Dbased,-AndyYan)

Variants : a64_bvN/bvS , a64_bvN/bvS-vndklite

### [Lineage 19.1](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=12%20Jan-,LineageOS%2019.1,-AndyYan)

Variants : a64_bvN/bvS , a64_bvN/bvS-vndklite , a64_bgN , a64_bgN-vndklite

### [AOSP 13](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=31%20Jan-,AOSP,-TrebleDroid%20Builders)

Variants : arm32_binder64-ab-vanilla , arm32_binder64-ab-vndklite-vanilla

### [AOSP 12.1](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list#:~:text=09%20Nov-,AOSP%2012.1,-Phhusson)

Variants : arm32_binder64-ab-vanilla/gogapps , arm32_binder64-ab-vndklite-vanilla/gogapps

**More GSI ROMs are being tested to see if they work! So use these ones for the time being!**