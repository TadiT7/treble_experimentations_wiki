# How to build a Project Treble GSI ROM from source?

In this guide I'll try to simplify building Treble GSI process.
As you read this guide now I'll assume you already have a previous knowledge about How to build android from source, so I won't cover some points with too many basic details. **(Some contents of this tutorial were outdated. If you have any problems go to [the builders' group](https://t.me/phhtreblebuilders).) Do not use dakkar or build-rom anymore!**
So, let's start:

**What you’ll need:**

* A treble enabled device, basically all devices that come with Android 8.1 out of box support it.
* A relatively recent 64-bit computer (Linux, macOS, or Windows) with a reasonable amount of RAM and about 120 GB of free storage (more if you enable ccache or build for multiple devices). The less RAM you have, the longer the build will take (aim for 16 GB or more). Using SSDs results in considerably faster build times than traditional hard drives.
* A USB cable compatible with your device
* A decent internet connection & reliable electricity :)
* Some familiarity with basic Android operation and terminology. It would help if you’ve installed custom ROMs on other devices and are familiar with recovery. It may also be useful to know some basic command line concepts such as cd for “change directory”, the concept of directory hierarchies, that in Linux they are separated by /. etc.


**Summary**
* 1. Install SDK
* 2. Install build packages
* 3. Install the repo command
* 4. Configure git
* 5. Turn on caching to speed up build
* 6. Build using phhusson's script (AOSP only)
* 8. Build using the manual way (Custom ROMs and AOSP)

### 1. Install SDK
If you haven’t previously installed `adb` and `fastboot`, you can [download them from Google](https://dl.google.com/android/repository/platform-tools-latest-linux.zip).
Extract it using: ```unzip platform-tools-latest-linux.zip -d ~```

Now we have to add `adb` and `fastboot` to our path. Open ~/.profile and add the following:

```
# add Android SDK platform tools to path
if [ -d "$HOME/platform-tools" ] ; then
    PATH="$HOME/platform-tools:$PATH"
fi
```


Then, run this to update your environment. ```source ~/.profile```

### 2. Install build packages

Several packages are needed to build Android and execute the scripts. You can install these using your distribution’s package manager. Use libwxgtk3.0-dev in place of libwxgtk3.0-gtk3-dev for earlier versions of Ubuntu (before 20.04) 
You’ll need:

```
bc bison build-essential curl flex g++-multilib gcc-multilib git gnupg gperf libxml2 \
lib32z1-dev liblz4-tool libncurses5-dev libsdl1.2-dev libwxgtk3.0-gtk3-dev imagemagick git \
lunzip lzop schedtool squashfs-tools xsltproc zip zlib1g-dev openjdk-8-jdk python perl  \
xmlstarlet virtualenv xz-utils rr jq libncurses5 pngcrush lib32ncurses5-dev git-lfs libxml2 \
openjdk-11-jdk-headless
```

### 3. Install the repo command

Enter the following to download the repo binary and make it executable (runnable):

```
mkdir -p ~/bin
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
chmod a+x ~/bin/repo
```

Put the ~/bin directory in your path of execution

In recent versions of Ubuntu, ~/bin should already be in your PATH. You can check this by opening ~/.profile with a text editor and verifying the following code exists (add it if it is missing):

```
# set PATH so it includes user's private bin if it exists
if [ -d "$HOME/bin" ] ; then
    PATH="$HOME/bin:$PATH"
fi
```

Then, use this to update your environment.

```source ~/.profile```

### 4. Configure git

You’ll need to set up git identity in order to sync the source, run these commands:

```
git config --global user.name "your username"
git config --global user.email yourmail@example.com
```

### 5. Turn on caching to speed up build

You can speed up subsequent builds by running:

```
export USE_CCACHE=1
export CCACHE_COMPRESS=1
export CCACHE_MAXSIZE=50G # 50 GB
```

And adding these lines to your ~/.bashrc OR ~/.zshrc file. 

You can configure the maximum amount of disk space you want the cache to use by editing `CCACHE_MAXSIZE` consequently. Anywhere from 25GB-100GB will result in very noticeably increased build speeds (for instance, a typical 1hr build time can be reduced to 20min). If you’re only building for one device, 25GB-50GB is fine. If you plan to build for several devices that do not share the same kernel source, aim for 75GB-100GB. This space will be permanently occupied on your drive, so take this into consideration.

### 6. Build using phhusson's script - AOSP only (build.sh)

If you encounter problems with the build-rom.sh script, you might consider using the newer script. Keep in mind that we'll need to modify it a bit, otherwise it will build system images for all possible options (all architectures, all partition options, all gapps choices,etc.).

1- Start by cloning phh's Treble_Experimentations project:

```
git clone https://github.com/phhusson/treble_experimentations
```

2. Start the build. We will create a folder named AOSP12, enter it and then call the build script.

```
mkdir AOSP12; cd AOSP12
bash ../treble_experimentations/build.sh android-12.0
```
The resulting system images will be stored in the release folder.

### 7. Build using the manual way

In simple steps:

1. Repo init the rom you want to build GSI for.
```
mkdir ~/rom &&  cd ~/rom
repo init -u https://github.com/LineageOS/android.git -b lineage-19.1
```

2. Add phh repos to your local_manifest
```
git clone https://github.com/phhusson/treble_manifest .repo/local_manifests -b android-12.0
```
After git clone you need to remove or delete replace.xml (.repo/local_manifests/replace.xml) if you're building any rom except AOSP GSI.

3. Sync the source

```
repo sync -c -j6 --force-sync --no-tags --no-clone-bundle
```

4. Modify the source to fix issues in other devices using one of these methods:

- Apply [phh patches](https://github.com/phhusson/treble_experimentations/releases/latest/download/patches-for-developers.zip):

Download [the patches](https://github.com/phhusson/treble_experimentations/releases/latest/download/patches-for-developers.zip)

Then apply each path in its project

```
git am patch
```

5. Go to the phh device repo and run `bash generate.sh vendor/lineage/config/common_full_phone.mk` - adapting for the rom you wish to build for. 

6. Lunch the [build variant](https://github.com/phhusson/treble_experimentations/blob/master/build.sh#L380) you want (ex. treble_arm64_avN-userdebug) and start the build

```
. build/envsetup.sh
lunch treble_arm64_avN-userdebug
WITHOUT_CHECK_API=true make -j$(nproc) systemimage
```

7. If you want to compress the system image after build finishes, go to out/target/product/phh_*/ folder and run

```
xz -9 -T0 -v -z system.img
```

That's all ;)

**Credits:**
- @phhusson for all his contributions, without his efforts this can't be possible.
- @Dakkar for his build script
- @faiyazsheth for helping me build my first GSI
- @sooti for his simplified instruction on phh-treble telegram.
- @LineageOS guys for their wiki
- And me (@yshalsager) for writing this guide :D	

**Edit Notes:**
- @Dualkem - added the build.sh build guide (point 7).
- @00p513-dev - Initial changes for 2021
- @TQMatvey Updated everything to Android 12 and other minor tweaks