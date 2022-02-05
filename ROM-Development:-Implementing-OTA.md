Phh-GSI includes support for seamless A/B upgrade, for all devices using dynamic partition.

Known flaws of this mechanism:
- It uses space definitely on /data. At the time of writing, it requires 4GB in /data per slot. Secondary slot is removed as soon as new slot is booted, so the average space consumption is 4GB, peak space consumption is 8GB.
- It is custom-made, it doesn't match other OTA methods made by Android
- No delta OTA
- No error detection. Meaning that if new slot doesn't boot, there is no way to fallback to previous slot


To use it, you need:
- https-accessible JSON describing current latest version, dubbed ota.json
- https-accessible xz-compressed unsparsed images
- Set `ro.system.ota.json_url` property to ota.json

About ota.json:
- The https request doesn't contain any metadata (version, device name or anything)
- Its format is like this:
```
{
    "version": "v400.h",
    "date": "1644083319",
    "variants": [
        {
            "name": "treble_arm64_bvS",
            "size": 0,
            "url": "https://github.com/phhusson/treble_experimentations/releases/download/v400.h/system-squeak-arm64-ab-vanilla.img.xz"
        }
    ]
}
```

Description of the fields using jq naming.
- '.version' => This is what will be displayed as new version to the user. This is a "user-friendly version name"
- '.date' => If ro.system.build.date.utc is smaller than '.date', then the UI will show that there is an update available. Please note that - ro.system.build.date.utc will vary from one build to the other, so from one flavor to the other, so you need to pick the lowest value for all the flavors (or take a `date +%s` before making your release)
- '.variants[0].name' => This is 'ro.build.flavor' (minus -user -userdebug) + -secure if /system/phh/secure + -vndklite if not secure and is vndklite
- '.variants[0].size' => This is what is displayed to the user as the size
- .variants[0].url' => https-accessible direct download link to unsparsed xz-compressed image