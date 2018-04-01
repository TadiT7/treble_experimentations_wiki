**FULL TREBLE support implemented by JDCTeam (Big thanks to @sirmordred)**

**Device codename:** gemini

**XDA Thread:** https://forum.xda-developers.com/mi-5/development/jdcteam-treble-support-project-t3761296

**Current version:** v3 (20180329) BETA

**Changelog:**

**v3** (20180329) - Beta status with the following updates:
- Updated camera Hal from latest qualcomm 8996 repo
- Hexedited more libs and removed more vendor <-> system dependency (better treble and preparation for versioned vndk)
- Updated wifi configs from lates CAF

**v2** (20180318) - Still alpha build but with the following updates:
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