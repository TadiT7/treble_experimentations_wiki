# How to build a Project Treble GSI ROM from source?

In this guide I'll try to simplify building Treble GSI process.
As you read this guide now I'll assume you already have a previous knowledge about How to build android from source, so I won't cover some points with too many basic details.
So, let's start:

**What you’ll need:**

* A treble enabled device, basically all devices that come with Android 8.1 out of box support it.
* A relatively recent 64-bit computer (Linux, OS X, or Windows) with a reasonable amount of RAM and about 100 GB of free storage (more if you enable ccache or build for multiple devices). The less RAM you have, the longer the build will take (aim for 8 GB or more). Using SSDs results in considerably faster build times than traditional hard drives.
* A USB cable compatible with your device
* A decent internet connection & reliable electricity :)
* Some familiarity with basic Android operation and terminology. It would help if you’ve installed custom ROMs on other devices and are familiar with recovery. It may also be useful to know some basic command line concepts such as cd for “change directory”, the concept of directory hierarchies, that in Linux they are separated by /. etc.


**Summary**
* 1. Install SDK
* 2. Install build packages
* 3. Install the repo command
* 4. Configure git
* 5. Turn on caching to speed up build
* 6. Build using phhusson's script
* 7. Build using dakkar's script
* 8. Build using the manual way

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

Several packages are needed to build Android. You can install these using your distribution’s package manager.
You’ll need:

```
bc bison build-essential curl flex g++-multilib gcc-multilib git gnupg gperf imagemagick lib32ncurses5-dev
lib32z1-dev liblz4-tool libncurses5-dev libsdl1.2-dev libwxgtk3.0-dev
libxml2 libxml2-utils lzop pngcrush schedtool squashfs-tools xsltproc zip zlib1g-dev openjdk-8-jdk
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

And adding these lines to your ~/.bashrc file. 

You can configure the maximum amount of disk space you want the cache to use by editing `CCACHE_MAXSIZE` consequently. Anywhere from 25GB-100GB will result in very noticeably increased build speeds (for instance, a typical 1hr build time can be reduced to 20min). If you’re only building for one device, 25GB-50GB is fine. If you plan to build for several devices that do not share the same kernel source, aim for 75GB-100GB. This space will be permanently occupied on your drive, so take this into consideration. See more information about ccache on [Google’s Android build environment initialization page](https://source.android.com/source/initializing.html#setting-up-ccache).

### 6. Build using phhusson's script

We can't deny that @phhusson has made amazing works and countless contributions to Project Treble ROMs development apart from his [experimentations](https://github.com/phhusson/treble_experimentations/) is a build script which make build a GSI super simple job.

By default, it supports building LineageOS - RR - Carbon.

1- Open your terminal and run:

```git clone https://github.com/phhusson/treble_experimentations```

2- To clone and build enter the following command and replace "romname" with `lineage|rr|carbon`

```
mkdir romname; cd romname
bash ../treble_experimentations/build-rom.sh android-8.1 romname
```

3- The script will automatically initialize the repository, sync the source, apply patches and start building.

### 7. Build using @dakkar script

dakkar's script is another treble building script, originally made by @Dakkar and improved by contributors on [treble experimentations](https://github.com/phhusson/treble_experimentations/) repo. It's customizable, easy to understand and can build almost all [ROMs](https://github.com/phhusson/treble_experimentations/blob/master/build-dakkar.sh#L29") with simple [edits](https://github.com/phhusson/treble_experimentations/commit/a5e1b285cb3a3c0430a85b2ad8db16cbee3328f5).

1- Open your terminal and run:

```git clone https://github.com/phhusson/treble_experimentations```

2- To start the process:

```bash ../treble_experimentations/build-dakkar.sh romname variant```

> Variants are dash-joined combinations of (in order):
> * processor type
>   * "arm" for ARM 32 bit
>   * "arm64" for ARM 64 bit
> * A or A/B partition layout ("aonly" or "ab")
> * GApps selection
>   * "vanilla" to not include GApps
>   * "gapps" to include opengapps
>   * "go" to include gapps go
> * SU selection ("su" or "nosu")
> for example:
> * arm-aonly-vanilla-nosu
> * arm64-ab-gapps-su

**Note:** check patches when you use these auto scripts, if some patch is broken you'll have build errors :p

### 8. Build using the manual way

In simple steps:

1. Repo init the rom you want to build GSI for.
```
mkdir ~/rom &&  cd ~/rom
repo init -u https://github.com/LineageOS/android.git -b lineage-15.1
```

2. Add phh repos to your local_manifest
```
git clone https://github.com/phhusson/treble_manifest .repo/local_manifests -b android-8.1
```
After git clone you need to remove replace.xml if you're building any rom expect aosp.

3. Sync the source

```
repo sync -c -j4 --force-sync --no-tags --no-clone-bundle
```

4. Modify the source to fix issues in other devices using one of these methods:

- Apply [phh patches](https://github.com/phhusson/treble_patches/tree/android-8.1/patches):

```
git clone https://github.com/phhusson/treble_patches -b android-8.1
```

Then apply each path in its project

```
patch -p1 < patch
```

- Or cherry-pick changes by phhusson from here, remember to choose the latest branch

[platform_build](https://github.com/phhusson/platform_build/) - [platform_external_selinux](https://github.com/phhusson/platform_external_selinux) - [platform_frameworks_av](https://github.com/phhusson/platform_frameworks_av) - [platform_frameworks_base](https://github.com/phhusson/platform_frameworks_base) - [platform_frameworks_native](https://github.com/phhusson/platform_frameworks_native) - [platform_frameworks_opt_telephony](https://github.com/phhusson/platform_frameworks_opt_telephony) - [platform_system_bt](https://github.com/phhusson/platform_system_bt) - [platform_system_core](https://github.com/phhusson/platform_system_core) - [platform_system_libvintf](https://github.com/phhusson/platform_system_libvintf) - [platform_system_vold](https://github.com/phhusson/platform_system_vold)

```git fetch repo branch && git cherry-pick commit```

5. Go to the phh device repo and edit the .mk for your ROM (example lineage.mk)

6. Lunch the [build varaint](https://github.com/phhusson/treble_experimentations/blob/master/build.sh#L380) you want (ex. treble_arm64_avN-userdebug) and start the build

```
. build/envsetup.sh
lunch treble_arm64_avN-userdebug
WITHOUT_CHECK_API=true make -j8 systemimage
```

7. If you want to compress the system image after build finishes, go to out/target/product/phh_*/ folder and run

```
xz -c system.img > system.img.xz
```

That's all ;)

**Credits:**
- @phhusson for all his contributions, without his efforts this can't be possible.
- @Dakkar for his build script
- @faiyazsheth for helping me build my first GSI
- @sooti for his simplified instruction on phh-treble telegram.
- @LineageOS guys for their wiki
- And me (@yshalsager) for writing this guide :D	