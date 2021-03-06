**FULL TREBLE support implemented by JDCTeam (Big thanks to @sirmordred)**

**Device codename:** gemini

**XDA Thread:** https://forum.xda-developers.com/mi-5/development/jdcteam-treble-support-project-t3761296

**Current version:** v6 (20190316) RC2 versioned_vndk

**Changelog:**

**v6** (20190316) - Release Candidate 2 full versioned_vndk v28
- VERSİONED_VNDK support is fully implemented
- FIXED NFC support
- FIXED Ambient Display main icon size and settings menu icons style
- FIXED ConfigPanel - Fingerprint settings menu icons style


**v5** (20190308) - Release Candidate full versioned_vndk v28
- VERSİONED_VNDK support is fully implemented
- Mostly all library dependencies between system/vendor are succesfully eliminated
- Updated kernel (enforced)
- **ro.vendor.vndk.version=28**
- misc updates and fixes

**v4** (20180409) - Beta partially versioned_vndk with the following updates:
- Updated kernel and ready for versioned_vndk support
- Hexedited last libs and removed mostly all vendor/system dependency (versioned vndk)
- **ro.vendor.vndk.version=27.1.0**
- misc updates and fixes

**v3** (20180329) - Beta build with the following updates:
- Updated camera Hal from latest qualcomm 8996 repo
- Hexedited more libs and removed more vendor <-> system dependency (better treble and preparation for versioned vndk)
- Updated wifi configs from lates CAF

**v2** (20180318) - Alpha build with the following updates:
- Upstreamed kernel
- Hexedited blobs to correct path (for treble)
- Linker issues fixed
- Vendor overlays
- Latest device tree updates from CAF and miui oreo beta
- Disabled non-working apps (custom xiaomi doze package and configpanel app which were designed to work with LOS APIs)
- Disabled userspace thermal hal initialization which we dont have in cameraHal (faster cam launch)
- Increased jpeg quality parameters
- other misc. dev tree updates

**v1** (20180310) - Initial release (Alpha)

Enjoy!