- Rebuild treble_app (`bash build.sh`), copy signed apk (./app.apk) to vendor_hardware_overlay/pie
- Rebase -i vendor_hardware_overlay:pie on top of vendor_hardware_overlay:master
- For all repos in .repo/local_manifests/replace.xml; rebase branches:
`git fetch aosp --tags && git fetch aosp && git fetch aosp android-9.0.0_r35 && git checkout -b android-9.0.0_r35-phh && git rebase -i android-9.0.0_r35 && git push phh android-9.0.0_r35-phh`
- Edit local_manifests/replace.xml to switch all branches to the new tag version
- Edit treble_experimentations/build.sh to update to new tag version

- `git config --global user.name 'Pierre-Hugues Husson'`
- `git config --global user.email phh@phh.me`
- `git config --global color.ui auto`
- `dpkg --add-architecture i386 && apt-get update && apt-get install -y build-essential imagemagick xorriso locales openjdk-8-jdk python git m4 unzip bison zip gperf libxml2-utils zlib1g:i386 libstdc++6:i386 bc curl lzop lzip lunzip squashfs-tools sudo`
- git clone https://github.com/phhusson/treble_experimentations/
- edit treble_experimentations/build.sh for:
  - `repo sync -j1` to `repo sync -j12`
  - `make -j8` to `make -j64`
- Create treble_experimentations/release/config.ini with:
```
[github]
token=XXXXX
```