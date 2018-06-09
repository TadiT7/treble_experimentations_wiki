Here are some answers to the most asked questions about GSIs and Project Treble in general:

### What is Google’s Project Treble?

A good overview of Project Treble is provided in the following XDA article by M. Rahman:
[Google’s Project Treble Modularizes Android so OEMs can Update Devices Faster](https://www.xda-developers.com/googles-project-treble-modularize-android-so-oems-can-update-devices-faster/)

For a more technical discussion of Treble, take a listen to Episode 75 of the Android Developers Backstage podcast: http://androidbackstage.blogspot.ca/2017/08/episode-75-project-treble-for-hal-of-it.html

### Why is it called "treble"?

It might be a play on the Meghan Trainor song [All About That Bass](https://youtu.be/7PCkvCPvDXk). That fits because Project Treble is all about standardizing the **base** of Android; i.e. it's about standardizing the APIs that allow the Android framework to communicate with hardware components.

### How can I check if my device is treble-enabled?<br/>

[Method 1](https://play.google.com/store/apps/details?id=com.kevintresuelo.treble) - [Method 2](https://www.xda-developers.com/project-treble-android-oreo/)

Note that any device that launched with Oreo on it must be treble-enabled.

You can find an updated supported devices list here: [[Home]]

### What is a GSI?

GSI stands for Generic System Image.  It is a file-system image that you flash to your device's system partition.  It is generic because it accesses hardware using the new standardized hardware APIs (so it should work on any treble-enabled device).

You can find an updated list for avilable GSIs here: [[Generic System Image (GSI) list]]

### What does "AB" and "A-only" mean? Should I use an "AB" GSI or an "A-only" GSI?

phh has provided "AB" and "A-only" GSIs.  The terms "AB" and "A-only" (or just "A") refer to the partition style used by a device.

The AB partition style was introduced in Android N to support [seamless OTA updates](https://source.android.com/devices/tech/ota/ab/).

A-only, A, or non-AB refers to the [legacy partition style](https://source.android.com/devices/tech/ota/nonab/).

If you have an AB device, then you must flash it with an AB GSI.  If you have an A-only device, then you must flash it with an A-only GSI.  The two types of system images are not compatible with each other.

### How do I flash a GSI?

First, you must unlock your bootloader; that is a capability your device manufacturer may or may not offer to end-users.

For more complete information, please see the following XDA article by M. Rahman:
[How to flash a Generic System Image (GSI) on Project Treble supported devices](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/)

### How to build a GSI?

Follow this guide [Here](https://github.com/phhusson/treble_experimentations/wiki/How-to-build-a-GSI%3F)

***

this page will be updated soon with more....