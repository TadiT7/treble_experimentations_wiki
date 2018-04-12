In an XDA thread, an early version of the phh-GSI was reported as working on the Sony XZ1.

Unfortunately, newer versions do not work.

On the XZ1 Compact, both v9 and v15 of the phh-GSI result in boot-loops when flashed over the stock 8.0.0 images 47.1.A.12.75 and 47.1.A.8.49.

**update (2018-04-11):**  test versions of the new phh-GSI are booting successfully on the XZ1 Compact!  The device is running the 47.1.A.12.75 stock firmware.  Logcat output reports some missing system libs.  Hardware support seems mostly functional (nfc, wifi, fingerprint reader).

Note that unlocked XZ1's suffer from the Sony green-screen issue, so the photographic camera does not work (the video camera does work).  For an unrelated reason, GoogleCamera (from opengapps) crashes on start-up (missing "tag" in com.google.nexus.experimental2016.jar).  Other camera apps do start up normally and can be used to capture video.
